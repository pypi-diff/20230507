# Comparing `tmp/junitparser-3.0.0.tar.gz` & `tmp/junitparser-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junitparser-3.0.0.tar", last modified: Sat Apr 22 04:09:03 2023, max compression
+gzip compressed data, was "junitparser-3.1.0.tar", last modified: Sun May  7 02:29:50 2023, max compression
```

## Comparing `junitparser-3.0.0.tar` & `junitparser-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:09:03.271137 junitparser-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-22 04:08:55.000000 junitparser-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-22 04:09:03.271137 junitparser-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-04-22 04:08:55.000000 junitparser-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:09:03.271137 junitparser-3.0.0/junitparser/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-22 04:08:55.000000 junitparser-3.0.0/junitparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-22 04:08:55.000000 junitparser-3.0.0/junitparser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-22 04:08:55.000000 junitparser-3.0.0/junitparser/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21378 2023-04-22 04:08:55.000000 junitparser-3.0.0/junitparser/junitparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 04:09:03.271137 junitparser-3.0.0/junitparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 04:09:03.000000 junitparser-3.0.0/junitparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-22 04:08:55.000000 junitparser-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-22 04:09:03.271137 junitparser-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-22 04:08:55.000000 junitparser-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:29:50.963492 junitparser-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-07 02:29:46.000000 junitparser-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-05-07 02:29:50.963492 junitparser-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-07 02:29:46.000000 junitparser-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:29:50.963492 junitparser-3.1.0/junitparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 02:29:46.000000 junitparser-3.1.0/junitparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 02:29:46.000000 junitparser-3.1.0/junitparser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-07 02:29:46.000000 junitparser-3.1.0/junitparser/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21619 2023-05-07 02:29:46.000000 junitparser-3.1.0/junitparser/junitparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-07 02:29:46.000000 junitparser-3.1.0/junitparser/xunit2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:29:50.963492 junitparser-3.1.0/junitparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-05-07 02:29:50.000000 junitparser-3.1.0/junitparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-07 02:29:50.000000 junitparser-3.1.0/junitparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:29:50.000000 junitparser-3.1.0/junitparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 02:29:50.000000 junitparser-3.1.0/junitparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:29:50.000000 junitparser-3.1.0/junitparser.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 02:29:50.000000 junitparser-3.1.0/junitparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 02:29:50.000000 junitparser-3.1.0/junitparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-07 02:29:46.000000 junitparser-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 02:29:50.963492 junitparser-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-07 02:29:46.000000 junitparser-3.1.0/setup.py
```

### Comparing `junitparser-3.0.0/LICENSE` & `junitparser-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `junitparser-3.0.0/PKG-INFO` & `junitparser-3.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junitparser
-Version: 3.0.0
+Version: 3.1.0
 Summary: Manipulates JUnit/xUnit Result XML files
 Home-page: https://github.com/weiwei/junitparser
 Author: Weiwei Wang
 Author-email: gastlygem@gmail.com
 License: Apache 2.0
 Keywords: junit xunit xml parser
 Classifier: Development Status :: 5 - Production/Stable
@@ -141,14 +141,47 @@
     newxml = xml1 + xml2
     # Alternatively, merge in place
     xml1 += xml2
 
 Note that it won't check for duplicate entries. You need to deal with them on
 your own.
 
+Schema Support
+~~~~~~~~~~~~~~~
+
+By default junitparser supports the schema of windyroad_, which is a relatively
+simple schema. 
+
+.. _windyroad: https://github.com/windyroad/JUnit-Schema/blob/master/JUnit.xsd
+
+Junitparser also support extra schemas:
+
+.. code-block:: python
+
+    from junitparser.xunit2 import JUnitParser, TestCase, TestSuite, \
+        RerunFailure
+    # These classes are redefined to support extra properties and attributes
+    # of the xunit2 schema.
+    suite = TestSuite("mySuite")
+    suite.system_err = "System err" # xunit2 specific property
+    case = TestCase("myCase")
+    rerun_failure = RerunFailure("Not found", "404") # case property
+    rerun_failure.stack_trace = "Stack"
+    rerun_failure.system_err = "E404"
+    rerun_failure.system_out = "NOT FOUND"
+    case.add_rerun_result(rerun_failure)
+
+Currently supported schemas including:
+
+- xunit2_, supported by pytest, Erlang/OTP, Maven Surefire, CppTest, etc.
+
+.. _xunit2: https://github.com/jenkinsci/xunit-plugin/blob/xunit-2.3.2/src/main/resources/org/jenkinsci/plugins/xunit/types/model/xsd/junit-10.xsd
+
+PRs are welcome to support more schemas.
+
 Create XML with custom attributes
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You want to use an attribute that is not supported by default.
 
 .. code-block:: python
```

### Comparing `junitparser-3.0.0/README.rst` & `junitparser-3.1.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -125,14 +125,47 @@
     newxml = xml1 + xml2
     # Alternatively, merge in place
     xml1 += xml2
 
 Note that it won't check for duplicate entries. You need to deal with them on
 your own.
 
+Schema Support
+~~~~~~~~~~~~~~~
+
+By default junitparser supports the schema of windyroad_, which is a relatively
+simple schema. 
+
+.. _windyroad: https://github.com/windyroad/JUnit-Schema/blob/master/JUnit.xsd
+
+Junitparser also support extra schemas:
+
+.. code-block:: python
+
+    from junitparser.xunit2 import JUnitParser, TestCase, TestSuite, \
+        RerunFailure
+    # These classes are redefined to support extra properties and attributes
+    # of the xunit2 schema.
+    suite = TestSuite("mySuite")
+    suite.system_err = "System err" # xunit2 specific property
+    case = TestCase("myCase")
+    rerun_failure = RerunFailure("Not found", "404") # case property
+    rerun_failure.stack_trace = "Stack"
+    rerun_failure.system_err = "E404"
+    rerun_failure.system_out = "NOT FOUND"
+    case.add_rerun_result(rerun_failure)
+
+Currently supported schemas including:
+
+- xunit2_, supported by pytest, Erlang/OTP, Maven Surefire, CppTest, etc.
+
+.. _xunit2: https://github.com/jenkinsci/xunit-plugin/blob/xunit-2.3.2/src/main/resources/org/jenkinsci/plugins/xunit/types/model/xsd/junit-10.xsd
+
+PRs are welcome to support more schemas.
+
 Create XML with custom attributes
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You want to use an attribute that is not supported by default.
 
 .. code-block:: python
```

### Comparing `junitparser-3.0.0/junitparser/cli.py` & `junitparser-3.1.0/junitparser/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,24 +61,27 @@
     merge_parser.add_argument(
         "--suite-name",
         help="Name added to <testsuites>.",
     )
 
     # command: verify
     merge_parser = command_parser.add_parser(
-        "verify", help="Return a non-zero exit code if one of the testcases failed or errored."
+        "verify",
+        help="Return a non-zero exit code if one of the testcases failed or errored.",
     )
     merge_parser.add_argument(
         "--glob",
         help="Treat original XML path(s) as glob(s).",
         dest="paths_are_globs",
         action="store_true",
         default=False,
     )
-    merge_parser.add_argument("paths", nargs="+", help="XML path(s) of reports to verify.")
+    merge_parser.add_argument(
+        "paths", nargs="+", help="XML path(s) of reports to verify."
+    )
 
     return parser
 
 
 def main(args=None, prog_name=None):
     """CLI's main runner."""
     args = args or _parser(prog_name=prog_name).parse_args()
```

### Comparing `junitparser-3.0.0/junitparser/junitparser.py` & `junitparser-3.1.0/junitparser/junitparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 junitparser is a JUnit/xUnit Result XML Parser. Use it to parse and manipulate
 existing Result XML files, or create new JUnit/xUnit result XMLs from scratch.
 
-:copyright: (c) 2019 by Joel Wang.
-:license: Apache2, see LICENSE for more details.
+Reference schema: https://github.com/windyroad/JUnit-Schema/blob/master/JUnit.xsd
+This according to the document is Apache Ant's JUnit output.
+
+See documentation for other supported schemas.
 """
 
 import itertools
 from copy import deepcopy
 
 try:
     from lxml import etree
@@ -53,22 +55,22 @@
 
     By default they are all string values. To support different value types,
     inherit this class and define your own methods.
 
     Also see: :class:`InitAttr`, :class:`FloatAttr`.
     """
 
-    def __init__(self, name=None):
+    def __init__(self, name: str = None):
         self.name = name
 
     def __get__(self, instance, cls):
         """Gets value from attribute, return None if attribute doesn't exist."""
         return instance._elem.attrib.get(self.name)
 
-    def __set__(self, instance, value):
+    def __set__(self, instance, value: str):
         """Sets XML element attribute."""
         if value is not None:
             instance._elem.attrib[self.name] = str(value)
 
 
 class IntAttr(Attr):
     """An integer attribute for an XML element.
@@ -80,15 +82,15 @@
     def __get__(self, instance, cls):
         result = super().__get__(instance, cls)
         if result is None and isinstance(instance, (JUnitXml, TestSuite)):
             instance.update_statistics()
             result = super().__get__(instance, cls)
         return int(result) if result else None
 
-    def __set__(self, instance, value):
+    def __set__(self, instance, value: int):
         if not isinstance(value, int):
             raise TypeError("Expected integer value.")
         super().__set__(instance, value)
 
 
 class FloatAttr(Attr):
     """A float attribute for an XML element.
@@ -100,15 +102,15 @@
     def __get__(self, instance, cls):
         result = super().__get__(instance, cls)
         if result is None and isinstance(instance, (JUnitXml, TestSuite)):
             instance.update_statistics()
             result = super().__get__(instance, cls)
         return float(result.replace(",", "")) if result else None
 
-    def __set__(self, instance, value):
+    def __set__(self, instance, value: float):
         if not (isinstance(value, float) or isinstance(value, int)):
             raise TypeError("Expected float value.")
         super().__set__(instance, value)
 
 
 def attributed(cls):
     """Decorator to read XML element attribute name from class attribute."""
@@ -126,15 +128,15 @@
         cls = attributed(cls)
         return cls
 
 
 class Element(metaclass=junitxml):
     """Base class for all Junit XML elements."""
 
-    def __init__(self, name=None):
+    def __init__(self, name: str = None):
         if not name:
             name = self._tag
         self._elem = etree.Element(name)
 
     def __hash__(self):
         return hash(etree.tostring(self._elem))
 
@@ -158,15 +160,15 @@
     def extend(self, sub_elems):
         """Adds elements subelement to the end of this elements internal
         list of subelements.
         """
         self._elem.extend((sub_elem._elem for sub_elem in sub_elems))
 
     @classmethod
-    def fromstring(cls, text):
+    def fromstring(cls, text: str):
         """Construct Junit objects from a XML string."""
         instance = cls()
         instance._elem = etree.fromstring(text)  # nosec
         return instance
 
     @classmethod
     def fromelem(cls, elem):
@@ -199,131 +201,277 @@
                 self._elem.remove(child._elem)
 
     def tostring(self):
         """Converts element to XML string."""
         return etree.tostring(self._elem, encoding="utf-8")
 
 
-class JUnitXml(Element):
-    """The JUnitXml root object.
+class Result(Element):
+    """Base class for test result.
 
-    It may contains a :class:`TestSuites` or a :class:`TestSuite`.
+    Attributes:
+        message: result as message string
+        type: message type
+    """
+
+    _tag = None
+    message = Attr()
+    type = Attr()
+
+    def __init__(self, message: str = None, type_: str = None):
+        super(Result, self).__init__(self._tag)
+        if message:
+            self.message = message
+        if type_:
+            self.type = type_
+
+    def __eq__(self, other):
+        return (
+            self._tag == other._tag
+            and self.type == other.type
+            and self.message == other.message
+        )
+
+    @property
+    def text(self):
+        return self._elem.text
+
+    @text.setter
+    def text(self, value: str):
+        self._elem.text = value
+
+
+class Skipped(Result):
+    """Test result when the case is skipped."""
+
+    _tag = "skipped"
+
+    def __eq__(self, other):
+        return super().__eq__(other)
+
+
+class Failure(Result):
+    """Test result when the case failed."""
+
+    _tag = "failure"
+
+    def __eq__(self, other):
+        return super().__eq__(other)
+
+
+class Error(Result):
+    """Test result when the case has errors during execution."""
+
+    _tag = "error"
+
+    def __eq__(self, other):
+        return super().__eq__(other)
+
+
+POSSIBLE_RESULTS = {Failure, Error, Skipped}
+
+
+class System(Element):
+    """Parent class for SystemOut and SystemErr.
 
     Attributes:
-        name: test suite name if it only contains one test suite
-        time: time consumed by the test suites
-        tests: total number of tests
-        failures: number of failed cases
-        errors: number of cases with errors
-        skipped: number of skipped cases
+        text: the output message
     """
 
-    _tag = "testsuites"
+    _tag = ""
+
+    def __init__(self, content: str = None):
+        super().__init__(self._tag)
+        self.text = content
+
+    @property
+    def text(self):
+        return self._elem.text
+
+    @text.setter
+    def text(self, value: str):
+        self._elem.text = value
+
+
+class SystemOut(System):
+    _tag = "system-out"
+
+
+class SystemErr(System):
+    _tag = "system-err"
+
+
+class TestCase(Element):
+    """Object to store a testcase and its result.
+
+    Attributes:
+        name: case name
+        classname: the parent class of the case
+        time: how much time is consumed by the test
+
+    Properties:
+        result: Failure, Skipped, or Error
+        system_out: stdout
+        system_err: stderr
+    """
+
+    _tag = "testcase"
     name = Attr()
+    classname = Attr()
     time = FloatAttr()
-    tests = IntAttr()
-    failures = IntAttr()
-    errors = IntAttr()
-    skipped = IntAttr()
 
-    def __init__(self, name=None):
+    def __init__(self, name: str = None, classname: str = None, time: float = None):
         super().__init__(self._tag)
-        self.filepath = None
-        self.name = name
+        if name is not None:
+            self.name = name
+        if classname is not None:
+            self.classname = classname
+        if time is not None:
+            self.time = float(time)
+
+    def __hash__(self):
+        return super().__hash__()
 
     def __iter__(self):
-        return super().iterchildren(TestSuite)
+        all_types = set.union(POSSIBLE_RESULTS, {SystemOut}, {SystemErr})
+        for elem in self._elem.iter():
+            for entry_type in all_types:
+                if elem.tag == entry_type._tag:
+                    yield entry_type.fromelem(elem)
 
-    def __len__(self):
-        return len(list(self.__iter__()))
+    def __eq__(self, other):
+        # TODO: May not work correctly if unreliable hash method is used.
+        return hash(self) == hash(other)
 
-    def __add__(self, other):
-        result = JUnitXml()
-        for suite in self:
-            result.add_testsuite(suite)
-        for suite in other:
-            result.add_testsuite(suite)
-        return result
+    @property
+    def is_passed(self):
+        """Whether this testcase was a success (i.e. if it isn't skipped, failed, or errored)."""
+        return not self.result
 
-    def __iadd__(self, other):
-        if other._elem.tag == "testsuites":
-            for suite in other:
-                self.add_testsuite(suite)
-        elif other._elem.tag == "testsuite":
-            suite = TestSuite(name=other.name)
-            for case in other:
-                suite._add_testcase_no_update_stats(case)
-            self.add_testsuite(suite)
-            self.update_statistics()
+    @property
+    def is_skipped(self):
+        """Whether this testcase was skipped."""
+        for r in self.result:
+            if isinstance(r, Skipped):
+                return True
+        return False
 
-        return self
+    @property
+    def result(self):
+        """A list of Failure, Skipped, or Error objects."""
+        results = []
+        for entry in self:
+            if isinstance(entry, tuple(POSSIBLE_RESULTS)):
+                results.append(entry)
 
-    def add_testsuite(self, suite):
-        """Add a test suite."""
-        for existing_suite in self:
-            if existing_suite == suite:
-                for case in suite:
-                    existing_suite._add_testcase_no_update_stats(case)
-                return
-        self.append(suite)
+        return results
 
-    def update_statistics(self):
-        """Update test count, time, etc."""
-        time = 0
-        tests = failures = errors = skipped = 0
-        for suite in self:
-            suite.update_statistics()
-            tests += suite.tests
-            failures += suite.failures
-            errors += suite.errors
-            skipped += suite.skipped
-            time += suite.time
-        self.tests = tests
-        self.failures = failures
-        self.errors = errors
-        self.skipped = skipped
-        self.time = round(time, 3)
+    @result.setter
+    def result(self, value: Result):
+        # First remove all existing results
+        for entry in self.result:
+            if any(isinstance(entry, r) for r in POSSIBLE_RESULTS):
+                self.remove(entry)
+        for entry in value:
+            if any(isinstance(entry, r) for r in POSSIBLE_RESULTS):
+                self.append(entry)
 
-    @classmethod
-    def fromroot(cls, root_elem):
-        """Constructs Junit objects from an elementTree root element."""
-        if root_elem.tag == "testsuites":
-            instance = cls()
-        elif root_elem.tag == "testsuite":
-            instance = TestSuite()
+    @property
+    def system_out(self):
+        """stdout."""
+        elem = self.child(SystemOut)
+        if elem is not None:
+            return elem.text
+        return None
+
+    @system_out.setter
+    def system_out(self, value: str):
+        out = self.child(SystemOut)
+        if out is not None:
+            out.text = value
         else:
-            raise JUnitXmlError("Invalid format.")
-        instance._elem = root_elem
-        return instance
+            out = SystemOut(value)
+            self.append(out)
 
-    @classmethod
-    def fromstring(cls, text):
-        """Construct Junit objects from a XML string."""
-        root_elem = etree.fromstring(text)  # nosec
-        return cls.fromroot(root_elem)
+    @property
+    def system_err(self):
+        """stderr."""
+        elem = self.child(SystemErr)
+        if elem is not None:
+            return elem.text
+        return None
 
-    @classmethod
-    def fromfile(cls, filepath, parse_func=None):
-        """Initiate the object from a report file."""
-        if parse_func:
-            tree = parse_func(filepath)
+    @system_err.setter
+    def system_err(self, value: str):
+        err = self.child(SystemErr)
+        if err is not None:
+            err.text = value
         else:
-            tree = etree.parse(filepath)  # nosec
-        root_elem = tree.getroot()
-        instance = cls.fromroot(root_elem)
-        instance.filepath = filepath
-        return instance
+            err = SystemErr(value)
+            self.append(err)
 
-    def write(self, filepath=None, pretty=False, to_console=False):
-        """Write the object into a junit xml file.
 
-        If `file_path` is not specified, it will write to the original file.
-        If `pretty` is True, the result file will be more human friendly.
-        """
-        write_xml(self, filepath=filepath, pretty=pretty, to_console=to_console)
+class Property(Element):
+    """A key/value pare that's stored in the test suite.
+
+    Use it to store anything you find interesting or useful.
+
+    Attributes:
+        name: the property name
+        value: the property value
+    """
+
+    _tag = "property"
+    name = Attr()
+    value = Attr()
+
+    def __init__(self, name: str = None, value: str = None):
+        super().__init__(self._tag)
+        self.name = name
+        self.value = value
+
+    def __eq__(self, other):
+        return self.name == other.name and self.value == other.value
+
+    def __ne__(self, other):
+        return not self == other
+
+    def __lt__(self, other):
+        """Supports sort() for properties."""
+        return self.name > other.name
+
+
+class Properties(Element):
+    """A list of properties inside a test suite.
+
+    See :class:`Property`
+    """
+
+    _tag = "properties"
+
+    def __init__(self):
+        super().__init__(self._tag)
+
+    def add_property(self, property_: Property):
+        self.append(property_)
+
+    def __iter__(self):
+        return super().iterchildren(Property)
+
+    def __eq__(self, other):
+        p1 = list(self)
+        p2 = list(other)
+        p1.sort()
+        p2.sort()
+        if len(p1) != len(p2):
+            return False
+        for e1, e2 in zip(p1, p2):
+            if e1 != e2:
+                return False
+        return True
 
 
 class TestSuite(Element):
     """The <testsuite> object.
 
     Attributes:
         name: test suite name
@@ -350,19 +498,15 @@
         super().__init__(self._tag)
         self.name = name
         self.filepath = None
 
     def __iter__(self):
         return itertools.chain(
             super().iterchildren(TestCase),
-            (
-                case
-                for suite in super().iterchildren(TestSuite)
-                for case in suite
-            ),
+            (case for suite in super().iterchildren(TestSuite) for case in suite),
         )
 
     def __len__(self):
         return len(list(self.__iter__()))
 
     def __eq__(self, other):
         def props_eq(props1, props2):
@@ -408,15 +552,15 @@
 
         result = JUnitXml()
         result.filepath = self.filepath
         result.add_testsuite(self)
         result.add_testsuite(other)
         return result
 
-    def remove_testcase(self, testcase):
+    def remove_testcase(self, testcase: TestCase):
         """Removes a test case from the suite."""
         for case in self:
             if case == testcase:
                 super().remove(case)
                 self.update_statistics()
 
     def update_statistics(self):
@@ -478,288 +622,142 @@
         """Iterates through all properties."""
         props = self.child(Properties)
         if props is None:
             return
         for prop in props:
             yield prop
 
-    def remove_property(self, property_):
+    def remove_property(self, property_: Property):
         """Removes a property."""
         props = self.child(Properties)
         if props is None:
             return
         for prop in props:
             if prop == property_:
                 props.remove(property_)
 
     def testsuites(self):
         """Iterates through all testsuites."""
         for suite in self.iterchildren(TestSuite):
             yield suite
 
-    def write(self, filepath=None, pretty=False):
+    def write(self, filepath: str = None, pretty=False):
         write_xml(self, filepath=filepath, pretty=pretty)
 
 
-class Properties(Element):
-    """A list of properties inside a test suite.
-
-    See :class:`Property`
-    """
-
-    _tag = "properties"
-
-    def __init__(self):
-        super().__init__(self._tag)
-
-    def add_property(self, property_):
-        self.append(property_)
-
-    def __iter__(self):
-        return super().iterchildren(Property)
-
-    def __eq__(self, other):
-        p1 = list(self)
-        p2 = list(other)
-        p1.sort()
-        p2.sort()
-        if len(p1) != len(p2):
-            return False
-        for e1, e2 in zip(p1, p2):
-            if e1 != e2:
-                return False
-        return True
-
-
-class Property(Element):
-    """A key/value pare that's stored in the test suite.
-
-    Use it to store anything you find interesting or useful.
-
-    Attributes:
-        name: the property name
-        value: the property value
-    """
-
-    _tag = "property"
-    name = Attr()
-    value = Attr()
-
-    def __init__(self, name=None, value=None):
-        super().__init__(self._tag)
-        self.name = name
-        self.value = value
-
-    def __eq__(self, other):
-        return self.name == other.name and self.value == other.value
-
-    def __ne__(self, other):
-        return not self == other
-
-    def __lt__(self, other):
-        """Supports sort() for properties."""
-        return self.name > other.name
-
-
-class Result(Element):
-    """Base class for test result.
-
-    Attributes:
-        message: result as message string
-        type: message type
-    """
-
-    _tag = None
-    message = Attr()
-    type = Attr()
-
-    def __init__(self, message=None, type_=None):
-        super(Result, self).__init__(self._tag)
-        if message:
-            self.message = message
-        if type_:
-            self.type = type_
-
-    def __eq__(self, other):
-        return (
-            self._tag == other._tag
-            and self.type == other.type
-            and self.message == other.message
-        )
-
-    @property
-    def text(self):
-        return self._elem.text
-
-    @text.setter
-    def text(self, value):
-        self._elem.text = value
-
-
-class Skipped(Result):
-    """Test result when the case is skipped."""
-
-    _tag = "skipped"
-
-    def __eq__(self, other):
-        return super().__eq__(other)
-
-
-class Failure(Result):
-    """Test result when the case failed."""
-
-    _tag = "failure"
-
-    def __eq__(self, other):
-        return super().__eq__(other)
-
-
-class Error(Result):
-    """Test result when the case has errors during execution."""
-
-    _tag = "error"
-
-    def __eq__(self, other):
-        return super().__eq__(other)
-
-
-POSSIBLE_RESULTS = {Failure, Error, Skipped}
-
+class JUnitXml(Element):
+    """The JUnitXml root object.
 
-class TestCase(Element):
-    """Object to store a testcase and its result.
+    It may contains a :class:`TestSuites` or a :class:`TestSuite`.
 
     Attributes:
-        name: case name
-        classname: the parent class of the case
-        time: how much time is consumed by the test
-
-    Properties:
-        result: Failure, Skipped, or Error
-        system_out: stdout
-        system_err: stderr
+        name: test suite name if it only contains one test suite
+        time: time consumed by the test suites
+        tests: total number of tests
+        failures: number of failed cases
+        errors: number of cases with errors
+        skipped: number of skipped cases
     """
 
-    _tag = "testcase"
+    _tag = "testsuites"
     name = Attr()
-    classname = Attr()
     time = FloatAttr()
+    tests = IntAttr()
+    failures = IntAttr()
+    errors = IntAttr()
+    skipped = IntAttr()
 
-    def __init__(self, name=None, classname=None, time=None):
+    def __init__(self, name=None):
         super().__init__(self._tag)
-        if name is not None:
-            self.name = name
-        if classname is not None:
-            self.classname = classname
-        if time is not None:
-            self.time = float(time)
-
-    def __hash__(self):
-        return super().__hash__()
+        self.filepath = None
+        self.name = name
 
     def __iter__(self):
-        all_types = set.union(POSSIBLE_RESULTS, {SystemOut}, {SystemErr})
-        for elem in self._elem.iter():
-            for entry_type in all_types:
-                if elem.tag == entry_type._tag:
-                    yield entry_type.fromelem(elem)
-
-    def __eq__(self, other):
-        # TODO: May not work correctly if unreliable hash method is used.
-        return hash(self) == hash(other)
+        return super().iterchildren(TestSuite)
 
-    @property
-    def is_passed(self):
-        """Whether this testcase was a success (i.e. if it isn't skipped, failed, or errored)."""
-        return not self.result
+    def __len__(self):
+        return len(list(self.__iter__()))
 
-    @property
-    def is_skipped(self):
-        """Whether this testcase was skipped."""
-        for r in self.result:
-            if isinstance(r, Skipped):
-                return True
-        return False
+    def __add__(self, other):
+        result = JUnitXml()
+        for suite in self:
+            result.add_testsuite(suite)
+        for suite in other:
+            result.add_testsuite(suite)
+        return result
 
-    @property
-    def result(self):
-        """A list of Failure, Skipped, or Error objects."""
-        results = []
-        for entry in self:
-            if isinstance(entry, tuple(POSSIBLE_RESULTS)):
-                results.append(entry)
+    def __iadd__(self, other):
+        if other._elem.tag == "testsuites":
+            for suite in other:
+                self.add_testsuite(suite)
+        elif other._elem.tag == "testsuite":
+            suite = TestSuite(name=other.name)
+            for case in other:
+                suite._add_testcase_no_update_stats(case)
+            self.add_testsuite(suite)
+            self.update_statistics()
 
-        return results
+        return self
 
-    @result.setter
-    def result(self, value):
-        # First remove all existing results
-        for entry in self.result:
-            if any(isinstance(entry, r) for r in POSSIBLE_RESULTS):
-                self.remove(entry)
-        for entry in value:
-            if any(isinstance(entry, r) for r in POSSIBLE_RESULTS):
-                self.append(entry)
+    def add_testsuite(self, suite: TestSuite):
+        """Add a test suite."""
+        for existing_suite in self:
+            if existing_suite == suite:
+                for case in suite:
+                    existing_suite._add_testcase_no_update_stats(case)
+                return
+        self.append(suite)
 
-    @property
-    def system_out(self):
-        """stdout."""
-        elem = self.child(SystemOut)
-        if elem is not None:
-            return elem.text
-        return None
+    def update_statistics(self):
+        """Update test count, time, etc."""
+        time = 0
+        tests = failures = errors = skipped = 0
+        for suite in self:
+            suite.update_statistics()
+            tests += suite.tests
+            failures += suite.failures
+            errors += suite.errors
+            skipped += suite.skipped
+            time += suite.time
+        self.tests = tests
+        self.failures = failures
+        self.errors = errors
+        self.skipped = skipped
+        self.time = round(time, 3)
 
-    @system_out.setter
-    def system_out(self, value):
-        out = self.child(SystemOut)
-        if out is not None:
-            out.text = value
+    @classmethod
+    def fromroot(cls, root_elem: Element):
+        """Constructs Junit objects from an elementTree root element."""
+        if root_elem.tag == "testsuites":
+            instance = cls()
+        elif root_elem.tag == "testsuite":
+            instance = TestSuite()
         else:
-            out = SystemOut(value)
-            self.append(out)
+            raise JUnitXmlError("Invalid format.")
+        instance._elem = root_elem
+        return instance
 
-    @property
-    def system_err(self):
-        """stderr."""
-        elem = self.child(SystemErr)
-        if elem is not None:
-            return elem.text
-        return None
+    @classmethod
+    def fromstring(cls, text: str):
+        """Construct Junit objects from a XML string."""
+        root_elem = etree.fromstring(text)  # nosec
+        return cls.fromroot(root_elem)
 
-    @system_err.setter
-    def system_err(self, value):
-        err = self.child(SystemErr)
-        if err is not None:
-            err.text = value
+    @classmethod
+    def fromfile(cls, filepath: str, parse_func=None):
+        """Initiate the object from a report file."""
+        if parse_func:
+            tree = parse_func(filepath)
         else:
-            err = SystemErr(value)
-            self.append(err)
-
-
-class System(Element):
-    """Parent class for SystemOut and SystemErr.
-
-    Attributes:
-        text: the output message
-    """
-
-    _tag = ""
-
-    def __init__(self, content=None):
-        super().__init__(self._tag)
-        self.text = content
-
-    @property
-    def text(self):
-        return self._elem.text
-
-    @text.setter
-    def text(self, value):
-        self._elem.text = value
-
-
-class SystemOut(System):
-    _tag = "system-out"
+            tree = etree.parse(filepath)  # nosec
+        root_elem = tree.getroot()
+        instance = cls.fromroot(root_elem)
+        instance.filepath = filepath
+        return instance
 
+    def write(self, filepath: str = None, pretty=False, to_console=False):
+        """Write the object into a junit xml file.
 
-class SystemErr(System):
-    _tag = "system-err"
+        If `file_path` is not specified, it will write to the original file.
+        If `pretty` is True, the result file will be more human friendly.
+        """
+        write_xml(self, filepath=filepath, pretty=pretty, to_console=to_console)
```

### Comparing `junitparser-3.0.0/junitparser.egg-info/PKG-INFO` & `junitparser-3.1.0/junitparser.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junitparser
-Version: 3.0.0
+Version: 3.1.0
 Summary: Manipulates JUnit/xUnit Result XML files
 Home-page: https://github.com/weiwei/junitparser
 Author: Weiwei Wang
 Author-email: gastlygem@gmail.com
 License: Apache 2.0
 Keywords: junit xunit xml parser
 Classifier: Development Status :: 5 - Production/Stable
@@ -141,14 +141,47 @@
     newxml = xml1 + xml2
     # Alternatively, merge in place
     xml1 += xml2
 
 Note that it won't check for duplicate entries. You need to deal with them on
 your own.
 
+Schema Support
+~~~~~~~~~~~~~~~
+
+By default junitparser supports the schema of windyroad_, which is a relatively
+simple schema. 
+
+.. _windyroad: https://github.com/windyroad/JUnit-Schema/blob/master/JUnit.xsd
+
+Junitparser also support extra schemas:
+
+.. code-block:: python
+
+    from junitparser.xunit2 import JUnitParser, TestCase, TestSuite, \
+        RerunFailure
+    # These classes are redefined to support extra properties and attributes
+    # of the xunit2 schema.
+    suite = TestSuite("mySuite")
+    suite.system_err = "System err" # xunit2 specific property
+    case = TestCase("myCase")
+    rerun_failure = RerunFailure("Not found", "404") # case property
+    rerun_failure.stack_trace = "Stack"
+    rerun_failure.system_err = "E404"
+    rerun_failure.system_out = "NOT FOUND"
+    case.add_rerun_result(rerun_failure)
+
+Currently supported schemas including:
+
+- xunit2_, supported by pytest, Erlang/OTP, Maven Surefire, CppTest, etc.
+
+.. _xunit2: https://github.com/jenkinsci/xunit-plugin/blob/xunit-2.3.2/src/main/resources/org/jenkinsci/plugins/xunit/types/model/xsd/junit-10.xsd
+
+PRs are welcome to support more schemas.
+
 Create XML with custom attributes
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You want to use an attribute that is not supported by default.
 
 .. code-block:: python
```

### Comparing `junitparser-3.0.0/setup.py` & `junitparser-3.1.0/setup.py`

 * *Files identical despite different names*

