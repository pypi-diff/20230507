# Comparing `tmp/tumfl-0.1.0.tar.gz` & `tmp/tumfl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumfl-0.1.0.tar", last modified: Sun May  7 15:24:51 2023, max compression
+gzip compressed data, was "tumfl-0.1.1.tar", last modified: Sun May  7 15:26:03 2023, max compression
```

## Comparing `tumfl-0.1.0.tar` & `tumfl-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:24:51.138810 tumfl-0.1.0/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1214 2023-05-07 15:24:51.137810 tumfl-0.1.0/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      429 2022-08-10 22:55:26.000000 tumfl-0.1.0/README.md
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1083 2023-05-07 15:19:49.000000 tumfl-0.1.0/pyproject.toml
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       38 2023-05-07 15:24:51.138810 tumfl-0.1.0/setup.cfg
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:24:51.129810 tumfl-0.1.0/test/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    12038 2023-05-07 15:10:00.000000 tumfl-0.1.0/test/test_lexer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    34797 2023-05-07 15:13:56.000000 tumfl-0.1.0/test/test_parser.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:24:51.130810 tumfl-0.1.0/tumfl/
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:24:51.131810 tumfl-0.1.0/tumfl/AST/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-05-07 06:49:52.000000 tumfl-0.1.0/tumfl/AST/ASTNode.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      667 2023-05-07 07:41:59.000000 tumfl-0.1.0/tumfl/AST/BaseFunctionDefinition.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:24:51.134810 tumfl-0.1.0/tumfl/AST/Expression/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1163 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/BinOp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      507 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/Boolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      513 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/ExpFunctionCall.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      820 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/ExpFunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      638 2023-05-07 06:48:48.000000 tumfl-0.1.0/tumfl/AST/Expression/ExpMethodInvocation.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      134 2023-02-03 20:08:43.000000 tumfl-0.1.0/tumfl/AST/Expression/Expression.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      414 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/Index.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      533 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/Name.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      437 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/NamedIndex.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      377 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/Nil.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2088 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/Number.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      531 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/String.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      384 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/Table.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1086 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/TableField.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      705 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/UnOp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      408 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/Vararg.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      180 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Expression/Variable.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      650 2023-05-07 15:14:20.000000 tumfl-0.1.0/tumfl/AST/Expression/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:24:51.137810 tumfl-0.1.0/tumfl/AST/Statement/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      530 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/Assign.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      513 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/Block.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      261 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/Break.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      100 2023-05-04 07:15:57.000000 tumfl-0.1.0/tumfl/AST/Statement/Chunk.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      548 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/FunctionCall.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1134 2023-05-07 11:58:15.000000 tumfl-0.1.0/tumfl/AST/Statement/FunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      348 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/Goto.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      623 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/If.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      649 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/IterativeFor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      360 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/Label.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1135 2023-05-07 11:44:32.000000 tumfl-0.1.0/tumfl/AST/Statement/LocalAssign.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      988 2023-05-07 11:50:43.000000 tumfl-0.1.0/tumfl/AST/Statement/LocalFunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      693 2023-05-07 06:48:41.000000 tumfl-0.1.0/tumfl/AST/Statement/MethodInvocation.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      791 2023-05-07 06:48:26.000000 tumfl-0.1.0/tumfl/AST/Statement/NumericFor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      450 2023-05-07 06:47:23.000000 tumfl-0.1.0/tumfl/AST/Statement/Repeat.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      247 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/Semicolon.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      356 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/Statement.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      437 2023-05-07 06:47:23.000000 tumfl-0.1.0/tumfl/AST/Statement/While.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/Statement/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       80 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/AST/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2116 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/Token.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      120 2023-05-07 15:21:36.000000 tumfl-0.1.0/tumfl/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      605 2023-05-07 08:21:02.000000 tumfl-0.1.0/tumfl/error.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    14372 2023-05-07 15:13:11.000000 tumfl-0.1.0/tumfl/lexer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    32511 2023-05-07 15:01:48.000000 tumfl-0.1.0/tumfl/parser.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1243 2023-05-07 06:47:22.000000 tumfl-0.1.0/tumfl/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:24:51.131810 tumfl-0.1.0/tumfl.egg-info/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1214 2023-05-07 15:24:51.000000 tumfl-0.1.0/tumfl.egg-info/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1609 2023-05-07 15:24:51.000000 tumfl-0.1.0/tumfl.egg-info/SOURCES.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-07 15:24:51.000000 tumfl-0.1.0/tumfl.egg-info/dependency_links.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       57 2023-05-07 15:24:51.000000 tumfl-0.1.0/tumfl.egg-info/requires.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        6 2023-05-07 15:24:51.000000 tumfl-0.1.0/tumfl.egg-info/top_level.txt
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.195799 tumfl-0.1.1/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1206 2023-05-07 15:26:03.195799 tumfl-0.1.1/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      429 2022-08-10 22:55:26.000000 tumfl-0.1.1/README.md
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1075 2023-05-07 15:25:47.000000 tumfl-0.1.1/pyproject.toml
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       38 2023-05-07 15:26:03.195799 tumfl-0.1.1/setup.cfg
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.189799 tumfl-0.1.1/test/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    12038 2023-05-07 15:10:00.000000 tumfl-0.1.1/test/test_lexer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    34797 2023-05-07 15:13:56.000000 tumfl-0.1.1/test/test_parser.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.190799 tumfl-0.1.1/tumfl/
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.190799 tumfl-0.1.1/tumfl/AST/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-05-07 06:49:52.000000 tumfl-0.1.1/tumfl/AST/ASTNode.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      667 2023-05-07 07:41:59.000000 tumfl-0.1.1/tumfl/AST/BaseFunctionDefinition.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.192799 tumfl-0.1.1/tumfl/AST/Expression/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1163 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/BinOp.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      507 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Boolean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      513 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/ExpFunctionCall.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      820 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/ExpFunctionDefinition.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      638 2023-05-07 06:48:48.000000 tumfl-0.1.1/tumfl/AST/Expression/ExpMethodInvocation.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      134 2023-02-03 20:08:43.000000 tumfl-0.1.1/tumfl/AST/Expression/Expression.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      414 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Index.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      533 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Name.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      437 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/NamedIndex.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      377 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Nil.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2088 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Number.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      531 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/String.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      384 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Table.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1086 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/TableField.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      705 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/UnOp.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      408 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Vararg.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      180 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Variable.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      650 2023-05-07 15:14:20.000000 tumfl-0.1.1/tumfl/AST/Expression/__init__.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.195799 tumfl-0.1.1/tumfl/AST/Statement/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      530 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Assign.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      513 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Block.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      261 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Break.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      100 2023-05-04 07:15:57.000000 tumfl-0.1.1/tumfl/AST/Statement/Chunk.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      548 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/FunctionCall.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1134 2023-05-07 11:58:15.000000 tumfl-0.1.1/tumfl/AST/Statement/FunctionDefinition.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      348 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Goto.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      623 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/If.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      649 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/IterativeFor.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      360 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Label.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1135 2023-05-07 11:44:32.000000 tumfl-0.1.1/tumfl/AST/Statement/LocalAssign.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      988 2023-05-07 11:50:43.000000 tumfl-0.1.1/tumfl/AST/Statement/LocalFunctionDefinition.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      693 2023-05-07 06:48:41.000000 tumfl-0.1.1/tumfl/AST/Statement/MethodInvocation.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      791 2023-05-07 06:48:26.000000 tumfl-0.1.1/tumfl/AST/Statement/NumericFor.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      450 2023-05-07 06:47:23.000000 tumfl-0.1.1/tumfl/AST/Statement/Repeat.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      247 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Semicolon.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      356 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Statement.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      437 2023-05-07 06:47:23.000000 tumfl-0.1.1/tumfl/AST/Statement/While.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       80 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2116 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/Token.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      120 2023-05-07 15:21:36.000000 tumfl-0.1.1/tumfl/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      605 2023-05-07 08:21:02.000000 tumfl-0.1.1/tumfl/error.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    14372 2023-05-07 15:13:11.000000 tumfl-0.1.1/tumfl/lexer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    32511 2023-05-07 15:01:48.000000 tumfl-0.1.1/tumfl/parser.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1243 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.190799 tumfl-0.1.1/tumfl.egg-info/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1206 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1609 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       57 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/requires.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        6 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/top_level.txt
```

### Comparing `tumfl-0.1.0/PKG-INFO` & `tumfl-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
-Project-URL: homepage, https://github.com/stormworks-utils/sw_mc_lib
-Project-URL: repository, https://github.com/stormworks-utils/sw_mc_lib
+Project-URL: homepage, https://github.com/stormworks-utils/tumfl
+Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tumfl-0.1.0/pyproject.toml` & `tumfl-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tumfl"
-version = "0.1.0"
+version = "0.1.1"
 description = "The Ultimate Minimizer For Lua: minimize your lua scripts"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["lua", "minimizer", "ast"]
 license = {text = "MIT License"}
 authors = [
     {name = "Fabian Wunsch"}
@@ -26,12 +26,12 @@
 ]
 dependencies = []
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pip-tools", "mypy", "flake8", "coverage", "pylint"]
 
 [project.urls]
-homepage = "https://github.com/stormworks-utils/sw_mc_lib"
-repository = "https://github.com/stormworks-utils/sw_mc_lib"
+homepage = "https://github.com/stormworks-utils/tumfl"
+repository = "https://github.com/stormworks-utils/tumfl"
 
 [tool.setuptools]
 packages = ["tumfl", "tumfl.AST", "tumfl.AST.Expression", "tumfl.AST.Statement"]
```

### Comparing `tumfl-0.1.0/test/test_lexer.py` & `tumfl-0.1.1/test/test_lexer.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/test/test_parser.py` & `tumfl-0.1.1/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/ASTNode.py` & `tumfl-0.1.1/tumfl/AST/ASTNode.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/BaseFunctionDefinition.py` & `tumfl-0.1.1/tumfl/AST/BaseFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/BinOp.py` & `tumfl-0.1.1/tumfl/AST/Expression/BinOp.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/ExpFunctionCall.py` & `tumfl-0.1.1/tumfl/AST/Expression/ExpFunctionCall.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/ExpFunctionDefinition.py` & `tumfl-0.1.1/tumfl/AST/Expression/ExpFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/ExpMethodInvocation.py` & `tumfl-0.1.1/tumfl/AST/Expression/ExpMethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/Name.py` & `tumfl-0.1.1/tumfl/AST/Expression/Name.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/Number.py` & `tumfl-0.1.1/tumfl/AST/Expression/Number.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/String.py` & `tumfl-0.1.1/tumfl/AST/Expression/String.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/TableField.py` & `tumfl-0.1.1/tumfl/AST/Expression/TableField.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/UnOp.py` & `tumfl-0.1.1/tumfl/AST/Expression/UnOp.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Expression/__init__.py` & `tumfl-0.1.1/tumfl/AST/Expression/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/Assign.py` & `tumfl-0.1.1/tumfl/AST/Statement/Assign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/Block.py` & `tumfl-0.1.1/tumfl/AST/Statement/Block.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/FunctionCall.py` & `tumfl-0.1.1/tumfl/AST/Statement/FunctionCall.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/FunctionDefinition.py` & `tumfl-0.1.1/tumfl/AST/Statement/FunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/If.py` & `tumfl-0.1.1/tumfl/AST/Statement/If.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/IterativeFor.py` & `tumfl-0.1.1/tumfl/AST/Statement/IterativeFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/LocalAssign.py` & `tumfl-0.1.1/tumfl/AST/Statement/LocalAssign.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/LocalFunctionDefinition.py` & `tumfl-0.1.1/tumfl/AST/Statement/LocalFunctionDefinition.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/MethodInvocation.py` & `tumfl-0.1.1/tumfl/AST/Statement/MethodInvocation.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/NumericFor.py` & `tumfl-0.1.1/tumfl/AST/Statement/NumericFor.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/AST/Statement/__init__.py` & `tumfl-0.1.1/tumfl/AST/Statement/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/Token.py` & `tumfl-0.1.1/tumfl/Token.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/error.py` & `tumfl-0.1.1/tumfl/error.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/lexer.py` & `tumfl-0.1.1/tumfl/lexer.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/parser.py` & `tumfl-0.1.1/tumfl/parser.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl/utils.py` & `tumfl-0.1.1/tumfl/utils.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.0/tumfl.egg-info/PKG-INFO` & `tumfl-0.1.1/tumfl.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.0
+Version: 0.1.1
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
-Project-URL: homepage, https://github.com/stormworks-utils/sw_mc_lib
-Project-URL: repository, https://github.com/stormworks-utils/sw_mc_lib
+Project-URL: homepage, https://github.com/stormworks-utils/tumfl
+Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tumfl-0.1.0/tumfl.egg-info/SOURCES.txt` & `tumfl-0.1.1/tumfl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

