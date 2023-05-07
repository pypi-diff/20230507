# Comparing `tmp/tumfl-0.1.1.tar.gz` & `tmp/tumfl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumfl-0.1.1.tar", last modified: Sun May  7 15:26:03 2023, max compression
+gzip compressed data, was "tumfl-0.1.2.tar", last modified: Sun May  7 17:46:56 2023, max compression
```

## Comparing `tumfl-0.1.1.tar` & `tumfl-0.1.2.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.195799 tumfl-0.1.1/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1206 2023-05-07 15:26:03.195799 tumfl-0.1.1/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      429 2022-08-10 22:55:26.000000 tumfl-0.1.1/README.md
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1075 2023-05-07 15:25:47.000000 tumfl-0.1.1/pyproject.toml
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       38 2023-05-07 15:26:03.195799 tumfl-0.1.1/setup.cfg
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.189799 tumfl-0.1.1/test/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    12038 2023-05-07 15:10:00.000000 tumfl-0.1.1/test/test_lexer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    34797 2023-05-07 15:13:56.000000 tumfl-0.1.1/test/test_parser.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.190799 tumfl-0.1.1/tumfl/
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.190799 tumfl-0.1.1/tumfl/AST/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-05-07 06:49:52.000000 tumfl-0.1.1/tumfl/AST/ASTNode.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      667 2023-05-07 07:41:59.000000 tumfl-0.1.1/tumfl/AST/BaseFunctionDefinition.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.192799 tumfl-0.1.1/tumfl/AST/Expression/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1163 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/BinOp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      507 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Boolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      513 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/ExpFunctionCall.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      820 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/ExpFunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      638 2023-05-07 06:48:48.000000 tumfl-0.1.1/tumfl/AST/Expression/ExpMethodInvocation.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      134 2023-02-03 20:08:43.000000 tumfl-0.1.1/tumfl/AST/Expression/Expression.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      414 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Index.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      533 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Name.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      437 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/NamedIndex.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      377 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Nil.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2088 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Number.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      531 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/String.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      384 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Table.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1086 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/TableField.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      705 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/UnOp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      408 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Vararg.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      180 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Expression/Variable.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      650 2023-05-07 15:14:20.000000 tumfl-0.1.1/tumfl/AST/Expression/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.195799 tumfl-0.1.1/tumfl/AST/Statement/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      530 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Assign.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      513 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Block.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      261 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Break.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      100 2023-05-04 07:15:57.000000 tumfl-0.1.1/tumfl/AST/Statement/Chunk.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      548 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/FunctionCall.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1134 2023-05-07 11:58:15.000000 tumfl-0.1.1/tumfl/AST/Statement/FunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      348 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Goto.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      623 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/If.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      649 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/IterativeFor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      360 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Label.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1135 2023-05-07 11:44:32.000000 tumfl-0.1.1/tumfl/AST/Statement/LocalAssign.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      988 2023-05-07 11:50:43.000000 tumfl-0.1.1/tumfl/AST/Statement/LocalFunctionDefinition.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      693 2023-05-07 06:48:41.000000 tumfl-0.1.1/tumfl/AST/Statement/MethodInvocation.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      791 2023-05-07 06:48:26.000000 tumfl-0.1.1/tumfl/AST/Statement/NumericFor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      450 2023-05-07 06:47:23.000000 tumfl-0.1.1/tumfl/AST/Statement/Repeat.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      247 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Semicolon.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      356 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/Statement.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      437 2023-05-07 06:47:23.000000 tumfl-0.1.1/tumfl/AST/Statement/While.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/Statement/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       80 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/AST/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2116 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/Token.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      120 2023-05-07 15:21:36.000000 tumfl-0.1.1/tumfl/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      605 2023-05-07 08:21:02.000000 tumfl-0.1.1/tumfl/error.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    14372 2023-05-07 15:13:11.000000 tumfl-0.1.1/tumfl/lexer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    32511 2023-05-07 15:01:48.000000 tumfl-0.1.1/tumfl/parser.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1243 2023-05-07 06:47:22.000000 tumfl-0.1.1/tumfl/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 15:26:03.190799 tumfl-0.1.1/tumfl.egg-info/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1206 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1609 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/SOURCES.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/dependency_links.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       57 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/requires.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        6 2023-05-07 15:26:03.000000 tumfl-0.1.1/tumfl.egg-info/top_level.txt
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 17:46:56.293007 tumfl-0.1.2/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1180 2023-05-07 17:46:56.293007 tumfl-0.1.2/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      403 2023-05-07 16:04:09.000000 tumfl-0.1.2/README.md
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1075 2023-05-07 17:46:24.000000 tumfl-0.1.2/pyproject.toml
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      175 2023-05-07 17:46:56.293007 tumfl-0.1.2/setup.cfg
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 17:46:56.287007 tumfl-0.1.2/test/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    12040 2023-05-07 15:43:26.000000 tumfl-0.1.2/test/test_lexer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    37047 2023-05-07 17:12:29.000000 tumfl-0.1.2/test/test_parser.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 17:46:56.288007 tumfl-0.1.2/tumfl/
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 17:46:56.289007 tumfl-0.1.2/tumfl/AST/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1303 2023-05-07 15:59:04.000000 tumfl-0.1.2/tumfl/AST/ASTNode.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      656 2023-05-07 15:47:19.000000 tumfl-0.1.2/tumfl/AST/BaseFunctionDefinition.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 17:46:56.290007 tumfl-0.1.2/tumfl/AST/Expression/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1152 2023-05-07 15:44:30.000000 tumfl-0.1.2/tumfl/AST/Expression/BinOp.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      507 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/AST/Expression/Boolean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      502 2023-05-07 15:44:48.000000 tumfl-0.1.2/tumfl/AST/Expression/ExpFunctionCall.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      809 2023-05-07 15:44:44.000000 tumfl-0.1.2/tumfl/AST/Expression/ExpFunctionDefinition.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      598 2023-05-07 15:44:56.000000 tumfl-0.1.2/tumfl/AST/Expression/ExpMethodInvocation.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      134 2023-02-03 20:08:43.000000 tumfl-0.1.2/tumfl/AST/Expression/Expression.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      419 2023-05-07 17:13:35.000000 tumfl-0.1.2/tumfl/AST/Expression/Index.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      533 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/AST/Expression/Name.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      444 2023-05-07 17:13:17.000000 tumfl-0.1.2/tumfl/AST/Expression/NamedIndex.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      377 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/AST/Expression/Nil.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2083 2023-05-07 15:45:21.000000 tumfl-0.1.2/tumfl/AST/Expression/Number.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      531 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/AST/Expression/String.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      373 2023-05-07 15:45:28.000000 tumfl-0.1.2/tumfl/AST/Expression/Table.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1066 2023-05-07 15:59:18.000000 tumfl-0.1.2/tumfl/AST/Expression/TableField.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      694 2023-05-07 15:45:38.000000 tumfl-0.1.2/tumfl/AST/Expression/UnOp.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      408 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/AST/Expression/Vararg.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      171 2023-05-07 15:59:24.000000 tumfl-0.1.2/tumfl/AST/Expression/Variable.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      650 2023-05-07 17:46:34.000000 tumfl-0.1.2/tumfl/AST/Expression/__init__.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 17:46:56.293007 tumfl-0.1.2/tumfl/AST/Statement/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      519 2023-05-07 15:45:49.000000 tumfl-0.1.2/tumfl/AST/Statement/Assign.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      502 2023-05-07 15:45:53.000000 tumfl-0.1.2/tumfl/AST/Statement/Block.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      250 2023-05-07 15:45:58.000000 tumfl-0.1.2/tumfl/AST/Statement/Break.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      100 2023-05-04 07:15:57.000000 tumfl-0.1.2/tumfl/AST/Statement/Chunk.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      537 2023-05-07 15:46:04.000000 tumfl-0.1.2/tumfl/AST/Statement/FunctionCall.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1123 2023-05-07 15:46:10.000000 tumfl-0.1.2/tumfl/AST/Statement/FunctionDefinition.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      337 2023-05-07 15:46:15.000000 tumfl-0.1.2/tumfl/AST/Statement/Goto.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 15:46:20.000000 tumfl-0.1.2/tumfl/AST/Statement/If.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      638 2023-05-07 15:46:25.000000 tumfl-0.1.2/tumfl/AST/Statement/IterativeFor.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      349 2023-05-07 15:46:29.000000 tumfl-0.1.2/tumfl/AST/Statement/Label.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1124 2023-05-07 15:46:35.000000 tumfl-0.1.2/tumfl/AST/Statement/LocalAssign.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      977 2023-05-07 15:46:40.000000 tumfl-0.1.2/tumfl/AST/Statement/LocalFunctionDefinition.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      653 2023-05-07 15:46:47.000000 tumfl-0.1.2/tumfl/AST/Statement/MethodInvocation.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      780 2023-05-07 15:46:51.000000 tumfl-0.1.2/tumfl/AST/Statement/NumericFor.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      439 2023-05-07 15:46:55.000000 tumfl-0.1.2/tumfl/AST/Statement/Repeat.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      236 2023-05-07 15:47:00.000000 tumfl-0.1.2/tumfl/AST/Statement/Semicolon.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      356 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/AST/Statement/Statement.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      426 2023-05-07 15:47:09.000000 tumfl-0.1.2/tumfl/AST/Statement/While.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      612 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/AST/Statement/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       80 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/AST/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2116 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/Token.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      120 2023-05-07 17:46:02.000000 tumfl-0.1.2/tumfl/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      605 2023-05-07 08:21:02.000000 tumfl-0.1.2/tumfl/error.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2023-05-07 17:44:29.000000 tumfl-0.1.2/tumfl/formatter.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    14367 2023-05-07 15:55:19.000000 tumfl-0.1.2/tumfl/lexer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    32621 2023-05-07 17:45:47.000000 tumfl-0.1.2/tumfl/parser.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1243 2023-05-07 06:47:22.000000 tumfl-0.1.2/tumfl/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-07 17:46:56.288007 tumfl-0.1.2/tumfl.egg-info/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1180 2023-05-07 17:46:56.000000 tumfl-0.1.2/tumfl.egg-info/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1638 2023-05-07 17:46:56.000000 tumfl-0.1.2/tumfl.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-07 17:46:56.000000 tumfl-0.1.2/tumfl.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       57 2023-05-07 17:46:56.000000 tumfl-0.1.2/tumfl.egg-info/requires.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        6 2023-05-07 17:46:56.000000 tumfl-0.1.2/tumfl.egg-info/top_level.txt
```

### Comparing `tumfl-0.1.1/PKG-INFO` & `tumfl-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
@@ -17,12 +17,12 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Tumfl: The Ultimate Minimizer For Lua
 
-[![codecov](https://codecov.io/gh/Factorio-debugging/factorio-circuit-ast/branch/main/graph/badge.svg?token=DO180QNO38)](https://codecov.io/gh/Factorio-debugging/factorio-circuit-ast)
+[![codecov](https://codecov.io/github/stormworks-utils/tumfl/branch/main/graph/badge.svg?token=X5TIVNJSZ7)](https://codecov.io/github/stormworks-utils/tumfl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This package contains the best minimizer you'll find on the market, or so I hope.
 # tumfl
```

### Comparing `tumfl-0.1.1/pyproject.toml` & `tumfl-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tumfl"
-version = "0.1.1"
+version = "0.1.2"
 description = "The Ultimate Minimizer For Lua: minimize your lua scripts"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["lua", "minimizer", "ast"]
 license = {text = "MIT License"}
 authors = [
     {name = "Fabian Wunsch"}
```

### Comparing `tumfl-0.1.1/test/test_lexer.py` & `tumfl-0.1.2/test/test_lexer.py`

 * *Files identical despite different names*

```diff
@@ -175,17 +175,17 @@
         lex = Lexer('"abc"')
         self.assertEqual(lex.get_string(), "abc")
         lex = Lexer("'abc'")
         self.assertEqual(lex.get_string(), "abc")
         self.assertEqual(lex.current_char, None)
 
     def test_skip_whitespace(self):
-        lex = Lexer("' \z    \n\ta'")
+        lex = Lexer("' \\z    \n\ta'")
         self.assertEqual(lex.get_string(), " a")
-        lex = Lexer("'\za'")
+        lex = Lexer("'\\za'")
         self.assertEqual(lex.get_string(), "a")
 
     def test_other_quote(self):
         lex = Lexer("'\"'")
         self.assertEqual(lex.get_string(), '"')
         lex = Lexer('"\'"')
         self.assertEqual(lex.get_string(), "'")
```

### Comparing `tumfl-0.1.1/test/test_parser.py` & `tumfl-0.1.2/test/test_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,56 +28,61 @@
     def test_simple_exp(self):
         parser = Parser("1+2")
         expected_tree = BinOp.from_token(
             Token(TokenType.PLUS, "+", 0, 0),
             self.parse_number("1"),
             self.parse_number("2"),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("4+5*6")
         expected_tree = BinOp.from_token(
             Token(TokenType.PLUS, "+", 0, 0),
             self.parse_number("4"),
             BinOp.from_token(
                 Token(TokenType.MULT, "*", 0, 0),
                 self.parse_number("5"),
                 self.parse_number("6"),
             ),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("true and false or 1")
         expected_tree = BinOp.from_token(
             Token(TokenType.OR, "or", 0, 0),
             BinOp.from_token(
                 Token(TokenType.AND, "and", 0, 0),
                 Boolean.from_token(Token(TokenType.TRUE, "true", 0, 0)),
                 Boolean.from_token(Token(TokenType.FALSE, "false", 0, 0)),
             ),
             self.parse_number("1"),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("-nil")
         expected_tree = UnOp.from_token(
             Token(TokenType.MINUS, "-", 0, 0),
             Nil.from_token(Token(TokenType.NIL, "nil", 0, 0)),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("\n#'a'")
         expected_tree = UnOp.from_token(
             Token(TokenType.HASH, "#", 0, 0),
             self.parse_string("a"),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("2^-2+s")
         expected_tree = BinOp.from_token(
             Token(TokenType.PLUS, "+", 0, 0),
             BinOp.from_token(
@@ -85,14 +90,15 @@
                 self.parse_number("2"),
                 UnOp.from_token(
                     Token(TokenType.MINUS, "-", 0, 0), self.parse_number("2")
                 ),
             ),
             self.parse_name("s"),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_associativity(self):
         parser = Parser("1^2^3")
         expected_tree = BinOp.from_token(
@@ -100,27 +106,29 @@
             self.parse_number("1"),
             BinOp.from_token(
                 Token(TokenType.EXPONENT, "^", 0, 0),
                 self.parse_number("2"),
                 self.parse_number("3"),
             ),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("1+2-3")
         expected_tree = BinOp.from_token(
             Token(TokenType.MINUS, "-", 0, 0),
             BinOp.from_token(
                 Token(TokenType.PLUS, "+", 0, 0),
                 self.parse_number("1"),
                 self.parse_number("2"),
             ),
             self.parse_number("3"),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_error(self):
         parser = Parser("1+")
         with self.assertRaises(ParserException):
@@ -129,28 +137,30 @@
     def test_unary_expr(self):
         parser = Parser("1- -2")
         expected_tree = BinOp.from_token(
             Token(TokenType.MINUS, "-", 0, 0),
             self.parse_number("1"),
             UnOp.from_token(Token(TokenType.MINUS, "-", 0, 0), self.parse_number("2")),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_len_operator(self):
         parser = Parser("\n#a + 1")
         expected_tree = BinOp.from_token(
             Token(TokenType.PLUS, "+", 0, 0),
             UnOp.from_token(
                 Token(TokenType.HASH, "#", 0, 0),
                 self.parse_name("a"),
             ),
             self.parse_number("1"),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_wrong_token(self):
         parser = Parser("a,b+")
         with self.assertRaises(ParserException):
@@ -166,105 +176,113 @@
             Index(
                 Token(TokenType.R_BRACKET, "[", 0, 0),
                 self.parse_name("a"),
                 self.parse_string("b"),
             ),
             self.parse_name("d"),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_var(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("(2)[1]")
         expected_tree = Index(
             Token(TokenType.L_BRACKET, "[", 0, 0),
             self.parse_number("2"),
             self.parse_number("1"),
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_var(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("(2)(1)")
         expected_tree = ExpFunctionCall(
             Token(TokenType.L_BRACKET, "[", 0, 0),
             self.parse_number("2"),
             [self.parse_number("1")],
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_var(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("a:b()")
         expected_tree = ExpMethodInvocation(
             Token(TokenType.COLON, "[", 0, 0),
             self.parse_name("a"),
             self.parse_name("b"),
             [],
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_var(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_table_constructor(self):
         parser = Parser("{}")
-        expected_result = Table(Token(TokenType.L_CURL, "{", 0, 0), [])
-        self.assertEqual(parser._parse_table_constructor(), expected_result)
+        expected_tree = Table(Token(TokenType.L_CURL, "{", 0, 0), [])
+        self.assertEqual(parser._parse_table_constructor(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("{a}")
-        expected_result = Table(
+        expected_tree = Table(
             Token(TokenType.L_CURL, "{", 0, 0),
             [
                 NumberedTableField(
                     Token(TokenType.NAME, "a", 0, 0), self.parse_name("a")
                 )
             ],
         )
-        self.assertEqual(parser._parse_table_constructor(), expected_result)
+        repr_test = repr(expected_tree)
+        self.assertEqual(parser._parse_table_constructor(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser('{["b"]=c}')
-        expected_result = Table(
+        expected_tree = Table(
             Token(TokenType.L_CURL, "{", 0, 0),
             [
                 ExplicitTableField(
                     Token(TokenType.L_BRACKET, "[", 0, 0),
                     self.parse_string("b"),
                     self.parse_name("c"),
                 )
             ],
         )
-        self.assertEqual(parser._parse_table_constructor(), expected_result)
+        repr_test = repr(expected_tree)
+        self.assertEqual(parser._parse_table_constructor(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("{a=b}")
-        expected_result = Table(
+        expected_tree = Table(
             Token(TokenType.L_CURL, "{", 0, 0),
             [
                 NamedTableField(
                     Token(TokenType.NAME, "a", 0, 0),
                     self.parse_name("a"),
                     self.parse_name("b"),
                 )
             ],
         )
-        self.assertEqual(parser._parse_table_constructor(), expected_result)
+        repr_test = repr(expected_tree)
+        self.assertEqual(parser._parse_table_constructor(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("{a, b,}")
-        expected_result = Table(
+        expected_tree = Table(
             Token(TokenType.L_CURL, "{", 0, 0),
             [
                 NumberedTableField(
                     Token(TokenType.NAME, "a", 0, 0), self.parse_name("a")
                 ),
                 NumberedTableField(
                     Token(TokenType.NAME, "b", 0, 0), self.parse_name("b")
                 ),
             ],
         )
-        self.assertEqual(parser._parse_table_constructor(), expected_result)
+        repr_test = repr(expected_tree)
+        self.assertEqual(parser._parse_table_constructor(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("{f'alo'..'xixi'}")
         expected_tree = Table(
             Token(TokenType.L_CURL, "{", 0, 0),
             [
                 NumberedTableField(
@@ -277,14 +295,15 @@
                             [self.parse_string("alo")],
                         ),
                         self.parse_string("xixi"),
                     ),
                 )
             ],
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser._parse_table_constructor(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_args(self):
         parser = Parser("()")
         self.assertEqual(parser._parse_args(), [])
@@ -343,90 +362,96 @@
             parser._parse_name_list()
         parser = Parser("a, 1")
         with self.assertRaises(ParserException):
             parser._parse_name_list()
 
     def test_parse_vararg(self):
         parser = Parser("...")
-        expected = Vararg(Token(TokenType.ELLIPSIS, "...", 0, 0))
-        self.assertEqual(parser._parse_exp(), expected)
+        expected_tree = Vararg(Token(TokenType.ELLIPSIS, "...", 0, 0))
+        self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_table_expr(self):
         parser = Parser("{a}")
-        expected = Parser("{a}")._parse_table_constructor()
-        self.assertEqual(parser._parse_exp(), expected)
+        expected_tree = Parser("{a}")._parse_table_constructor()
+        self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_funcbody(self):
         function_token = Token(TokenType.FUNCTION, "function", 0, 0)
         parser = Parser("()end")
-        expected = BaseFunctionDefinition(
+        expected_tree = BaseFunctionDefinition(
             function_token, [], Block(Token(TokenType.END, "end", 0, 0), [], [])
         )
+        repr_test = repr(expected_tree)
         parser._add_hint("function", "function")
-        self.assertEqual(parser._parse_funcbody(function_token), expected)
+        self.assertEqual(parser._parse_funcbody(function_token), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("(a,b)end")
-        expected = BaseFunctionDefinition(
+        expected_tree = BaseFunctionDefinition(
             function_token,
             [self.parse_name("a"), self.parse_name("b")],
             Block(Token(TokenType.END, "end", 0, 0), [], []),
         )
+        repr_test = repr(expected_tree)
         parser._add_hint("function", "function")
-        self.assertEqual(parser._parse_funcbody(function_token), expected)
+        self.assertEqual(parser._parse_funcbody(function_token), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("(...)end")
-        expected = BaseFunctionDefinition(
+        expected_tree = BaseFunctionDefinition(
             function_token,
             [Vararg.from_token(Token(TokenType.ELLIPSIS, "...", 0, 0))],
             Block(Token(TokenType.END, "end", 0, 0), [], []),
         )
+        repr_test = repr(expected_tree)
         parser._add_hint("function", "function")
-        self.assertEqual(parser._parse_funcbody(function_token), expected)
+        self.assertEqual(parser._parse_funcbody(function_token), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("(a,...)end")
-        expected = BaseFunctionDefinition(
+        expected_tree = BaseFunctionDefinition(
             function_token,
             [
                 self.parse_name("a"),
                 Vararg.from_token(Token(TokenType.ELLIPSIS, "...", 0, 0)),
             ],
             Block(Token(TokenType.END, "end", 0, 0), [], []),
         )
+        repr_test = repr(expected_tree)
         parser._add_hint("function", "function")
-        self.assertEqual(parser._parse_funcbody(function_token), expected)
+        self.assertEqual(parser._parse_funcbody(function_token), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_func_expr(self):
         parser = Parser("function()end")
-        expected = ExpFunctionDefinition(
+        expected_tree = ExpFunctionDefinition(
             Token(TokenType.FUNCTION, "function", 0, 0),
             [],
             Block(Token(TokenType.END, "end", 0, 0), [], []),
         )
-        self.assertEqual(parser._parse_exp(), expected)
+        repr_test = repr(expected_tree)
+        self.assertEqual(parser._parse_exp(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_assign(self):
         parser = Parser('a = "bcd"')
         expected_tree = self.get_chunk(
             Assign(
                 Token(TokenType.NAME, "a", 0, 0),
                 [self.parse_name("a")],
                 [self.parse_string("bcd")],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser('a,b,c = "bcd"')
         expected_tree = self.get_chunk(
             Assign(
                 Token(TokenType.NAME, "a", 0, 0),
@@ -434,37 +459,40 @@
                     self.parse_name("a"),
                     self.parse_name("b"),
                     self.parse_name("c"),
                 ],
                 [self.parse_string("bcd")],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser('a = "bcd", "def"')
         expected_tree = self.get_chunk(
             Assign(
                 Token(TokenType.NAME, "a", 0, 0),
                 [self.parse_name("a")],
                 [
                     self.parse_string("bcd"),
                     self.parse_string("def"),
                 ],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_function_stmt(self):
         parser = Parser("a()")
         expected_tree = self.get_chunk(
             FunctionCall(Token(TokenType.NAME, "a", 0, 0), self.parse_name("a"), [])
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("a[1].b()")
         expected_tree = self.get_chunk(
             FunctionCall(
                 Token(TokenType.NAME, "a", 0, 0),
@@ -476,35 +504,38 @@
                         self.parse_number("1"),
                     ),
                     self.parse_name("b"),
                 ),
                 [],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_method_stmt(self):
         parser = Parser("a:b()")
         expected_tree = self.get_chunk(
             MethodInvocation(
                 Token(TokenType.NAME, "a", 0, 0),
                 self.parse_name("a"),
                 self.parse_name("b"),
                 [],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_semicolon(self):
         parser = Parser(";")
         expected_tree = self.get_chunk(Semicolon(Token(TokenType.SEMICOLON, ";", 0, 0)))
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_local_assignment(self):
         parser = Parser("local a, b")
         expected_tree = self.get_chunk(
@@ -513,53 +544,57 @@
                 [
                     AttributedName(self.parse_name("a")),
                     AttributedName(self.parse_name("b")),
                 ],
                 None,
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("local a <const>, b <final>")
         expected_tree = self.get_chunk(
             LocalAssign(
                 Token(TokenType.LOCAL, "local", 0, 0),
                 [
                     AttributedName(self.parse_name("a"), self.parse_name("const")),
                     AttributedName(self.parse_name("b"), self.parse_name("final")),
                 ],
                 None,
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("local a=d,e")
         expected_tree = self.get_chunk(
             LocalAssign(
                 Token(TokenType.LOCAL, "local", 0, 0),
                 [AttributedName(self.parse_name("a"))],
                 [self.parse_name("d"), self.parse_name("e")],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_local_function(self):
         parser = Parser("local function a ()end")
         expected_tree = self.get_chunk(
             LocalFunctionDefinition(
                 Token(TokenType.LOCAL, "local", 0, 0),
                 self.parse_name("a"),
                 [],
                 Block(Token(TokenType.END, "end", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_unknown_local(self):
         parser = Parser("local and")
         with self.assertRaises(ParserException):
@@ -572,53 +607,57 @@
                 Token(TokenType.FUNCTION, "function", 0, 0),
                 [self.parse_name("a")],
                 None,
                 [],
                 Block(Token(TokenType.END, "end", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("function a.b:c ()end")
         expected_tree = self.get_chunk(
             FunctionDefinition(
                 Token(TokenType.FUNCTION, "function", 0, 0),
                 [self.parse_name("a"), self.parse_name("b")],
                 self.parse_name("c"),
                 [],
                 Block(Token(TokenType.END, "end", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_iterative_for(self):
         parser = Parser("for a in 2 do end")
         expected_tree = self.get_chunk(
             IterativeFor(
                 Token(TokenType.FOR, "for", 0, 0),
                 [self.parse_name("a")],
                 [self.parse_number("2")],
                 Block(Token(TokenType.DO, "do", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("for a, b in 1, 2 do end")
         expected_tree = self.get_chunk(
             IterativeFor(
                 Token(TokenType.FOR, "for", 0, 0),
                 [self.parse_name("a"), self.parse_name("b")],
                 [self.parse_number("1"), self.parse_number("2")],
                 Block(Token(TokenType.DO, "do", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_numeric_for(self):
         parser = Parser("for a=1,b do end")
         expected_tree = self.get_chunk(
@@ -627,28 +666,30 @@
                 self.parse_name("a"),
                 self.parse_number("1"),
                 self.parse_name("b"),
                 None,
                 Block(Token(TokenType.DO, "do", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("for a=1,b,3 do end")
         expected_tree = self.get_chunk(
             NumericFor(
                 Token(TokenType.FOR, "for", 0, 0),
                 self.parse_name("a"),
                 self.parse_number("1"),
                 self.parse_name("b"),
                 self.parse_number("3"),
                 Block(Token(TokenType.DO, "do", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_unknown_for(self):
         parser = Parser("for name and")
         with self.assertRaises(ParserException):
@@ -660,26 +701,28 @@
             If(
                 Token(TokenType.IF, "if", 0, 0),
                 self.parse_number("1"),
                 Block(Token(TokenType.THEN, "then", 0, 0), [], []),
                 None,
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("if 1 then else end")
         expected_tree = self.get_chunk(
             If(
                 Token(TokenType.IF, "if", 0, 0),
                 self.parse_number("1"),
                 Block(Token(TokenType.THEN, "then", 0, 0), [], []),
                 Block(Token(TokenType.ELSE, "else", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("if 1 then elseif 2 then else end")
         expected_tree = self.get_chunk(
             If(
                 Token(TokenType.IF, "if", 0, 0),
@@ -689,94 +732,103 @@
                     Token(TokenType.ELSEIF, "elseif", 0, 0),
                     self.parse_number("2"),
                     Block(Token(TokenType.ELSEIF, "elseif", 0, 0), [], []),
                     Block(Token(TokenType.ELSE, "else", 0, 0), [], []),
                 ),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_repeat(self):
         parser = Parser("repeat until 1")
         expected_tree = self.get_chunk(
             Repeat(
                 Token(TokenType.REPEAT, "repeat", 0, 0),
                 self.parse_number("1"),
                 Block(Token(TokenType.REPEAT, "repeat", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_while(self):
         parser = Parser("while 1 do end")
         expected_tree = self.get_chunk(
             While(
                 Token(TokenType.WHILE, "while", 0, 0),
                 self.parse_number("1"),
                 Block(Token(TokenType.DO, "do", 0, 0), [], []),
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_label(self):
         parser = Parser("::label::")
         expected_tree = self.get_chunk(
             Label(Token(TokenType.LABEL_BORDER, "::", 0, 0), self.parse_name("label"))
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_goto(self):
         parser = Parser("goto label")
         expected_tree = self.get_chunk(
             Goto(Token(TokenType.GOTO, "goto", 0, 0), self.parse_name("label"))
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_break(self):
         parser = Parser("break")
         expected_tree = self.get_chunk(Break(Token(TokenType.BREAK, "break", 0, 0)))
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_parse_block(self):
         parser = Parser("do end")
         expected_tree = self.get_chunk(Block(Token(TokenType.DO, "do", 0, 0), [], []))
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("do ; end")
         expected_tree = self.get_chunk(
             Block(
                 Token(TokenType.DO, "do", 0, 0),
                 [Semicolon(Token(TokenType.SEMICOLON, ";", 0, 0))],
                 [],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("do ;return a; end")
         expected_tree = self.get_chunk(
             Block(
                 Token(TokenType.DO, "do", 0, 0),
                 [Semicolon(Token(TokenType.SEMICOLON, ";", 0, 0))],
                 [self.parse_name("a")],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("do ;return a end")
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
@@ -784,25 +836,27 @@
         expected_tree = self.get_chunk(
             Block(
                 Token(TokenType.DO, "do", 0, 0),
                 [Semicolon(Token(TokenType.SEMICOLON, ";", 0, 0))],
                 [],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
         parser = Parser("do return end")
         expected_tree = self.get_chunk(
             Block(
                 Token(TokenType.DO, "do", 0, 0),
                 [],
                 [],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
 
     def test_unexpected_statement(self):
         parser = Parser("+")
         with self.assertRaises(ParserException):
@@ -815,10 +869,11 @@
                 Token(TokenType.NAME, "assert", 0, 0),
                 ExpFunctionCall(
                     Token(TokenType.NAME, "assert", 0, 0), self.parse_name("assert"), []
                 ),
                 [],
             )
         )
+        repr_test = repr(expected_tree)
         self.assertEqual(parser.parse_chunk(), expected_tree)
         self.assertEqual(len(parser.context_hints), 0)
         self.assertEqual(parser.current_token, Token(TokenType.EOF, "eof", 0, 0))
```

### Comparing `tumfl-0.1.1/tumfl/AST/ASTNode.py` & `tumfl-0.1.2/tumfl/AST/ASTNode.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
+from abc import ABC
 from typing import Any, Generator, Optional
 
 from tumfl.Token import Token
 from tumfl.utils import generic_str
 
 
 class ASTNode(ABC):
@@ -25,15 +25,15 @@
 
     def __repr__(self) -> str:
         return generic_str(self, ["replace", "parent", "parent_class"])
 
     def __dir(self) -> Generator[str, None, None]:
         return (
             i
-            for i in self.__dir__()
+            for i in dir(self)
             if not i.startswith("__")
             # ignore "token" for comparison (and parent check)
             and i not in ["replace", "parent", "parent_class", "var", "token"]
         )
 
     def parent(self, parent: ASTNode) -> None:
         self.parent_class = parent
```

### Comparing `tumfl-0.1.1/tumfl/AST/BaseFunctionDefinition.py` & `tumfl-0.1.2/tumfl/AST/BaseFunctionDefinition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from abc import ABC
 from typing import TYPE_CHECKING
 
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .ASTNode import ASTNode
 
 if TYPE_CHECKING:
     from .Expression.Name import Name
     from .Expression.Vararg import Vararg
     from .Statement.Block import Block
```

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/BinOp.py` & `tumfl-0.1.2/tumfl/AST/Expression/BinOp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from enum import Enum
 
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Expression import Expression
 
 
 class BinaryOperand(Enum):
     PLUS = "+"
     MINUS = "-"
```

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/ExpFunctionCall.py` & `tumfl-0.1.2/tumfl/AST/Expression/ExpMethodInvocation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Expression import Expression
+from .Name import Name
 
 
-class ExpFunctionCall(Expression):
-    """A function call, may be a statement or an expression. Like f(a,b,c) or f()"""
+class ExpMethodInvocation(Expression):
+    """A method invocation, may be a statement or an expression. Like f:b(a,b,c) or f:b()"""
 
     def __init__(
         self,
         token: Token,
         function: Expression,
+        method: Name,
         arguments: list[Expression],
     ):
-        super().__init__(token, "ExpFunctionCall")
+        super().__init__(token, "ExpMethodInvocation")
         self.function: Expression = function
+        self.method: Name = method
         self.arguments: list[Expression] = arguments
```

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/ExpFunctionDefinition.py` & `tumfl-0.1.2/tumfl/AST/Expression/ExpFunctionDefinition.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from tumfl.AST.BaseFunctionDefinition import BaseFunctionDefinition
 from tumfl.AST.Statement.Block import Block
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Expression import Expression
 from .Name import Name
 from .Vararg import Vararg
 
 
 class ExpFunctionDefinition(Expression):
```

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/ExpMethodInvocation.py` & `tumfl-0.1.2/tumfl/AST/Statement/MethodInvocation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from __future__ import annotations
 
-from typing import Optional
+from tumfl.AST.Expression import Expression
+from tumfl.AST.Expression.Name import Name
+from tumfl.Token import Token
 
-from tumfl.Token import Token, TokenType
+from .Statement import Statement
 
-from .Expression import Expression
-from .Name import Name
 
-
-class ExpMethodInvocation(Expression):
+class MethodInvocation(Statement):
     """A method invocation, may be a statement or an expression. Like f:b(a,b,c) or f:b()"""
 
     def __init__(
         self,
         token: Token,
         function: Expression,
         method: Name,
         arguments: list[Expression],
     ):
-        super().__init__(token, "ExpMethodInvocation")
+        super().__init__(token, "MethodInvocation")
         self.function: Expression = function
         self.method: Name = method
         self.arguments: list[Expression] = arguments
```

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/Name.py` & `tumfl-0.1.2/tumfl/AST/Expression/Name.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/Number.py` & `tumfl-0.1.2/tumfl/AST/Expression/Number.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Optional
+from typing import Optional
 
 from tumfl.Token import Token, TokenType
 
 from .Expression import Expression
 
 
 class Number(Expression):
```

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/String.py` & `tumfl-0.1.2/tumfl/AST/Expression/String.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/TableField.py` & `tumfl-0.1.2/tumfl/AST/Expression/TableField.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 
 from abc import ABC
 
 from tumfl.AST.ASTNode import ASTNode
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Expression import Expression
 from .Name import Name
 
 
 class TableField(ASTNode, ABC):
     """Base class for all table fields"""
 
-    ...
-
 
 class ExplicitTableField(TableField):
     """Table field of the form `[ expr ] = expr`"""
 
     def __init__(self, token: Token, at: Expression, value: Expression):
         super().__init__(token, "ExplicitTableField")
         self.at: Expression = at
```

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/UnOp.py` & `tumfl-0.1.2/tumfl/AST/Expression/UnOp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from enum import Enum
 
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Expression import Expression
 
 
 class UnaryOperand(Enum):
     MINUS = "-"
     HASH = "#"
```

### Comparing `tumfl-0.1.1/tumfl/AST/Expression/__init__.py` & `tumfl-0.1.2/tumfl/AST/Expression/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.1/tumfl/AST/Statement/Assign.py` & `tumfl-0.1.2/tumfl/AST/Statement/Assign.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from tumfl.AST.Expression.Expression import Expression
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Statement import Statement
 
 
 class Assign(Statement):
     """The assignment statement, like a,b = 1,nil"""
```

### Comparing `tumfl-0.1.1/tumfl/AST/Statement/FunctionCall.py` & `tumfl-0.1.2/tumfl/AST/Statement/FunctionCall.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from tumfl.AST.Expression import Expression
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Statement import Statement
 
 
 class FunctionCall(Statement):
     """A function call, may be a statement or an expression. Like f(a,b,c) or f()"""
```

### Comparing `tumfl-0.1.1/tumfl/AST/Statement/FunctionDefinition.py` & `tumfl-0.1.2/tumfl/AST/Statement/FunctionDefinition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from tumfl.AST.BaseFunctionDefinition import BaseFunctionDefinition
 from tumfl.AST.Expression.Name import Name
 from tumfl.AST.Expression.Vararg import Vararg
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Block import Block
 from .Statement import Statement
 
 
 class FunctionDefinition(Statement):
     """Definition of a lua function, NOT local"""
```

### Comparing `tumfl-0.1.1/tumfl/AST/Statement/If.py` & `tumfl-0.1.2/tumfl/AST/Statement/If.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from tumfl.AST.Expression.Expression import Expression
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Block import Block
 from .Statement import Statement
 
 
 class If(Statement):
     """An if statement, may contain a block or other if as false condition"""
```

### Comparing `tumfl-0.1.1/tumfl/AST/Statement/IterativeFor.py` & `tumfl-0.1.2/tumfl/AST/Statement/IterativeFor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from tumfl.AST.Expression.Expression import Expression
 from tumfl.AST.Expression.Name import Name
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Block import Block
 from .Statement import Statement
 
 
 class IterativeFor(Statement):
     """The iterative for, i.e. using pairs() or ipairs()"""
```

### Comparing `tumfl-0.1.1/tumfl/AST/Statement/LocalAssign.py` & `tumfl-0.1.2/tumfl/AST/Statement/LocalAssign.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 from tumfl.AST.Expression.Expression import Expression
 from tumfl.AST.Expression.Name import Name
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Statement import Statement
 
 
 class AttributedName:
     def __init__(self, name: Name, attribute: Optional[Name] = None):
         self.name: Name = name
```

### Comparing `tumfl-0.1.1/tumfl/AST/Statement/LocalFunctionDefinition.py` & `tumfl-0.1.2/tumfl/AST/Statement/LocalFunctionDefinition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from tumfl.AST.BaseFunctionDefinition import BaseFunctionDefinition
 from tumfl.AST.Expression.Name import Name
 from tumfl.AST.Expression.Vararg import Vararg
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Block import Block
 from .Statement import Statement
 
 
 class LocalFunctionDefinition(Statement):
     """Definition for a local function"""
```

### Comparing `tumfl-0.1.1/tumfl/AST/Statement/NumericFor.py` & `tumfl-0.1.2/tumfl/AST/Statement/NumericFor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from tumfl.AST.Expression.Expression import Expression
 from tumfl.AST.Expression.Name import Name
-from tumfl.Token import Token, TokenType
+from tumfl.Token import Token
 
 from .Block import Block
 from .Statement import Statement
 
 
 class NumericFor(Statement):
     """The numeric for, i.e. for i=1,10 do"""
```

### Comparing `tumfl-0.1.1/tumfl/AST/Statement/__init__.py` & `tumfl-0.1.2/tumfl/AST/Statement/__init__.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.1/tumfl/Token.py` & `tumfl-0.1.2/tumfl/Token.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.1/tumfl/error.py` & `tumfl-0.1.2/tumfl/error.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.1/tumfl/lexer.py` & `tumfl-0.1.2/tumfl/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
             elif self.current_char == "]":
                 closing_equals = 0
             else:
                 closing_equals = -1
             inner_string += self.current_char
             self.advance()
         self.error("long brackets never closed", line, column)
+        assert False
 
     def skip_comment(self) -> None:
         """Skip a comment (long or short)"""
         assert self.current_char == "-" and self.peek() == "-"
         self.advance()
         self.advance()
         comment: str = ""
@@ -356,16 +357,15 @@
 
             if self.current_char == "." and self.peek() == ".":
                 self.advance()
                 self.advance()
                 if self.current_char == ".":
                     self.advance()
                     return Token(TokenType.ELLIPSIS, "...", **args)
-                else:
-                    return Token(TokenType.CONCAT, "..", **args)
+                return Token(TokenType.CONCAT, "..", **args)
 
             if peek := self.peek():
                 double_character: str = self.current_char + peek
                 if token_type := SYMBOLS.get(double_character):
                     self.advance()
                     self.advance()
                     return Token(token_type, double_character, **args)
```

### Comparing `tumfl-0.1.1/tumfl/parser.py` & `tumfl-0.1.2/tumfl/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -273,17 +273,18 @@
         for_token: Token = self.current_token
         self._add_hint("for", "name")
         self._eat_token(TokenType.FOR)
         first_name: Name = self.__eat_name()
         self._remove_hint()
         if self.current_token.type == TokenType.ASSIGN:
             return self._parse_numeric_for(for_token, first_name)
-        elif self.current_token.type in (TokenType.COMMA, TokenType.IN):
+        if self.current_token.type in (TokenType.COMMA, TokenType.IN):
             return self._parse_iterative_for(for_token, first_name)
         self._error("unexpected for condition", self.current_token)
+        assert False
 
     def _parse_numeric_for(self, for_token: Token, name: Name) -> NumericFor:
         """
         Parse a numeric for
 
         num_for: FOR Name ASSIGN exp COMMA exp [COMMA exp] DO block END
         """
@@ -379,17 +380,18 @@
 
         local_stmt: local_funct_stmt | local_assign_stmt
         """
         local_token: Token = self.current_token
         self._eat_token(TokenType.LOCAL)
         if self.current_token.type == TokenType.FUNCTION:
             return self._parse_local_function(local_token)
-        elif self.current_token.type == TokenType.NAME:
+        if self.current_token.type == TokenType.NAME:
             return self._parse_local_assignment(local_token)
         self._error("Unexpected symbol after local", self.current_token)
+        assert False
 
     def _parse_local_function(self, local_token: Token) -> LocalFunctionDefinition:
         """
         Parse a local function definition
 
         local_funct_stmt: LOCAL FUNCTION Name funcbody
         """
@@ -463,19 +465,19 @@
 
         var_funct: assign_stmt | funct_call_stmt
         """
         first_token: Token = self.current_token
         first_var: Expression = self._parse_var()
         if self.current_token.type in (TokenType.COMMA, TokenType.ASSIGN):
             return self._parse_assignment(first_token, first_var)
-        elif isinstance(first_var, ExpFunctionCall):
+        if isinstance(first_var, ExpFunctionCall):
             return FunctionCall(
                 first_var.token, first_var.function, first_var.arguments
             )
-        elif isinstance(first_var, ExpMethodInvocation):
+        if isinstance(first_var, ExpMethodInvocation):
             return MethodInvocation(
                 first_var.token,
                 first_var.function,
                 first_var.method,
                 first_var.arguments,
             )
         assert False, "unreachable line"
@@ -673,40 +675,41 @@
 
         atom: NIL | TRUE | FALSE | NUMBER | STRING | ELLIPSIS | FUNCTION func_def | tableconstructor | var
         """
         token: Token = self.current_token
         if token.type == TokenType.NIL:
             self._eat_token()
             return Nil.from_token(token)
-        elif token.type == TokenType.TRUE:
+        if token.type == TokenType.TRUE:
             self._eat_token()
             return Boolean.from_token(token)
-        elif token.type == TokenType.FALSE:
+        if token.type == TokenType.FALSE:
             self._eat_token()
             return Boolean.from_token(token)
-        elif token.type == TokenType.NUMBER:
+        if token.type == TokenType.NUMBER:
             self._eat_token()
             return Number.from_token(token)
-        elif token.type == TokenType.STRING:
+        if token.type == TokenType.STRING:
             self._eat_token()
             return String.from_token(token)
-        elif token.type == TokenType.ELLIPSIS:
+        if token.type == TokenType.ELLIPSIS:
             self._eat_token()
             return Vararg.from_token(token)
-        elif token.type == TokenType.FUNCTION:
+        if token.type == TokenType.FUNCTION:
             function_token: Token = self.current_token
             self._add_hint("function expression", "definition")
             self._eat_token()
             base_function: BaseFunctionDefinition = self._parse_funcbody(function_token)
             return ExpFunctionDefinition.from_base_definition(base_function)
-        elif token.type == TokenType.L_CURL:
+        if token.type == TokenType.L_CURL:
             return self._parse_table_constructor()
-        elif token.type in (TokenType.L_PAREN, TokenType.NAME):
+        if token.type in (TokenType.L_PAREN, TokenType.NAME):
             return self._parse_var()
         self._error("Unexpected expression", self.current_token)
+        assert False
 
     def _parse_name_list(
         self, first_name: Optional[Name] = None, leave_vararg: bool = False
     ) -> list[Name]:
         """
         Parse a list of names
 
@@ -832,15 +835,15 @@
             at: Expression = self._parse_exp()
             self._eat_token(TokenType.R_BRACKET)
             self._switch_hint("value expression")
             self._eat_token(TokenType.ASSIGN)
             value = self._parse_exp()
             self._remove_hint()
             return ExplicitTableField(token, at, value)
-        elif (
+        if (
             self.current_token.type == TokenType.NAME
             and self.next_token.type == TokenType.ASSIGN
         ):
             self._add_hint("named table field", "name")
             name: Name = self.__eat_name()
             self._switch_hint("value expression")
             self._eat_token(TokenType.ASSIGN)
@@ -870,7 +873,11 @@
         elif self.current_token.type == TokenType.STRING:
             expressions.append(String.from_token(self.current_token))
             self._eat_token()
         else:
             assert False, "unreachable line"
         self._remove_hint()
         return expressions
+
+
+def parse(chunk: str) -> Chunk:
+    return Parser(chunk).parse_chunk()
```

### Comparing `tumfl-0.1.1/tumfl/utils.py` & `tumfl-0.1.2/tumfl/utils.py`

 * *Files identical despite different names*

### Comparing `tumfl-0.1.1/tumfl.egg-info/PKG-INFO` & `tumfl-0.1.2/tumfl.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumfl
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Ultimate Minimizer For Lua: minimize your lua scripts
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/tumfl
 Project-URL: repository, https://github.com/stormworks-utils/tumfl
 Keywords: lua,minimizer,ast
 Classifier: Programming Language :: Python :: 3
@@ -17,12 +17,12 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Tumfl: The Ultimate Minimizer For Lua
 
-[![codecov](https://codecov.io/gh/Factorio-debugging/factorio-circuit-ast/branch/main/graph/badge.svg?token=DO180QNO38)](https://codecov.io/gh/Factorio-debugging/factorio-circuit-ast)
+[![codecov](https://codecov.io/github/stormworks-utils/tumfl/branch/main/graph/badge.svg?token=X5TIVNJSZ7)](https://codecov.io/github/stormworks-utils/tumfl)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 This package contains the best minimizer you'll find on the market, or so I hope.
 # tumfl
```

### Comparing `tumfl-0.1.1/tumfl.egg-info/SOURCES.txt` & `tumfl-0.1.2/tumfl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 README.md
 pyproject.toml
+setup.cfg
 test/test_lexer.py
 test/test_parser.py
 tumfl/Token.py
 tumfl/__init__.py
 tumfl/error.py
+tumfl/formatter.py
 tumfl/lexer.py
 tumfl/parser.py
 tumfl/utils.py
 tumfl.egg-info/PKG-INFO
 tumfl.egg-info/SOURCES.txt
 tumfl.egg-info/dependency_links.txt
 tumfl.egg-info/requires.txt
```

