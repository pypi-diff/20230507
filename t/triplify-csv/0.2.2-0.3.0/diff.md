# Comparing `tmp/triplify_csv-0.2.2.tar.gz` & `tmp/triplify_csv-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triplify_csv-0.2.2.tar", max compression
+gzip compressed data, was "triplify_csv-0.3.0.tar", max compression
```

## Comparing `triplify_csv-0.2.2.tar` & `triplify_csv-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1526 2023-04-03 19:59:17.539697 triplify_csv-0.2.2/LICENSE
--rw-r--r--   0        0        0     7042 2023-04-03 19:59:17.539697 triplify_csv-0.2.2/README.md
--rw-r--r--   0        0        0      568 2023-04-21 08:39:08.590347 triplify_csv-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-03 19:59:17.546697 triplify_csv-0.2.2/triplify_csv/__init__.py
--rwxr-xr-x   0        0        0    17486 2023-04-21 08:17:19.466388 triplify_csv-0.2.2/triplify_csv/triplify_csv.py
--rw-r--r--   0        0        0     7839 1970-01-01 00:00:00.000000 triplify_csv-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-04-03 19:59:17.539697 triplify_csv-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7467 2023-05-07 09:13:43.889593 triplify_csv-0.3.0/README.md
+-rw-r--r--   0        0        0      568 2023-05-07 09:36:22.549551 triplify_csv-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-03 19:59:17.546697 triplify_csv-0.3.0/triplify_csv/__init__.py
+-rwxr-xr-x   0        0        0    17765 2023-04-30 07:29:04.624548 triplify_csv-0.3.0/triplify_csv/triplify_csv.py
+-rw-r--r--   0        0        0     8264 1970-01-01 00:00:00.000000 triplify_csv-0.3.0/PKG-INFO
```

### Comparing `triplify_csv-0.2.2/LICENSE` & `triplify_csv-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `triplify_csv-0.2.2/README.md` & `triplify_csv-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 **How to make your configuration file**
 
 The configuration file contains a set of mappings for triplify\_csv to follow to set the subjects, predicates and objects or literal values of your triples or nquads from the data in one or more CSV files. These mappings are RDF triples in the turtle syntax. The terms that can be used are a subset of the terms defined in the R2RML standard.
 
 R2RML was not designed for this purpose. R2RML is '.. a language for expressing customized mappings from relational databases to RDF datasets.' (see [https://www.w3.org/TR/r2rml/](https://www.w3.org/TR/r2rml/) ). Triplify\_csv uses a subset of R2RML to express customised mappings from CSV files to RDF datasets. Where R2RML refers to the tables of a database using 'rr:logicalTable' this should be understood in the triplify\_csv use of R2RML as referring to the name (without '.csv') of a corresponding csv file. 'rr:sqlQuery', the term of the R2RML language that lets you express mappings from database queries to RDF isn't supported in the triplify\_csv usage. Also, there is no need to support 'rr:sqlVersion'.
 
-For a complete list of what parts of the R2RML language are supported see the examples in the /tests folder and refer to the R2RML test cases document ([https://www.w3.org/TR/rdb2rdf-test-cases/](https://www.w3.org/TR/rdb2rdf-test-cases/)). As of version 0.2.0 the test cases supported are
+For a complete list of what parts of the R2RML language are supported see the examples in the /tests folder and refer to the R2RML test cases document ([https://www.w3.org/TR/rdb2rdf-test-cases/](https://www.w3.org/TR/rdb2rdf-test-cases/)). As of version 0.3.0 the test cases supported are
 
 - R2RMLTC0007a - Typing resources by relying on rdf:type predicate
 - R2RMLTC0007b - Assigning triples to Named Graphs
 - R2RMLTC0007c - One column mapping, using rr:class
 - R2RMLTC0007d - One column mapping, specifying an rr:predicateObjectMap with rdf:type
 - R2RMLTC0007e - One column mapping, using rr:graphMap and rr:class
 - R2RMLTC0007f - One column mapping, using rr:graphMap and specifying an rr:predicateObjectMap with rdf:type
@@ -85,14 +85,16 @@
 - R2RMLTC0007h - Assigning triples to a non-IRI named graph
 - R2RMLTC0008a - Generation of triples to a target graph by using rr:graphMap and rr:template
 - R2RMLTC0008b - Generation of triples referencing object map
 - R2RMLTC0008c - Generation of triples by using multiple predicateMaps within a rr:predicateObjectMap
 - R2RMLTC0009a - Generation of triples from foreign key relations
 - R2RMLTC0015a - Generation of language tags for plain literals from a CSV 'table' with language information
 	- note: this test uses a separate CSV file for each language and differs from the original test case (in the [rdf-test-cases page](https://www.w3.org/TR/rdb2rdf-test-cases/)) which uses 'rr:sqlQuery' to select tags in each language from a single table.
+- R2RMLTC0016a to R2RMLTC0016d, setting data types as in these tests for string, integer, real, float, date, timestamp and boolean.  
+	- note: instead of deriving the data type from the sql column, as the subset of r2rml used here does not refer to a database the user must use 'explicitly typed literals' as in section [7.6 Typed Literals](https://www.w3.org/TR/r2rml/#typed-literals) (rr:datatype) of the r2rml standard.
 
 Copyright © 2015 W3C® (MIT, ERCIM, Keio, Beihang). This software or document includes material copied from or derived from 'R2RML: RDB to RDF Mapping Language' [http://www.w3.org/TR/2012/REC-r2rml-20120927/](http://www.w3.org/TR/2012/REC-r2rml-20120927/) and 'R2RML and Direct Mapping Test Cases' [http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/](http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/)
 
 **Simple config file example** Suppose you have a CSV file containing details of contacts (example CSV below) and you want to generate RDF data from this using FOAF, the R2RML config file might look like this ...
 
 	@prefix rr: <http://www.w3.org/ns/r2rml#> .
 	@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@@ -157,8 +159,8 @@
 	    foaf:name "Joe Bloggs" .
 	
 	<http://example.com/Contact/30/Mr%20Bun> a foaf:Person ;
 	    ex:id 30 ;
 	    foaf:interest "https://en.m.wikipedia.org/wiki/Spam\_(food)" ;
 	    foaf:name "Mr Bun" .
 
-
+
```

### Comparing `triplify_csv-0.2.2/pyproject.toml` & `triplify_csv-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "triplify_csv"
-version = "0.2.2"
+version = "0.3.0"
 description = "A tool to generate triples from CSV files according to a configuration file."
 authors = ["Adrian Atley"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/AAtley/triplify_csv"
 
 [tool.poetry.dependencies]
```

### Comparing `triplify_csv-0.2.2/triplify_csv/triplify_csv.py` & `triplify_csv-0.3.0/triplify_csv/triplify_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,20 +350,26 @@
 						predicates = str(pom[rr('predicate')]).split(',')
 						for pred_str in predicates:
 							predicate = URIRef(pred_str)
 						
 							pom_column = ''
 							pom_object = ''
 							literal_lang = ''
+							lit_datatype = ''
 							if rr('object') in pom:
 								pom_object = pom[rr('object')]
 							if rr('objectMap') in pom and rr('column') in pom[rr('objectMap')]:
 								pom_column = pom[rr('objectMap')][rr('column')]
 								if rr('language') in pom[rr('objectMap')]:
 									literal_lang = pom[rr('objectMap')][rr('language')]
+								else:
+									if rr('datatype') in pom[rr('objectMap')]:
+										lit_datatype = pom[rr('objectMap')][rr('datatype')]
+										
+										
 								
 							# if objectmap in pom and key of this om is also in tmap then it is a refobjmap
 							if rr('objectMap') in pom and str(pom[rr('objectMap')]) in tmaps.keys() and rr('parentTriplesMap') in tmaps[str(pom[rr('objectMap')])] and tmaps[str(pom[rr('objectMap')])][rr('parentTriplesMap')] in tmaps.keys():
 								rom = pom[rr('objectMap')]
 								
 								ptm = tmaps[rom][rr('parentTriplesMap')]
 								ptmSubjectTemplate = tmaps[ptm][rr('subjectMap')][rr('template')]
@@ -400,15 +406,15 @@
 											# get uri from fk csv's template and fk row
 											ptmSubjectTemplate = tmaps[ptm][rr('subjectMap')][rr('template')]
 											
 											object = URIRef(self.get_Uri_From_Template(ptmSubjectTemplate,record))
 							
 							elif len(pom_column) > 0 and pom_column in row.keys():
 								
-								object = self.get_literal(row[pom_column],csvinfo.options.dateformat, literal_lang)
+								object = self.get_literal(row[pom_column],csvinfo.options.dateformat, literal_lang, lit_datatype)
 							else:
 								object = URIRef(pom_object)
 	
 							# add to Dataset for quads if non-default graph else add just add triple
 							if making_quads:
 								gc = self.triples.graph(URIRef(context))
 								self.triples.add((subject, predicate, object, gc))
@@ -422,16 +428,19 @@
 		for n in self.g.namespace_manager.namespaces():
 			self.triples.namespace_manager.bind(n[0],n[1])
 		self.triples.namespace_manager.bind('rdf', RDF)	
 	
 		# close any open input files
 		self.close_csvs()
 	
-	def get_literal(self, value, dateformat='%Y-%m-%d', lang=''):
+	def get_literal(self, value, dateformat='%Y-%m-%d', lang='', lit_datatype=''):
 		
+		if lit_datatype:
+			return Literal(value, datatype = lit_datatype)
+			
 		try:
 			dt = datetime.strptime(value,dateformat).date()
 			return Literal(dt, datatype=XSD.date)
 		except ValueError:
 			pass
 		try: 
 			i = int(value)
```

### Comparing `triplify_csv-0.2.2/PKG-INFO` & `triplify_csv-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplify-csv
-Version: 0.2.2
+Version: 0.3.0
 Summary: A tool to generate triples from CSV files according to a configuration file.
 Home-page: https://github.com/AAtley/triplify_csv
 License: BSD-3-Clause
 Author: Adrian Atley
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -89,15 +89,15 @@
 
 **How to make your configuration file**
 
 The configuration file contains a set of mappings for triplify\_csv to follow to set the subjects, predicates and objects or literal values of your triples or nquads from the data in one or more CSV files. These mappings are RDF triples in the turtle syntax. The terms that can be used are a subset of the terms defined in the R2RML standard.
 
 R2RML was not designed for this purpose. R2RML is '.. a language for expressing customized mappings from relational databases to RDF datasets.' (see [https://www.w3.org/TR/r2rml/](https://www.w3.org/TR/r2rml/) ). Triplify\_csv uses a subset of R2RML to express customised mappings from CSV files to RDF datasets. Where R2RML refers to the tables of a database using 'rr:logicalTable' this should be understood in the triplify\_csv use of R2RML as referring to the name (without '.csv') of a corresponding csv file. 'rr:sqlQuery', the term of the R2RML language that lets you express mappings from database queries to RDF isn't supported in the triplify\_csv usage. Also, there is no need to support 'rr:sqlVersion'.
 
-For a complete list of what parts of the R2RML language are supported see the examples in the /tests folder and refer to the R2RML test cases document ([https://www.w3.org/TR/rdb2rdf-test-cases/](https://www.w3.org/TR/rdb2rdf-test-cases/)). As of version 0.2.0 the test cases supported are
+For a complete list of what parts of the R2RML language are supported see the examples in the /tests folder and refer to the R2RML test cases document ([https://www.w3.org/TR/rdb2rdf-test-cases/](https://www.w3.org/TR/rdb2rdf-test-cases/)). As of version 0.3.0 the test cases supported are
 
 - R2RMLTC0007a - Typing resources by relying on rdf:type predicate
 - R2RMLTC0007b - Assigning triples to Named Graphs
 - R2RMLTC0007c - One column mapping, using rr:class
 - R2RMLTC0007d - One column mapping, specifying an rr:predicateObjectMap with rdf:type
 - R2RMLTC0007e - One column mapping, using rr:graphMap and rr:class
 - R2RMLTC0007f - One column mapping, using rr:graphMap and specifying an rr:predicateObjectMap with rdf:type
@@ -105,14 +105,16 @@
 - R2RMLTC0007h - Assigning triples to a non-IRI named graph
 - R2RMLTC0008a - Generation of triples to a target graph by using rr:graphMap and rr:template
 - R2RMLTC0008b - Generation of triples referencing object map
 - R2RMLTC0008c - Generation of triples by using multiple predicateMaps within a rr:predicateObjectMap
 - R2RMLTC0009a - Generation of triples from foreign key relations
 - R2RMLTC0015a - Generation of language tags for plain literals from a CSV 'table' with language information
 	- note: this test uses a separate CSV file for each language and differs from the original test case (in the [rdf-test-cases page](https://www.w3.org/TR/rdb2rdf-test-cases/)) which uses 'rr:sqlQuery' to select tags in each language from a single table.
+- R2RMLTC0016a to R2RMLTC0016d, setting data types as in these tests for string, integer, real, float, date, timestamp and boolean.  
+	- note: instead of deriving the data type from the sql column, as the subset of r2rml used here does not refer to a database the user must use 'explicitly typed literals' as in section [7.6 Typed Literals](https://www.w3.org/TR/r2rml/#typed-literals) (rr:datatype) of the r2rml standard.
 
 Copyright © 2015 W3C® (MIT, ERCIM, Keio, Beihang). This software or document includes material copied from or derived from 'R2RML: RDB to RDF Mapping Language' [http://www.w3.org/TR/2012/REC-r2rml-20120927/](http://www.w3.org/TR/2012/REC-r2rml-20120927/) and 'R2RML and Direct Mapping Test Cases' [http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/](http://www.w3.org/TR/2012/NOTE-rdb2rdf-test-cases-20120814/)
 
 **Simple config file example** Suppose you have a CSV file containing details of contacts (example CSV below) and you want to generate RDF data from this using FOAF, the R2RML config file might look like this ...
 
 	@prefix rr: <http://www.w3.org/ns/r2rml#> .
 	@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@@ -177,9 +179,8 @@
 	    foaf:name "Joe Bloggs" .
 	
 	<http://example.com/Contact/30/Mr%20Bun> a foaf:Person ;
 	    ex:id 30 ;
 	    foaf:interest "https://en.m.wikipedia.org/wiki/Spam\_(food)" ;
 	    foaf:name "Mr Bun" .
 
-
-
+
```

