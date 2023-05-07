# Comparing `tmp/simple_starlette-2.3.2.tar.gz` & `tmp/simple_starlette-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_starlette-2.3.2.tar", last modified: Sun Feb 12 08:28:36 2023, max compression
+gzip compressed data, was "simple_starlette-3.0.0.tar", last modified: Sun May  7 12:09:17 2023, max compression
```

## Comparing `simple_starlette-2.3.2.tar` & `simple_starlette-3.0.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.818796 simple_starlette-2.3.2/
--rw-r--r--   0 jjj       (1000) jjj       (1000)    35149 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/LICENSE
--rw-r--r--   0 jjj       (1000) jjj       (1000)     2419 2023-02-12 08:28:36.817798 simple_starlette-2.3.2/PKG-INFO
--rw-r--r--   0 jjj       (1000) jjj       (1000)     2172 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/README.md
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.785943 simple_starlette-2.3.2/example/
--rw-r--r--   0 jjj       (1000) jjj       (1000)        0 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/__init__.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     2189 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/auth_middleware.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      920 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/ctxvars.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     1563 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/curd.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      511 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/curd_cbv.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     1280 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/err_handle.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      660 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/include_api.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      360 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/json_rpc_client.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      393 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/json_rpc_server.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     2028 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/rate_limiter.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      531 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/redis_demo.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      866 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/req_hook.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      618 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/sentry_demo.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     3106 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/sqlalchemy_db.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     3468 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/example/use_simple_api_docs.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)       55 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/pyproject.toml
--rw-r--r--   0 jjj       (1000) jjj       (1000)       38 2023-02-12 08:28:36.818796 simple_starlette-2.3.2/setup.cfg
--rw-r--r--   0 jjj       (1000) jjj       (1000)      673 2023-02-12 08:28:30.000000 simple_starlette-2.3.2/setup.py
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.794919 simple_starlette-2.3.2/simple_starlette/
--rw-r--r--   0 jjj       (1000) jjj       (1000)      551 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/__init__.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)    13230 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/app.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     1075 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/args.py
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.802932 simple_starlette-2.3.2/simple_starlette/cache/
--rw-r--r--   0 jjj       (1000) jjj       (1000)        0 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/cache/__init__.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      875 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/cache/guava_cache.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     9337 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/cache/memory_cache.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      834 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/cache/redis_cache.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      159 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/code.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     2932 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/config.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     3824 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/ctx.py
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.804926 simple_starlette-2.3.2/simple_starlette/db/
--rw-r--r--   0 jjj       (1000) jjj       (1000)        0 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/db/__init__.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)    12009 2023-02-12 08:18:52.000000 simple_starlette-2.3.2/simple_starlette/db/db_sqlalchemy.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      981 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/db/redis.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     3582 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/dispatch_request.py
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.805923 simple_starlette-2.3.2/simple_starlette/docs/
--rw-r--r--   0 jjj       (1000) jjj       (1000)        0 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/docs/__init__.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     6971 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/docs/api.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     2472 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/exceptions.py
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.807918 simple_starlette-2.3.2/simple_starlette/http_client/
--rw-r--r--   0 jjj       (1000) jjj       (1000)        0 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/http_client/__init__.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     5579 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/http_client/request_utils.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     1267 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/include.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      800 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/logger.py
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.810882 simple_starlette-2.3.2/simple_starlette/middleware/
--rw-r--r--   0 jjj       (1000) jjj       (1000)      462 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/middleware/__init__.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      882 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/middleware/cors.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     6713 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/middleware/rate_limiter.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     6956 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/middleware/token_auth.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     1393 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/responses.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     5085 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/route.py
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.811793 simple_starlette-2.3.2/simple_starlette/rpc/
--rw-r--r--   0 jjj       (1000) jjj       (1000)        0 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/rpc/__init__.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)     2253 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/rpc/json_rpc.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      510 2023-02-11 14:38:36.000000 simple_starlette-2.3.2/simple_starlette/types.py
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.798942 simple_starlette-2.3.2/simple_starlette.egg-info/
--rw-r--r--   0 jjj       (1000) jjj       (1000)     2419 2023-02-12 08:28:36.000000 simple_starlette-2.3.2/simple_starlette.egg-info/PKG-INFO
--rw-r--r--   0 jjj       (1000) jjj       (1000)     1707 2023-02-12 08:28:36.000000 simple_starlette-2.3.2/simple_starlette.egg-info/SOURCES.txt
--rw-r--r--   0 jjj       (1000) jjj       (1000)        1 2023-02-12 08:28:36.000000 simple_starlette-2.3.2/simple_starlette.egg-info/dependency_links.txt
--rw-r--r--   0 jjj       (1000) jjj       (1000)      244 2023-02-12 08:28:36.000000 simple_starlette-2.3.2/simple_starlette.egg-info/requires.txt
--rw-r--r--   0 jjj       (1000) jjj       (1000)       31 2023-02-12 08:28:36.000000 simple_starlette-2.3.2/simple_starlette.egg-info/top_level.txt
-drwxr-xr-x   0 jjj       (1000) jjj       (1000)        0 2023-02-12 08:28:36.817798 simple_starlette-2.3.2/tests/
--rw-r--r--   0 jjj       (1000) jjj       (1000)        0 2023-02-11 14:38:37.000000 simple_starlette-2.3.2/tests/__init__.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)       16 2023-02-11 14:38:37.000000 simple_starlette-2.3.2/tests/conf.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      498 2023-02-11 14:38:37.000000 simple_starlette-2.3.2/tests/config_tests.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      192 2023-02-11 14:38:37.000000 simple_starlette-2.3.2/tests/conftest.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)        0 2023-02-11 14:38:37.000000 simple_starlette-2.3.2/tests/crx_tests.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)      389 2023-02-11 14:38:37.000000 simple_starlette-2.3.2/tests/memory_cache_tests.py
--rw-r--r--   0 jjj       (1000) jjj       (1000)       26 2023-02-11 14:38:37.000000 simple_starlette-2.3.2/tests/p_tests.py
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.020809 simple_starlette-3.0.0/
+-rw-r--r--   0 riverjiang   (501) staff       (20)    35149 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/LICENSE
+-rw-r--r--   0 riverjiang   (501) staff       (20)     2914 2023-05-07 12:09:17.020625 simple_starlette-3.0.0/PKG-INFO
+-rw-r--r--   0 riverjiang   (501) staff       (20)     2722 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/README.md
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.013324 simple_starlette-3.0.0/example/
+-rw-r--r--   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/__init__.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     2189 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/auth_middleware.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      920 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/ctxvars.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     1563 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/curd.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      511 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/curd_cbv.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     1280 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/err_handle.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      660 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/include_api.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      360 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/json_rpc_client.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      393 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/json_rpc_server.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     2028 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/rate_limiter.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      531 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/redis_demo.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      866 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/req_hook.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      618 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/sentry_demo.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     3960 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/sqlalchemy_db.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     3468 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/example/use_simple_api_docs.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)       55 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/pyproject.toml
+-rw-r--r--   0 riverjiang   (501) staff       (20)       38 2023-05-07 12:09:17.020852 simple_starlette-3.0.0/setup.cfg
+-rw-r--r--   0 riverjiang   (501) staff       (20)      701 2023-05-07 12:06:56.000000 simple_starlette-3.0.0/setup.py
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.015908 simple_starlette-3.0.0/simple_starlette/
+-rw-r--r--   0 riverjiang   (501) staff       (20)      551 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/__init__.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)    13230 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/app.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     1239 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/args.py
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.017149 simple_starlette-3.0.0/simple_starlette/cache/
+-rw-r--r--   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/cache/__init__.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      875 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/cache/guava_cache.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     9337 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/cache/memory_cache.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      834 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/cache/redis_cache.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      159 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/code.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     2932 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/config.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     3824 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/ctx.py
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.017749 simple_starlette-3.0.0/simple_starlette/db/
+-rw-r--r--   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/db/__init__.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)    12671 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/db/db_sqlalchemy.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     1000 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/db/redis.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      176 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/db/sqlalchemy_types.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     3582 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/dispatch_request.py
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.018016 simple_starlette-3.0.0/simple_starlette/docs/
+-rw-r--r--   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/docs/__init__.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     6971 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/docs/api.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     2472 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/exceptions.py
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.018289 simple_starlette-3.0.0/simple_starlette/http_client/
+-rw-r--r--   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/http_client/__init__.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     5579 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/http_client/request_utils.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     1267 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/include.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      800 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/logger.py
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.018896 simple_starlette-3.0.0/simple_starlette/middleware/
+-rw-r--r--   0 riverjiang   (501) staff       (20)      462 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/middleware/__init__.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      882 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/middleware/cors.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     6682 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/middleware/rate_limiter.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     6956 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/middleware/token_auth.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     1393 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/responses.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     5085 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/route.py
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.019155 simple_starlette-3.0.0/simple_starlette/rpc/
+-rw-r--r--   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/rpc/__init__.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)     2253 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/rpc/json_rpc.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      510 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/simple_starlette/types.py
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.016597 simple_starlette-3.0.0/simple_starlette.egg-info/
+-rw-r--r--   0 riverjiang   (501) staff       (20)     2914 2023-05-07 12:09:17.000000 simple_starlette-3.0.0/simple_starlette.egg-info/PKG-INFO
+-rw-r--r--   0 riverjiang   (501) staff       (20)     1747 2023-05-07 12:09:17.000000 simple_starlette-3.0.0/simple_starlette.egg-info/SOURCES.txt
+-rw-r--r--   0 riverjiang   (501) staff       (20)        1 2023-05-07 12:09:17.000000 simple_starlette-3.0.0/simple_starlette.egg-info/dependency_links.txt
+-rw-r--r--   0 riverjiang   (501) staff       (20)      259 2023-05-07 12:09:17.000000 simple_starlette-3.0.0/simple_starlette.egg-info/requires.txt
+-rw-r--r--   0 riverjiang   (501) staff       (20)       31 2023-05-07 12:09:17.000000 simple_starlette-3.0.0/simple_starlette.egg-info/top_level.txt
+drwxr-xr-x   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:09:17.020395 simple_starlette-3.0.0/tests/
+-rw-r--r--   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/tests/__init__.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)       16 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/tests/conf.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      534 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/tests/config_tests.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      177 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/tests/conftest.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)        0 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/tests/crx_tests.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)      494 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/tests/memory_cache_tests.py
+-rw-r--r--   0 riverjiang   (501) staff       (20)       26 2023-05-07 12:05:40.000000 simple_starlette-3.0.0/tests/p_tests.py
```

### Comparing `simple_starlette-2.3.2/LICENSE` & `simple_starlette-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/PKG-INFO` & `simple_starlette-3.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: simple_starlette
-Version: 2.3.2
-Summary: a micro server
-Home-page: UNKNOWN
-Author: asbt
-Author-email: sg5htd@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Simple-Starlette
 
 [![License](https://img.shields.io/static/v1?label=asgi&message=starlette&color=red)]()
 [![License](https://img.shields.io/static/v1?label=asgi-server&message=uvicorn&color=green)]()
 [![License](https://img.shields.io/static/v1?label=imports&message=isort&color=origin)]()
 [![License](https://img.shields.io/static/v1?label=format&message=black&color=origin)]()
 [![License](https://img.shields.io/static/v1?label=type-hint&message=pyright&color=origin)]()
@@ -67,22 +55,51 @@
 # curl http://localhost:9091/test?arg1=hello&arg2=world
 # response:
 # {"arg1":"hello", "arg2":"world"}
 ```
 查看更多开发使用实例：[example usage](https://github.com/mapyJJJ/simple-starlette/tree/master/example)
 
 ---
-关于框架：   
-目的是整合业界常用的技术选型与各种解决方案的封装，在保证框架稳定性与高性能的前提下，提供快速开发与部署后端项目的能力
-todo：[todo](https://github.com/mapyJJJ/simple-starlette/tree/master/todo.md)
+#### basic:
 
----
+- apis支持: 
+    - `cbv/fbv http api`
+    - `json-rpc`
+    - `tcp-rpc`
+    - `grpc-rpc`
+    - `websocket`
+
+- middleware:
+    - `cors`
+    - `auth jwt+cookie`
+    - `api-rate-limit`
+    - `sentry`
+    - ...(compatible all asgi middleware)
+
+- database:
+    - relational database: `mysql + sqlalchemy`, `postgresql + sqlalchemy`
+    - not noly sql database: `redis`, `mongodb`   
+
+- cache:
+    - ttl: `ttlcache`, `lruttlcache`
+    - guava_cache: `GuavaCache`
+    - redis-cache
+
+- async task(定时，延时执行): 
+    - `simple-async-task`: 
+    - `celery` : 一般架构为(celery+rabbitmq)
+
+- other: 
+    - `simple-api-docs`
+    - `polish query/body params`
+    - `type hint`
 
+---
+各类系统架构template [README](https://github.com/mapyJJJ/simple-starlette/blob/master/system_architecture_template/README.md)
 
 
 ---
 #### LICENSE
 
 [GPL-3.0 License](https://github.com/mapyJJJ/simple-starlette/blob/master/LICENSE)
 
----
-
+---
```

### Comparing `simple_starlette-2.3.2/README.md` & `simple_starlette-3.0.0/simple_starlette.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: simple-starlette
+Version: 3.0.0
+Summary: a micro server
+Author: asbt
+Author-email: sg5htd@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Simple-Starlette
 
 [![License](https://img.shields.io/static/v1?label=asgi&message=starlette&color=red)]()
 [![License](https://img.shields.io/static/v1?label=asgi-server&message=uvicorn&color=green)]()
 [![License](https://img.shields.io/static/v1?label=imports&message=isort&color=origin)]()
 [![License](https://img.shields.io/static/v1?label=format&message=black&color=origin)]()
 [![License](https://img.shields.io/static/v1?label=type-hint&message=pyright&color=origin)]()
@@ -55,21 +64,51 @@
 # curl http://localhost:9091/test?arg1=hello&arg2=world
 # response:
 # {"arg1":"hello", "arg2":"world"}
 ```
 查看更多开发使用实例：[example usage](https://github.com/mapyJJJ/simple-starlette/tree/master/example)
 
 ---
-关于框架：   
-目的是整合业界常用的技术选型与各种解决方案的封装，在保证框架稳定性与高性能的前提下，提供快速开发与部署后端项目的能力
-todo：[todo](https://github.com/mapyJJJ/simple-starlette/tree/master/todo.md)
+#### basic:
 
----
+- apis支持: 
+    - `cbv/fbv http api`
+    - `json-rpc`
+    - `tcp-rpc`
+    - `grpc-rpc`
+    - `websocket`
+
+- middleware:
+    - `cors`
+    - `auth jwt+cookie`
+    - `api-rate-limit`
+    - `sentry`
+    - ...(compatible all asgi middleware)
+
+- database:
+    - relational database: `mysql + sqlalchemy`, `postgresql + sqlalchemy`
+    - not noly sql database: `redis`, `mongodb`   
+
+- cache:
+    - ttl: `ttlcache`, `lruttlcache`
+    - guava_cache: `GuavaCache`
+    - redis-cache
+
+- async task(定时，延时执行): 
+    - `simple-async-task`: 
+    - `celery` : 一般架构为(celery+rabbitmq)
+
+- other: 
+    - `simple-api-docs`
+    - `polish query/body params`
+    - `type hint`
 
+---
+各类系统架构template [README](https://github.com/mapyJJJ/simple-starlette/blob/master/system_architecture_template/README.md)
 
 
 ---
 #### LICENSE
 
 [GPL-3.0 License](https://github.com/mapyJJJ/simple-starlette/blob/master/LICENSE)
 
----
+---
```

### Comparing `simple_starlette-2.3.2/example/auth_middleware.py` & `simple_starlette-3.0.0/example/auth_middleware.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/example/ctxvars.py` & `simple_starlette-3.0.0/example/ctxvars.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/example/curd.py` & `simple_starlette-3.0.0/example/curd.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/example/err_handle.py` & `simple_starlette-3.0.0/example/err_handle.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/example/include_api.py` & `simple_starlette-3.0.0/example/include_api.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/example/rate_limiter.py` & `simple_starlette-3.0.0/example/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/example/redis_demo.py` & `simple_starlette-3.0.0/example/redis_demo.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/example/req_hook.py` & `simple_starlette-3.0.0/example/req_hook.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/example/sentry_demo.py` & `simple_starlette-3.0.0/example/sentry_demo.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/example/use_simple_api_docs.py` & `simple_starlette-3.0.0/example/use_simple_api_docs.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/setup.py` & `simple_starlette-3.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 from setuptools import find_packages, setup
 
-__version__ = "2.3.2"
+__version__ = "3.0.0"
 
 find_file_path = (
     lambda file_name: os.path.split(__file__)[0] + "/" + file_name
 )
 
 requires = (
-    open(find_file_path("dev_requirements.txt"), "r")
+    open(os.path.join(os.getcwd(), "dev_requirements.txt"), "r")
     .read()
     .split("/n")
 )
-with open(find_file_path("README.md"), "r", encoding="utf-8") as fh:
+with open(
+    os.path.join(os.getcwd(), "README.md"), "r", encoding="utf-8"
+) as fh:
     long_description = fh.read()
 
 
 setup(
     author="asbt",
     version=__version__,
     name="simple_starlette",
```

### Comparing `simple_starlette-2.3.2/simple_starlette/__init__.py` & `simple_starlette-3.0.0/simple_starlette/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/app.py` & `simple_starlette-3.0.0/simple_starlette/app.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/args.py` & `simple_starlette-3.0.0/simple_starlette/args.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # args.py
 # ~~~~~~~~
 
 from abc import ABCMeta
-from typing import Dict, Optional, Union, cast
+from typing import Dict, Optional, Union, cast, Union, Callable, overload
 
 import pydantic
 
 from simple_starlette.types import ArgsT
 
 
 class BaseModel(pydantic.BaseModel, metaclass=ABCMeta):
@@ -24,15 +24,24 @@
 class ResponseParams(BaseModel, metaclass=ABCMeta):
     ...
 
 
 request_args_model_map: Dict[str, Union[QueryParams, BodyParams]] = {}
 
 
-def register_args(cls: Optional[ArgsT] = None) -> ArgsT:
+
+@overload
+def register_args(cls: ArgsT) -> ArgsT:
+    ...
+
+@overload
+def register_args() -> Callable:
+    ...
+    
+def register_args(cls: Optional[ArgsT] = None) -> Union[Callable, ArgsT]:    
     if not cls:
         return lambda cls: register_args(cls)  # type: ignore
 
     cls_name = getattr(cls, "__name__")
     if issubclass(cls, (QueryParams, BodyParams)):  # type: ignore
         if cls_name in request_args_model_map:
             raise AttributeError(
```

### Comparing `simple_starlette-2.3.2/simple_starlette/cache/guava_cache.py` & `simple_starlette-3.0.0/simple_starlette/cache/guava_cache.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/cache/memory_cache.py` & `simple_starlette-3.0.0/simple_starlette/cache/memory_cache.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/cache/redis_cache.py` & `simple_starlette-3.0.0/simple_starlette/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/config.py` & `simple_starlette-3.0.0/simple_starlette/config.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/ctx.py` & `simple_starlette-3.0.0/simple_starlette/ctx.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/db/db_sqlalchemy.py` & `simple_starlette-3.0.0/simple_starlette/db/db_sqlalchemy.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,78 @@
 # asyncio orm docs: https://docs.sqlalchemy.org/en/14/orm/extensions/asyncio.html
 # ~~~~~~~~~~~~~
 
 import logging
 import random
 import re
 from datetime import datetime
-from typing import (TYPE_CHECKING, Any, Callable, Dict, Generic, List,
-                    Type, TypeVar, Union, cast, overload)
-
-from sqlalchemy.ext.asyncio import async_scoped_session, create_async_engine
-from sqlalchemy.ext.asyncio.session import AsyncSession as _AsyncSession
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    List,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
+
+from sqlalchemy import delete, update, insert, delete
+from sqlalchemy.ext.asyncio import (
+    async_scoped_session,
+    create_async_engine,
+)
+from sqlalchemy.ext.asyncio.session import (
+    AsyncSession as _AsyncSession,
+)
+from sqlalchemy.sql.elements import Label
+from sqlalchemy.sql.functions import count
+from sqlalchemy.sql.schema import Index
 from sqlalchemy.ext.declarative import DeclarativeMeta, declared_attr
 from sqlalchemy.orm import Session, sessionmaker
 from sqlalchemy.orm.decl_api import registry
 from sqlalchemy.orm.session import Session
 from sqlalchemy.sql.dml import Delete, Insert, Update
 from sqlalchemy.sql.schema import Column
-from sqlalchemy.sql.sqltypes import (BIGINT, DECIMAL, NUMERIC, BigInteger,
-                                     Boolean, Date, DateTime, Float, Integer,
-                                     String, Time, Text)
+from sqlalchemy.sql.sqltypes import (
+    BIGINT,
+    DECIMAL,
+    NUMERIC,
+    BigInteger,
+    Boolean,
+    Date,
+    DateTime,
+    Float,
+    Integer,
+    String,
+    Time,
+    Text,
+)
 
 from simple_starlette.ctx import g
+from .sqlalchemy_types import Select
+from sqlalchemy import select
 
 logger = logging.getLogger("sqlalchemy_db")
 
 D = TypeVar("D")
 C = TypeVar("C")
 
+select = cast(Type[Select], select)
+update = update
+insert = insert
+delete = delete
+Label = Label
+count = count
+Index = Index
+
+
 
 def check_cls_need_tablename(cls):
     if cls.__dict__.get("__abstract__", False) or not any(
         isinstance(b, DeclarativeMeta) for b in cls.__mro__[1:]
     ):
         return False
 
@@ -94,14 +136,15 @@
             return cls(**kwargs)
 
 
 def row_obj_to_dict(
     obj,
     exclude_fields: List[str] = ["_sa_instance_state"],
     convert_func: List[Callable] = [],
+    datetime_to_str_fmt: str = "%Y-%m-%d %H:%M:%S",
 ):
     """orm 对象转为 dict
 
     exclude_fields: 排除不必要的字段
     convert_func: 进行一些数据操作，如 将 datetime 转换为 timestamp
 
     配合 partial 使用
@@ -118,14 +161,19 @@
 
     obj_dict = obj.__dict__
     for k in exclude_fields:
         if k in obj_dict:
             obj_dict.pop(k)
     for _conver_f in convert_func:
         obj_dict = _conver_f(obj_dict)
+    for column in obj_dict:
+        if isinstance(obj_dict[column], datetime):
+            obj_dict[column] = cast(
+                datetime, obj_dict[column]
+            ).strftime(datetime_to_str_fmt)
     return obj_dict
 
 
 class ColumnType(Generic[C], Column):
     if TYPE_CHECKING:
 
         def __add__(self, some) -> "ColumnType[C]":
@@ -209,15 +257,15 @@
 ) -> ColumnType[str]:
     ...
 
 
 @overload
 def column_field(
     column_type: Union[Type[Boolean], Boolean],
-    primary_key: bool,
+    primary_key: bool = False,
     default=None,
     nullable=None,
     comment=None,
     **kwargs,
 ) -> ColumnType[bool]:
     ...
 
@@ -477,8 +525,8 @@
     @property
     def engines_iter(self):
         for _engine in engines.values():
             yield _engine
 
     async def create_all(self):
         async with engines["master"].begin() as conn:
-            await conn.run_sync(_Base.metadata.create_all)
+            await conn.run_sync(_Base.metadata.create_all)
```

### Comparing `simple_starlette-2.3.2/simple_starlette/db/redis.py` & `simple_starlette-3.0.0/simple_starlette/db/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,17 @@
         db_uri = redis_db_uri or app.config.get("REDIS_DB_URI", None)
         if not db_uri:
             raise AttributeError(
                 "init redis db , the `REDIS_DB_URI` must be set"
             )
         pool = ConnectionPool(host=db_uri, port=redis_port, db=db)
         self.redis = Redis(connection_pool=pool)
+        self.redis.info()
 
         self.__check_connection()
 
     def __check_connection(self):
         try:
-            self.redis.client_info()
+            self.redis.info()
         except redis.exceptions.ConnectionError:
             logger.error("连接redis失败,检查配置，以及确保服务可被访问")
             sys.exit(0)
```

### Comparing `simple_starlette-2.3.2/simple_starlette/dispatch_request.py` & `simple_starlette-3.0.0/simple_starlette/dispatch_request.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/docs/api.py` & `simple_starlette-3.0.0/simple_starlette/docs/api.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/exceptions.py` & `simple_starlette-3.0.0/simple_starlette/exceptions.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/http_client/request_utils.py` & `simple_starlette-3.0.0/simple_starlette/http_client/request_utils.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/include.py` & `simple_starlette-3.0.0/simple_starlette/include.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/logger.py` & `simple_starlette-3.0.0/simple_starlette/logger.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/middleware/cors.py` & `simple_starlette-3.0.0/simple_starlette/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/middleware/rate_limiter.py` & `simple_starlette-3.0.0/simple_starlette/middleware/rate_limiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         self.redis_client = cast(
             Optional[RedisClient], self.options.get("redis_client")
         )
         if self.redis_client:
             self._lock = self.redis_client.redis.lock(
                 "rate_limit_lock_%s" % id(self),
                 timeout=10,
-                blocking=True,
                 blocking_timeout=5,
             )
         else:
             self._lock = threading.Lock()
 
         super().__init__(app, **options)
```

### Comparing `simple_starlette-2.3.2/simple_starlette/middleware/token_auth.py` & `simple_starlette-3.0.0/simple_starlette/middleware/token_auth.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/responses.py` & `simple_starlette-3.0.0/simple_starlette/responses.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/route.py` & `simple_starlette-3.0.0/simple_starlette/route.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette/rpc/json_rpc.py` & `simple_starlette-3.0.0/simple_starlette/rpc/json_rpc.py`

 * *Files identical despite different names*

### Comparing `simple_starlette-2.3.2/simple_starlette.egg-info/PKG-INFO` & `simple_starlette-3.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
-Name: simple-starlette
-Version: 2.3.2
+Name: simple_starlette
+Version: 3.0.0
 Summary: a micro server
-Home-page: UNKNOWN
 Author: asbt
 Author-email: sg5htd@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simple-Starlette
 
 [![License](https://img.shields.io/static/v1?label=asgi&message=starlette&color=red)]()
 [![License](https://img.shields.io/static/v1?label=asgi-server&message=uvicorn&color=green)]()
@@ -67,22 +64,51 @@
 # curl http://localhost:9091/test?arg1=hello&arg2=world
 # response:
 # {"arg1":"hello", "arg2":"world"}
 ```
 查看更多开发使用实例：[example usage](https://github.com/mapyJJJ/simple-starlette/tree/master/example)
 
 ---
-关于框架：   
-目的是整合业界常用的技术选型与各种解决方案的封装，在保证框架稳定性与高性能的前提下，提供快速开发与部署后端项目的能力
-todo：[todo](https://github.com/mapyJJJ/simple-starlette/tree/master/todo.md)
+#### basic:
 
----
+- apis支持: 
+    - `cbv/fbv http api`
+    - `json-rpc`
+    - `tcp-rpc`
+    - `grpc-rpc`
+    - `websocket`
+
+- middleware:
+    - `cors`
+    - `auth jwt+cookie`
+    - `api-rate-limit`
+    - `sentry`
+    - ...(compatible all asgi middleware)
+
+- database:
+    - relational database: `mysql + sqlalchemy`, `postgresql + sqlalchemy`
+    - not noly sql database: `redis`, `mongodb`   
+
+- cache:
+    - ttl: `ttlcache`, `lruttlcache`
+    - guava_cache: `GuavaCache`
+    - redis-cache
+
+- async task(定时，延时执行): 
+    - `simple-async-task`: 
+    - `celery` : 一般架构为(celery+rabbitmq)
+
+- other: 
+    - `simple-api-docs`
+    - `polish query/body params`
+    - `type hint`
 
+---
+各类系统架构template [README](https://github.com/mapyJJJ/simple-starlette/blob/master/system_architecture_template/README.md)
 
 
 ---
 #### LICENSE
 
 [GPL-3.0 License](https://github.com/mapyJJJ/simple-starlette/blob/master/LICENSE)
 
 ---
-
```

### Comparing `simple_starlette-2.3.2/simple_starlette.egg-info/SOURCES.txt` & `simple_starlette-3.0.0/simple_starlette.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 simple_starlette/cache/__init__.py
 simple_starlette/cache/guava_cache.py
 simple_starlette/cache/memory_cache.py
 simple_starlette/cache/redis_cache.py
 simple_starlette/db/__init__.py
 simple_starlette/db/db_sqlalchemy.py
 simple_starlette/db/redis.py
+simple_starlette/db/sqlalchemy_types.py
 simple_starlette/docs/__init__.py
 simple_starlette/docs/api.py
 simple_starlette/http_client/__init__.py
 simple_starlette/http_client/request_utils.py
 simple_starlette/middleware/__init__.py
 simple_starlette/middleware/cors.py
 simple_starlette/middleware/rate_limiter.py
```

