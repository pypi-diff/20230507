# Comparing `tmp/tomcru-0.1.3.tar.gz` & `tmp/tomcru-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomcru-0.1.3.tar", max compression
+gzip compressed data, was "tomcru-0.2.3.tar", max compression
```

## Comparing `tomcru-0.1.3.tar` & `tomcru-0.2.3.tar`

### file list

```diff
@@ -1,101 +1,110 @@
--rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.1.3/LICENSE
--rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.1.3/README.md
--rw-r--r--   0        0        0      632 2023-04-27 10:29:13.203529 tomcru-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      561 2023-04-23 17:44:15.255606 tomcru-0.1.3/tomcru/__init__.py
--rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.1.3/tomcru/appbuilders/envmapping.py
--rw-r--r--   0        0        0     1416 2023-04-27 10:26:11.129112 tomcru-0.1.3/tomcru/appbuilders/faas/InjectableAppBase.py
--rw-r--r--   0        0        0     2954 2023-04-27 10:14:15.984656 tomcru-0.1.3/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/appbuilders/faas/sam_app/__init__.py
--rw-r--r--   0        0        0      848 2023-04-27 10:14:15.980656 tomcru-0.1.3/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
--rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/appbuilders/faas/static_app/__init__.py
--rw-r--r--   0        0        0    10214 2023-04-27 10:27:22.520399 tomcru-0.1.3/tomcru/cfgparsers/BaseCfgParser.py
--rw-r--r--   0        0        0     3076 2023-04-26 23:45:03.858775 tomcru-0.1.3/tomcru/cfgparsers/EnvParser.py
--rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.1.3/tomcru/cfgparsers/MergeCfgParser.py
--rw-r--r--   0        0        0     4746 2023-04-27 01:54:56.413640 tomcru-0.1.3/tomcru/cfgparsers/SwaggerCfgParser.py
--rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.1.3/tomcru/cfgparsers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.1.3/tomcru/core/__init__.py
--rw-r--r--   0        0        0     3524 2023-04-19 21:58:50.454140 tomcru-0.1.3/tomcru/core/cfg/api.py
--rw-r--r--   0        0        0     1284 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/core/cfg/authorizers.py
--rw-r--r--   0        0        0     3605 2023-04-23 18:19:12.194283 tomcru-0.1.3/tomcru/core/cfg/integrations.py
--rw-r--r--   0        0        0     2081 2023-04-26 23:45:03.854775 tomcru-0.1.3/tomcru/core/cfg/proj.py
--rw-r--r--   0        0        0      563 2023-04-27 01:48:19.835005 tomcru-0.1.3/tomcru/core/modloader.py
--rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.1.3/tomcru/core/obj_store.py
--rw-r--r--   0        0        0     2948 2023-04-27 10:13:31.952519 tomcru-0.1.3/tomcru/core/project.py
--rw-r--r--   0        0        0     2252 2023-04-27 01:48:39.354937 tomcru-0.1.3/tomcru/core/servmgr.py
--rw-r--r--   0        0        0     3802 2023-04-25 11:22:05.331979 tomcru-0.1.3/tomcru/core/utils/MyMetaLoader.py
--rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.1.3/tomcru/core/utils/__init__.py
--rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.1.3/tomcru/core/utils/toml_custom.py
--rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.1.3/tomcru/core/utils/yaml_custom.py
--rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.1.3/tomcru/services/ServiceBase.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/__init__.py
--rw-r--r--   0        0        0     4838 2023-04-27 01:49:50.786690 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
--rw-r--r--   0        0        0     1511 2023-04-21 15:39:22.023408 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/apigw_hosted_utils.py
--rw-r--r--   0        0        0      851 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     2718 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
--rw-r--r--   0        0        0     3203 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
--rw-r--r--   0        0        0      727 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
--rw-r--r--   0        0        0      287 2023-04-23 18:04:30.986605 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
--rw-r--r--   0        0        0     3663 2023-04-27 01:48:52.550891 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
--rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
--rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
--rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
--rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
--rw-r--r--   0        0        0     3872 2023-04-27 01:49:37.482736 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
--rw-r--r--   0        0        0     1918 2023-04-23 18:23:35.039805 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
--rw-r--r--   0        0        0     2613 2023-04-27 01:49:29.598764 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
--rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
--rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
--rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
--rw-r--r--   0        0        0     3070 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
--rw-r--r--   0        0        0     1770 2023-04-18 00:10:51.017128 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
--rw-r--r--   0        0        0     3312 2023-04-19 01:27:07.459839 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
--rw-r--r--   0        0        0     3528 2023-04-18 00:10:51.013128 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
--rw-r--r--   0        0        0      185 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
--rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
--rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.1.3/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
--rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.1.3/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-25 19:34:10.268617 tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
--rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/__init__.py
--rw-r--r--   0        0        0      802 2023-04-25 20:07:24.831399 tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/boto3.py
--rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/__init__.py
--rw-r--r--   0        0        0      289 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DdbSqlalchemyAdapter.py
--rw-r--r--   0        0        0     8044 2023-04-21 01:21:56.198102 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DdbTableAdapter.py
--rw-r--r--   0        0        0      697 2023-04-27 10:20:48.798424 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
--rw-r--r--   0        0        0     1133 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
--rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
--rw-r--r--   0        0        0     4076 2023-04-25 22:35:24.903552 tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
--rw-r--r--   0        0        0      779 2023-04-21 01:02:40.764855 tomcru-0.1.3/tomcru/services/aws/hosted/lambda_b/EmeLambdaContext.py
--rw-r--r--   0        0        0     3409 2023-04-27 10:26:11.121112 tomcru-0.1.3/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/hosted/lambda_b/__init__.py
--rw-r--r--   0        0        0     2553 2023-04-27 10:27:22.512399 tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
--rw-r--r--   0        0        0      529 2023-04-25 22:30:36.985428 tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/S3Service.py
--rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/__init__.py
--rw-r--r--   0        0        0     4097 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
--rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/model_checker/__init__.py
--rw-r--r--   0        0        0      790 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
--rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/onpremise/s3_static/__init__.py
--rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/SamTplBuilder.py
--rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/core.yaml
--rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/httpapi.yaml
--rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/integ_normal.yaml
--rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/integ_ws.yaml
--rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/lambda.yaml
--rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/layer.yaml
--rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/template.yaml
--rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/_junk/wsapi.yaml
--rw-r--r--   0        0        0     2120 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
--rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/lambda_b/__init__.py
--rw-r--r--   0        0        0     1363 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/params_b/ParametersBuilder.py
--rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/params_b/__init__.py
--rw-r--r--   0        0        0     2843 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
--rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/__init__.py
--rw-r--r--   0        0        0     1773 2023-04-17 19:28:58.101580 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
--rw-r--r--   0        0        0      790 2023-04-17 18:29:36.248599 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
--rw-r--r--   0        0        0      861 2023-04-17 19:29:32.681461 tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
--rw-r--r--   0        0        0     2326 2023-04-17 18:29:36.252599 tomcru-0.1.3/tomcru/services/general/eme2swagger/Eme2Swagger.py
--rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.1.3/tomcru/services/general/eme2swagger/__init__.py
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-17 18:29:36.244599 tomcru-0.2.3/LICENSE
+-rw-r--r--   0        0        0      183 2023-04-17 18:29:36.244599 tomcru-0.2.3/README.md
+-rw-r--r--   0        0        0      632 2023-05-07 01:40:00.618980 tomcru-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-29 11:53:00.162328 tomcru-0.2.3/tomcru/__init__.py
+-rw-r--r--   0        0        0      885 2023-04-20 17:28:59.003207 tomcru-0.2.3/tomcru/appbuilders/envmapping.py
+-rw-r--r--   0        0        0     1587 2023-04-29 18:55:53.024675 tomcru-0.2.3/tomcru/appbuilders/faas/InjectableAppBase.py
+-rw-r--r--   0        0        0     2936 2023-04-29 11:52:43.934414 tomcru-0.2.3/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/appbuilders/faas/sam_app/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-27 10:14:15.980656 tomcru-0.2.3/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py
+-rw-r--r--   0        0        0       79 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/appbuilders/faas/static_app/__init__.py
+-rw-r--r--   0        0        0     9980 2023-04-29 12:03:31.807647 tomcru-0.2.3/tomcru/cfgparsers/BaseCfgParser.py
+-rw-r--r--   0        0        0     3070 2023-04-29 01:53:19.641911 tomcru-0.2.3/tomcru/cfgparsers/EnvParser.py
+-rw-r--r--   0        0        0     1144 2023-04-20 10:17:05.036609 tomcru-0.2.3/tomcru/cfgparsers/MergeCfgParser.py
+-rw-r--r--   0        0        0     5090 2023-04-29 12:02:36.779844 tomcru-0.2.3/tomcru/cfgparsers/SwaggerCfgParser.py
+-rw-r--r--   0        0        0      322 2023-04-23 19:46:42.543716 tomcru-0.2.3/tomcru/cfgparsers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 19:28:55.917588 tomcru-0.2.3/tomcru/core/__init__.py
+-rw-r--r--   0        0        0     3291 2023-04-29 12:02:24.479889 tomcru-0.2.3/tomcru/core/cfg/api.py
+-rw-r--r--   0        0        0     1244 2023-04-29 11:52:34.470450 tomcru-0.2.3/tomcru/core/cfg/authorizers.py
+-rw-r--r--   0        0        0     3716 2023-04-29 12:01:41.192048 tomcru-0.2.3/tomcru/core/cfg/integrations.py
+-rw-r--r--   0        0        0     2041 2023-04-29 11:52:34.486450 tomcru-0.2.3/tomcru/core/cfg/proj.py
+-rw-r--r--   0        0        0      670 2023-04-29 16:16:10.250867 tomcru-0.2.3/tomcru/core/modloader.py
+-rw-r--r--   0        0        0      833 2023-04-25 19:30:27.561274 tomcru-0.2.3/tomcru/core/obj_store.py
+-rw-r--r--   0        0        0     2989 2023-04-29 17:03:04.510715 tomcru-0.2.3/tomcru/core/project.py
+-rw-r--r--   0        0        0     2227 2023-04-29 16:20:26.534540 tomcru-0.2.3/tomcru/core/servmgr.py
+-rw-r--r--   0        0        0     3802 2023-05-07 01:20:10.626850 tomcru-0.2.3/tomcru/core/utils/MyMetaLoader.py
+-rw-r--r--   0        0        0      104 2023-04-20 13:43:12.977618 tomcru-0.2.3/tomcru/core/utils/__init__.py
+-rw-r--r--   0        0        0     1135 2023-04-20 13:44:18.245442 tomcru-0.2.3/tomcru/core/utils/toml_custom.py
+-rw-r--r--   0        0        0     2462 2023-04-17 18:29:36.252599 tomcru-0.2.3/tomcru/core/utils/yaml_custom.py
+-rw-r--r--   0        0        0       72 2023-05-05 20:11:13.811402 tomcru-0.2.3/tomcru/etc/proxies/aws-sdk/index.js
+-rw-r--r--   0        0        0      261 2023-05-05 20:10:34.172421 tomcru-0.2.3/tomcru/etc/proxies/aws-sdk/package.json
+-rw-r--r--   0        0        0      558 2023-05-05 23:50:53.045569 tomcru-0.2.3/tomcru/etc/proxies/aws-sdk/proxylib.js
+-rw-r--r--   0        0        0      873 2023-05-06 16:59:17.798252 tomcru-0.2.3/tomcru/etc/proxies/aws-sdk/serv/ddb.js
+-rw-r--r--   0        0        0      703 2023-05-06 16:12:42.134096 tomcru-0.2.3/tomcru/etc/proxies/t_proxy.js
+-rw-r--r--   0        0        0      540 2023-04-25 19:12:49.028297 tomcru-0.2.3/tomcru/services/ServiceBase.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 00:05:26.709577 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/__init__.py
+-rw-r--r--   0        0        0     6799 2023-04-29 12:52:25.243899 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/ApiGWBuilderBase.py
+-rw-r--r--   0        0        0        0 2023-04-29 03:09:12.832374 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-29 11:52:34.482450 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     2688 2023-05-01 08:08:53.636339 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py
+-rw-r--r--   0        0        0     3726 2023-05-07 01:32:16.704224 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py
+-rw-r--r--   0        0        0      711 2023-04-29 11:52:34.510450 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py
+-rw-r--r--   0        0        0      322 2023-04-29 03:05:19.325205 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/integration/__init__.py
+-rw-r--r--   0        0        0     4871 2023-05-01 09:27:22.908562 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/ApiGWFlaskBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-21 15:34:30.512217 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py
+-rw-r--r--   0        0        0      213 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/HomeController.py
+-rw-r--r--   0        0        0      236 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/SwaggerController.py
+-rw-r--r--   0        0        0     3897 2023-04-29 11:55:18.949636 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0     1808 2023-04-29 11:52:43.966414 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py
+-rw-r--r--   0        0        0     2553 2023-04-29 11:52:43.966414 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py
+-rw-r--r--   0        0        0      148 2023-04-23 17:59:42.203687 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/integration/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-21 15:34:30.504217 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/ApiGWWebsocketBuilder.py
+-rw-r--r--   0        0        0       97 2023-04-21 15:34:35.936203 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/__init__.py
+-rw-r--r--   0        0        0     2994 2023-04-29 11:52:43.946414 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-29 11:53:00.170328 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py
+-rw-r--r--   0        0        0     3296 2023-04-29 11:52:34.474450 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py
+-rw-r--r--   0        0        0     3510 2023-04-29 11:52:43.962414 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py
+-rw-r--r--   0        0        0      185 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/TomcruApiGWWsIntegration.py
+-rw-r--r--   0        0        0      686 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py
+-rw-r--r--   0        0        0      853 2023-04-25 19:16:13.145908 tomcru-0.2.3/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py
+-rw-r--r--   0        0        0       58 2023-04-23 13:47:38.385293 tomcru-0.2.3/tomcru/services/aws/hosted/apigw_manager_b/__init__.py
+-rw-r--r--   0        0        0     1477 2023-05-07 01:20:36.754727 tomcru-0.2.3/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py
+-rw-r--r--   0        0        0       70 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/hosted/boto3_b/__init__.py
+-rw-r--r--   0        0        0      622 2023-05-03 19:16:05.271285 tomcru-0.2.3/tomcru/services/aws/hosted/boto3_b/boto3.py
+-rw-r--r--   0        0        0     1782 2023-04-29 22:03:41.543858 tomcru-0.2.3/tomcru/services/aws/hosted/cloudfront/flask_b/CloudfrontFlaskBuilder.py
+-rw-r--r--   0        0        0      100 2023-04-29 15:54:06.512215 tomcru-0.2.3/tomcru/services/aws/hosted/cloudfront/flask_b/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:57:16.415271 tomcru-0.2.3/tomcru/services/aws/hosted/ddb/__init__.py
+-rw-r--r--   0        0        0      993 2023-05-04 12:19:56.412205 tomcru-0.2.3/tomcru/services/aws/hosted/ddb/proxy.py
+-rw-r--r--   0        0        0     8598 2023-05-03 19:26:51.189625 tomcru-0.2.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py
+-rw-r--r--   0        0        0      971 2023-05-04 22:52:05.711536 tomcru-0.2.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py
+-rw-r--r--   0        0        0     1133 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py
+-rw-r--r--   0        0        0       79 2023-04-20 17:41:37.808233 tomcru-0.2.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/__init__.py
+-rw-r--r--   0        0        0      355 2023-05-04 22:52:05.707535 tomcru-0.2.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/boto3_proxy.py
+-rw-r--r--   0        0        0     5354 2023-04-29 18:49:25.769803 tomcru-0.2.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/dal_ddb.py
+-rw-r--r--   0        0        0     4400 2023-05-07 01:24:03.213853 tomcru-0.2.3/tomcru/services/aws/hosted/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0      784 2023-05-01 08:27:27.476570 tomcru-0.2.3/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/hosted/lambda_b/__init__.py
+-rw-r--r--   0        0        0     5103 2023-05-06 18:34:46.898263 tomcru-0.2.3/tomcru/services/aws/hosted/lambda_b/proxy/Py2NodeLambdaProxy.py
+-rw-r--r--   0        0        0     2555 2023-04-27 21:53:01.387107 tomcru-0.2.3/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py
+-rw-r--r--   0        0        0      529 2023-04-25 22:30:36.985428 tomcru-0.2.3/tomcru/services/aws/hosted/s3_b/S3Service.py
+-rw-r--r--   0        0        0       61 2023-04-25 22:42:25.629435 tomcru-0.2.3/tomcru/services/aws/hosted/s3_b/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/onpremise/__init__.py
+-rw-r--r--   0        0        0     4043 2023-04-29 11:53:00.190328 tomcru-0.2.3/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py
+-rw-r--r--   0        0        0      121 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/onpremise/model_checker/__init__.py
+-rw-r--r--   0        0        0      782 2023-04-29 11:52:34.530450 tomcru-0.2.3/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py
+-rw-r--r--   0        0        0       78 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/onpremise/s3_static/__init__.py
+-rw-r--r--   0        0        0     7308 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/_junk/SamTplBuilder.py
+-rw-r--r--   0        0        0      841 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/_junk/core.yaml
+-rw-r--r--   0        0        0      855 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/_junk/httpapi.yaml
+-rw-r--r--   0        0        0      372 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/_junk/integ_normal.yaml
+-rw-r--r--   0        0        0      638 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/_junk/integ_ws.yaml
+-rw-r--r--   0        0        0      153 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/_junk/lambda.yaml
+-rw-r--r--   0        0        0      231 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/_junk/layer.yaml
+-rw-r--r--   0        0        0     4389 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/_junk/template.yaml
+-rw-r--r--   0        0        0     1027 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/_junk/wsapi.yaml
+-rw-r--r--   0        0        0     2101 2023-04-29 11:53:00.174328 tomcru-0.2.3/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py
+-rw-r--r--   0        0        0       74 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/lambda_b/__init__.py
+-rw-r--r--   0        0        0     1344 2023-04-29 11:53:00.154328 tomcru-0.2.3/tomcru/services/aws/sam/params_b/ParametersBuilder.py
+-rw-r--r--   0        0        0       85 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/params_b/__init__.py
+-rw-r--r--   0        0        0     2725 2023-04-29 11:53:00.170328 tomcru-0.2.3/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py
+-rw-r--r--   0        0        0       91 2023-04-17 18:29:36.248599 tomcru-0.2.3/tomcru/services/aws/sam/spec_api_b/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-29 11:52:34.502450 tomcru-0.2.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py
+-rw-r--r--   0        0        0      774 2023-04-29 11:52:34.470450 tomcru-0.2.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMOIDCAuthBuilder.py
+-rw-r--r--   0        0        0      835 2023-04-29 11:52:43.962414 tomcru-0.2.3/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py
+-rw-r--r--   0        0        0     2266 2023-04-29 11:52:43.970414 tomcru-0.2.3/tomcru/services/general/eme2swagger/Eme2Swagger.py
+-rw-r--r--   0        0        0       67 2023-04-17 18:29:36.252599 tomcru-0.2.3/tomcru/services/general/eme2swagger/__init__.py
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 tomcru-0.2.3/PKG-INFO
```

### Comparing `tomcru-0.1.3/LICENSE` & `tomcru-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/pyproject.toml` & `tomcru-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomcru"
-version = "0.1.3"
+version = "0.2.3"
 description = "Serverless app framework"
 authors = ["Rajmund Csombordi <rajmund.csombordi@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "tomcru"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tomcru-0.1.3/tomcru/appbuilders/envmapping.py` & `tomcru-0.2.3/tomcru/appbuilders/envmapping.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/appbuilders/faas/InjectableAppBase.py` & `tomcru-0.2.3/tomcru/appbuilders/faas/InjectableAppBase.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,7 +40,10 @@
         utils.cleanup_injects()
 
     def service(self, serv_id):
         return self.p.srvmgr.service(self.env, serv_id)
 
     def object(self, srv, obj_id):
         return self.p.objmgr.get(srv, obj_id)
+
+    def __repr__(self):
+        return f'<InjectableAppBase env={self.env.env_id} target={self.env.target} service_type={self.env.service_type} path={self.env.app_path}>'
```

### Comparing `tomcru-0.1.3/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py` & `tomcru-0.2.3/tomcru/appbuilders/faas/sam_app/SamAppBuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,27 +57,27 @@
         raise NotImplementedError()
 
     def build_app_stack(self, env):
         tpl = {
             'AWSTemplateFormatVersion': '2010-09-09',
             'Transform': 'AWS::Serverless-2016-10-31',
             # todo: add custom description
-            'Description': 'Serverless website',
+            'EP': 'Serverless website',
             'Parameters': {},
             'Globals': {},
             'Resources': {}
             # todo: output
         }
 
         # inject app parameters hier
 
         return tpl
 
     def _sort_keys_tpl(self, tpl):
-        SAM_KEYS_ORDER = ['AWSTemplateFormatVersion', 'Transform', 'Description', 'Parameters', 'Globals', 'Resources']
+        SAM_KEYS_ORDER = ['AWSTemplateFormatVersion', 'Transform', 'EP', 'Parameters', 'Globals', 'Resources']
         # RES_KEYS_ORDER = ['Type', 'Parameters']
         #
         tpl = {k: tpl[k] for k in sorted(tpl, key=lambda x: SAM_KEYS_ORDER.index(x) if x in SAM_KEYS_ORDER else 1000)}
 
         AWSSAM_RES_TYPE_ORDER = [
             'AWS::Serverless::LayerVersion',
             'AWS::Serverless::Function',
```

### Comparing `tomcru-0.1.3/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py` & `tomcru-0.2.3/tomcru/appbuilders/faas/static_app/StaticAppBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/cfgparsers/BaseCfgParser.py` & `tomcru-0.2.3/tomcru/cfgparsers/BaseCfgParser.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from deepmerge import always_merger
 
 from tomcru.core.utils.toml_custom import toml, load_settings, SettingWrapper
 from tomcru.core.utils.yaml_custom import yaml
 
 from ..core.utils.toml_custom import load_settings
-from tomcru import TomcruSubProjectCfg, TomcruRouteDescriptor, TomcruEndpointDescriptor, TomcruApiDescriptor, \
-    TomcruApiLambdaAuthorizerDescriptor, TomcruLambdaIntegrationDescription, TomcruApiAuthorizerDescriptor, \
-    TomcruSwaggerIntegrationDescription, TomcruApiOIDCAuthorizerDescriptor, TomcruMockedIntegrationDescription
+from tomcru import TomcruSubProjectCfg, TomcruRouteEP, TomcruEndpoint, TomcruApiEP, \
+    TomcruApiLambdaAuthorizerEP, TomcruLambdaIntegrationEP, TomcruApiAuthorizerEP, \
+    TomcruSwaggerIntegrationEP, TomcruApiOIDCAuthorizerEP, TomcruMockedIntegrationEP
 
 
 class BaseCfgParser:
     def __init__(self, project, name):
         self.proj = project
         self.name = name
         self.cfg: TomcruSubProjectCfg | None = None
@@ -108,16 +108,16 @@
             cfg = {**cfg_all_, **cfg}
 
             if _api_type == 'rest':
                 raise NotImplementedError("HTTPv1 not supported")
 
             #print(f"Parsing api: {api_name}")
 
-            #cfg_api_ = self.cfg.apis.setdefault(api_name, TomcruApiDescriptor(api_name, _api_type))
-            cfg_api_ = self.cfg.apis[api_name] = TomcruApiDescriptor(api_name, _api_type)
+            #cfg_api_ = self.cfg.apis.setdefault(api_name, TomcruApiEP(api_name, _api_type))
+            cfg_api_ = self.cfg.apis[api_name] = TomcruApiEP(api_name, _api_type)
 
             # map ini to tomcru descriptor
             cfg_api_.swagger_enabled = cfg.get('swagger_enabled', False)
             cfg_api_.swagger_ui = cfg.get('swagger_ui', False)
             cfg_api_.swagger_check_models = cfg.get('swagger_check_models', False)
             cfg_api_.default_authorizer = cfg.get('default_authorizer', None)
             cfg_api_.enabled = cfg.get('enabled', True)
@@ -138,15 +138,15 @@
                 #     self.cfg.authorizers[auth_id] = auth_integ
 
     def add_eme_routes(self, api_name: str, routes: dict, check_files=False, subkey=None):
         # assert integration is not None
         #
         # _api_type = integration
         #
-        cfg_api_ = self.cfg.apis[api_name] #.setdefault(api_name, TomcruApiDescriptor(api_name, _api_type))
+        cfg_api_ = self.cfg.apis[api_name] #.setdefault(api_name, TomcruApiEP(api_name, _api_type))
 
         if not cfg_api_.enabled:
             return
 
         #print(f"Parsing routes: {api_name}.{subkey}")
         for endpoint, integ_opts in routes.items():
             # if endpoint.startswith('#'):
@@ -160,15 +160,15 @@
             else:
                 method, route = endpoint.split(' ')
 
                 endpoint_integ = self._get_integ(api_name, integ_opts, check_files, route, method)
 
                 # add Api Gateway integration
                 if endpoint_integ:
-                    cfg_api_.routes.setdefault(route, TomcruRouteDescriptor(endpoint_integ.route, endpoint_integ.group, api_name))
+                    cfg_api_.routes.setdefault(route, TomcruRouteEP(endpoint_integ.route, api_name))
                     cfg_api_.routes[route].add_endpoint(endpoint_integ)
 
     def parser(self, p):
         return self.subparsers.get(p, None)
 
     def add_layer(self, layer_name, packages=None, /, folder=None, *, in_house=True):
         """
@@ -178,15 +178,15 @@
         :param packages: List of directories (python packages) to be added to the zip file.
         :param folder: Package path
         :param in_house: set true if the layer package is within the project (./layers/ directory)
         :return:
         """
         self.cfg.layers.append((layer_name, packages, folder, in_house))
 
-    def _get_integ(self, api_name, integ_opts, check_files: bool, route, method) -> TomcruEndpointDescriptor | None:
+    def _get_integ(self, api_name, integ_opts, check_files: bool, route, method) -> TomcruEndpoint | None:
         """
 
         :param integ_opts:
         :param check_files:
         :param route:
         :param method:
         :return:
@@ -219,38 +219,38 @@
             if check_files:
                 # check if files exist
                 if not os.path.exists(f'{self.cfg.app_path}/lambdas/{group}/{lamb_name}'):
                     raise Exception(f"Lambda package {self.cfg.app_path}/lambdas/{group}/{lamb_name} doesn't exist")
                     return None
 
             # Lambda integration
-            integ = TomcruLambdaIntegrationDescription(group, route, method, lamb_name, layers, role, auth, integ_opts)
+            integ = TomcruLambdaIntegrationEP(route, method, group, lamb_name, layers, role, auth, integ_opts)
         elif 'swagger' in params:
-            integ = TomcruSwaggerIntegrationDescription('swagger', route, method, params['swagger'])
+            integ = TomcruSwaggerIntegrationEP(route, method, params['swagger'])
         elif 'mocked' in params:
-            integ = TomcruMockedIntegrationDescription(params.get('group', 'Mocked'), route, method, params['mocked'])
+            integ = TomcruMockedIntegrationEP(route, method, params['mocked'])
         else:
             raise Exception(f"Integration not recognized!")
 
         return integ
 
-    def _get_auth_integ(self, auth_id, integ_opt) -> TomcruApiAuthorizerDescriptor | None:
+    def _get_auth_integ(self, auth_id, integ_opt) -> TomcruApiAuthorizerEP | None:
         if not integ_opt:
             return None
         params = self._parse_linear_params(integ_opt)
 
         if 'lambda' in params:
             lambda_source, lambda_id = params['lambda'].split('/')
 
-            return TomcruApiLambdaAuthorizerDescriptor(auth_id, lambda_id, lambda_source)
+            return TomcruApiLambdaAuthorizerEP(auth_id, lambda_id, lambda_source)
         elif 'oidc' in params:
             audience = params.get('audience')
             scopes = params.get('scopes')
 
-            return TomcruApiOIDCAuthorizerDescriptor(auth_id, params['oidc'], audience, scopes)
+            return TomcruApiOIDCAuthorizerEP(auth_id, params['oidc'], audience, scopes)
         else:
             pass
         raise NotImplementedError("auth")
 
     def _parse_linear_params(self, line: list):
         if isinstance(line, str):
             if ',' in line:
```

### Comparing `tomcru-0.1.3/tomcru/cfgparsers/EnvParser.py` & `tomcru-0.2.3/tomcru/cfgparsers/EnvParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,19 @@
         for root, dirs, files in os.walk(basepath):
             root_dirname = os.path.basename(root)
 
             if 'envvars' == root_dirname:
                 # load envvars
                 for file in files:
                     envvars_wrap = toml.load(os.path.join(root, file))
+                    envcfg.global_envvars.update(envvars_wrap.pop('__ALL__', {}))
 
                     if 'lambdas' in envvars_wrap:
                         envvar_groups = unflatten_1lv(flatten(envvars_wrap['lambdas'], separator='/'))
 
-                        envcfg.global_envvars.update(envvar_groups.pop('__ALL__', {}))
-
                         for lambda_id, envvars in envvar_groups.items():
                             envcfg.envvars_lamb[lambda_id].update(envvars)
             else:
                 # other configs are loaded as service specifiers
                 for file in filter(lambda f: f.endswith('.toml'), files):
                     if file == 'tomcru.toml':
                         continue
```

### Comparing `tomcru-0.1.3/tomcru/cfgparsers/MergeCfgParser.py` & `tomcru-0.2.3/tomcru/cfgparsers/MergeCfgParser.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/cfgparsers/SwaggerCfgParser.py` & `tomcru-0.2.3/tomcru/cfgparsers/SwaggerCfgParser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,120 @@
 import os
 
 #from apispec import APISpec
-from prance import ResolvingParser, BaseParser
+from prance import ResolvingParser, BaseParser, ValidationError
 
-from tomcru import TomcruSubProjectCfg, TomcruRouteDescriptor, TomcruEndpointDescriptor, TomcruApiDescriptor, \
-    TomcruApiLambdaAuthorizerDescriptor, TomcruLambdaIntegrationDescription, TomcruApiAuthorizerDescriptor, TomcruApiOIDCAuthorizerDescriptor
+from tomcru import TomcruSubProjectCfg, TomcruRouteEP, TomcruEndpoint, TomcruApiEP, \
+    TomcruApiLambdaAuthorizerEP, TomcruLambdaIntegrationEP, TomcruMockedIntegrationEP, TomcruApiOIDCAuthorizerEP
 
 
 class SwaggerCfgParser:
     def __init__(self, cfgparser, name):
         self.name = name
         self.cfg: TomcruSubProjectCfg | None = None
 
     def add_cfg(self, cfg):
         self.cfg = cfg
 
     def add(self, file, check_files=False):
         if not os.path.exists(file): raise Exception("File doesnt exist: " + file)
 
-        f_resolved = ResolvingParser(file)
+        try:
+            f_resolved = ResolvingParser(file)
+        except ValidationError as e:
+            print("prance.ValidationError:")
+            #errors = e.args[4]
+            raise e
+            exit()
 
         f = BaseParser(file)
         # spec = APISpec(
         #     title=f.specification['info']['title'],
         #     version=f.specification['info']['version'],
         #     openapi_version=f.semver,
         #     info=dict(f.specification['info']),
         # )
         api_name = f.specification['info']['title']
 
         # specification = yaml_utils.load_yaml_from_docstring(content)
         # #specification = yaml_utils.load_operations_from_docstring()
-        cfg_api_ = self.cfg.apis.setdefault(api_name, TomcruApiDescriptor(api_name, 'http'))
+        cfg_api_ = self.cfg.apis.setdefault(api_name, TomcruApiEP(api_name, 'http'))
         # cfg_api_.spec = {k: f.specification[k] for k in sorted(f.specification)} # add dict in key order
         # cfg_api_.spec_resolved_schemas = {k: f_resolved.specification[k] for k in sorted(f_resolved.specification)}
         cfg_api_.spec = dict(f.specification) # add dict in key order
         cfg_api_.spec_resolved_schemas = dict(f_resolved.specification)
         cfg_api_.swagger_file = file
 
         # if not cfg_api_.enabled:
         #     return
-        components = f.specification.get('components', {})
+        components = f_resolved.specification.get('components', {})
 
         # parse authorizers
         if 'securitySchemes' in components:
             for auth_id, auth_spec in components['securitySchemes'].items():
                 auth = self._get_authorizer(auth_id, auth_spec)
                 self.cfg.authorizers[auth_id] = auth
 
-        default_auth = next(iter(self.cfg.authorizers)) if len(self.cfg.authorizers)==1 else None
+        default_auth = self.cfg.authorizers.get(cfg_api_.default_authorizer)
+
+        # integ opts refs
+        # _integ_opts_ref = f.specification['components'].pop('x-integ-opts')
 
         # parse endpoints
-        for route, path in f.specification['paths'].items():
-            #group = route.replace('/', '_').strip('_')
+        for route, path in f_resolved.specification['paths'].items():
+            default_group = route.replace('/', '_').strip('_')
 
             for method, operation in path.items():
                 method = method.upper()
-                auth = operation.pop('x-auth', default_auth)
-                integ: TomcruEndpointDescriptor
-
+                integ: TomcruEndpoint
                 integ_opts = operation.pop('x-integ', {})
-                if integ_opts:
-                    if integ_opts['type'] != 'lambda':
-                        raise NotImplementedError("")
-
-                    # parse lambda integration
-                    group, lamb, role, layers = self._get_lambda(integ_opts)
 
-                    integ = TomcruLambdaIntegrationDescription(group, route, method, lamb, layers, role, auth, integ_opts)
+                if not integ_opts:
+                    continue
+                # if '$ref' in integ_opts:
+                #     print("!!!!!!!!!!!", method, integ_opts)
+                #     continue
+
+                # parse lambda integration
+                auth = integ_opts.pop('auth', default_auth)
+                role = integ_opts.pop('role', None)
+
+                # todo: support more integration types
+                if integ_opts['type'] == 'lambda':
+                    layers = integ_opts.pop('layers', [])
+                    group, lamb = integ_opts.pop('lambda-id').split('/')
+
+                    integ = TomcruLambdaIntegrationEP(route, method, group, lamb, layers, role, auth, integ_opts)
+                elif integ_opts['type'] == 'mocked':
+                    example = None
+
+                    integ = TomcruMockedIntegrationEP(route, method, operation['operationId'], integ_opts.get('file'), example)
+                else:
+                    raise NotImplementedError(integ_opts.get('type'))
 
                 # subset of the swagger is referenced from the tomcru cfg so that it can be modified for SAM building
                 integ.spec_ref = operation
 
-                cfg_api_.routes.setdefault(route, TomcruRouteDescriptor(route, group, api_name))
+                cfg_api_.routes.setdefault(route, TomcruRouteEP(route, api_name))
                 cfg_api_.routes[route].add_endpoint(integ)
 
     def _get_authorizer(self, auth_id, spec: dict):
 
         if spec['type'] == 'apiKey':
             # todo: is it possible to define non-lambda for this auth type?
             group, lambda_id, role, layers = self._get_lambda(spec.pop('x-lambda'))
             _in = spec.get('in', 'header')
             _name = spec.get('name', 'Authorization')
 
-            return TomcruApiLambdaAuthorizerDescriptor(auth_id, lambda_id, group, _in, _name)
+            return TomcruApiLambdaAuthorizerEP(auth_id, lambda_id, group, _in, _name)
         elif spec['type'] == 'openIdConnect':
             # openapi3 doesn't allow in/name for openIdConnect, so authorization header is set static
 
             # oidc endpoint is going to be redundant because SAM also requires it
             endpoint = spec['openIdConnectUrl']
             oidc_cfg = spec.pop('x-oidc')
 
-            return TomcruApiOIDCAuthorizerDescriptor(auth_id, endpoint, oidc_cfg.get('audience'), oidc_cfg.get('scopes'))
+            return TomcruApiOIDCAuthorizerEP(auth_id, endpoint, oidc_cfg.get('audience'), oidc_cfg.get('scopes'))
         elif spec['type'] == 'oauth2':
             raise NotImplementedError("we don't know how to implement this LOL")
         else:
             raise NotImplementedError("")
-
-    def _get_lambda(self, lamb):
-        role, layers = None, []
-
-        if isinstance(lamb, dict):
-            lamb, role, layers = lamb['lambda-id'], lamb.get('role'), lamb.get('layers')
-        elif not isinstance(lamb, str):
-            raise Exception("Lambda integration as array not supported")
-
-        # fetch endpoint
-        group, integ_id = lamb.split('/')
-        return group, integ_id, role, layers
```

### Comparing `tomcru-0.1.3/tomcru/core/cfg/api.py` & `tomcru-0.2.3/tomcru/core/cfg/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from collections import defaultdict
 from typing import List, Dict, Set
 
-from .authorizers import TomcruApiAuthorizerDescriptor
-from .integrations import TomcruEndpointDescriptor
+from .authorizers import TomcruApiAuthorizerEP
+from .integrations import TomcruEndpoint
 
 
 
-class TomcruApiDescriptor:
+class TomcruApiEP:
     def __init__(self, api_name, api_type):
         """
 
         :param api_name:
         :param api_type:
         """
         self.api_name = api_name
         self.api_type = api_type # http | ws | rest
 
         # Api configuration:
         self.enabled = True
-        self.routes: Dict[str, TomcruRouteDescriptor] = {}
+        self.routes: Dict[str, TomcruRouteEP] = {}
         #self.authorizers: Set[str] = set()
 
         # OpenApi spec dict
         self.spec: dict | None = None
         self.spec_resolved_schemas: dict | None = None
         self.swagger_enabled = False
         self.swagger_ui = False
@@ -30,15 +30,15 @@
         self.swagger_check_models = None
 
         # default integration values
         self.default_authorizer = None
         self.default_role = None
         self.default_layers = []
 
-    def update(self, api: 'TomcruApiDescriptor'):
+    def update(self, api: 'TomcruApiEP'):
         if api.enabled is not None:
             self.enabled = api.enabled
 
         if self.api_name != api.api_name:
             raise f"Api name mismatch in update(): {self.api_name} != {api.api_name}"
         if self.api_type != api.api_type:
             raise f"Api name mismatch in update(): {self.api_type} != {api.api_type}"
@@ -50,47 +50,44 @@
         print('@TODO: merge self.swagger_file = api.swagger_file')
         print('@TODO: merge self.swagger_check_models = api.swagger_check_models')
         print('@TODO: merge self.default_authorizer = api.default_authorizer')
         print('@TODO: merge self.default_role = api.default_role')
         print('@TODO: merge self.default_layers = api.default_layers')
 
         # additive merge, not override
-        route: TomcruRouteDescriptor
+        route: TomcruRouteEP
         for route_uri, route in api.routes.items():
             if route_uri in self.routes:
                 self.routes[route_uri].update(route)
             else:
                 self.routes[route_uri] = route
 
     def __repr__(self):
         return f'<{self.__class__.__name__} {self.api_type.upper()} - {self.api_name}>'
 
 
-class TomcruRouteDescriptor:
+class TomcruRouteEP:
 
-    def __init__(self, route, group, api_name):
+    def __init__(self, route, api_name):
         """
 
         :param route:
         :param group:
         :param api_name:
         """
         self.api_name = api_name
-        self.group = group
         self.route = route
-        self.endpoints: List[TomcruEndpointDescriptor] = []
+        self.endpoints: List[TomcruEndpoint] = []
 
     def add_endpoint(self, ep):
         self.endpoints.append(ep)
 
-    def update(self, route: 'TomcruRouteDescriptor'):
+    def update(self, route: 'TomcruRouteEP'):
         if self.api_name != route.api_name:
             raise f"Route api name mismatch in update(): {self.api_name} != {route.api_name}"
-        if self.group != route.group:
-            raise f"Route group mismatch in update(): {self.group} != {route.group}"
         if self.route != route.route:
             raise f"Route route mismatch in update(): {self.route} != {route.route}"
 
         # additive merge, not override, but drop redundancies
         s = set()
         s.update(route.endpoints)
         s.update(self.endpoints)
```

### Comparing `tomcru-0.1.3/tomcru/core/cfg/authorizers.py` & `tomcru-0.2.3/tomcru/core/cfg/authorizers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 
 
-class TomcruApiAuthorizerDescriptor:
+class TomcruApiAuthorizerEP:
     def __init__(self, auth_id, auth_type, integ_id):
         """
         Describes authorizer for an API
 
         :param auth_type: lambda, lambda_external, iam, jwt
         :param integ_id: lambda name OR lambda ARN OR iam ARN OR jwt url
         """
         self.auth_id = auth_id
         self.auth_type = auth_type
         self.integ_id = integ_id
 
 
-class TomcruApiLambdaAuthorizerDescriptor(TomcruApiAuthorizerDescriptor):
+class TomcruApiLambdaAuthorizerEP(TomcruApiAuthorizerEP):
     def __init__(self, auth_id, lambda_id, lambda_source, src_in = None, src_name = None):
         """
 
         :param auth_type:
         :param lambda_id:
         """
         super().__init__(auth_id, 'lambda', lambda_id)
@@ -27,15 +27,15 @@
         self.src_in = src_in
 
     @property
     def lambda_id(self):
         return self.lambda_source+'/'+self.integ_id
 
 
-class TomcruApiOIDCAuthorizerDescriptor(TomcruApiAuthorizerDescriptor):
+class TomcruApiOIDCAuthorizerEP(TomcruApiAuthorizerEP):
     def __init__(self, auth_id, endpoint, audience, scopes):
         """
 
         :param auth_type:
         :param integ_id:
         """
         super().__init__(auth_id, 'oidc', endpoint)
```

### Comparing `tomcru-0.1.3/tomcru/core/cfg/integrations.py` & `tomcru-0.2.3/tomcru/core/cfg/integrations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 
 
-class TomcruEndpointDescriptor:
+class TomcruEndpoint:
 
-    def __init__(self, group, route, method, auth=None, opts=None):
+    def __init__(self, route, method, auth=None, opts=None):
         """
 
         :param group:
         :param route:
         :param method:
         """
         self.route: str = route
         self.method: str = method
-        self.group = group
         self.auth = auth
         self.integ_opts = opts if opts is not None else {}
 
         self.spec_ref: dict | None = None
 
         # self.integration: TomcruEndpointIntegration
         # self.lamb: str = lamb
@@ -32,55 +31,57 @@
 
     def __eq__(self, other):
         return self.__hash__() == other.__hash__()
 
     @property
     def endpoint_id(self):
         # eme-like endpoint id (group & method name from lambda)
-        return f'{self.group}:{self.method.lower()}_{self.integ_id}'
+        return f'{self.route}:{self.method.lower()}_{self.integ_id}'
 
     @staticmethod
-    def get_endpoint_id(group, method, integ_id):
-        # eme-like endpoint id (group & method name from lambda)
-        return f'{group}:{method.lower()}_{integ_id}'
+    def get_endpoint_id(route, method, integ_id):
+        # eme-like endpoint id (route & method name from lambda)
+        return f'{route}:{method.lower()}_{integ_id}'
 
     @property
     def is_http(self):
         return not self.method or self.method == 'ws'
 
     @property
     def endpoint(self):
         return self.route
 
     @property
     def _tomcru_json_serializer(self):
         return self.endpoint_id
 
-class TomcruLambdaIntegrationDescription(TomcruEndpointDescriptor):
 
-    def __init__(self, group, route, method, lamb_name, layers, role, auth, opts):
+class TomcruLambdaIntegrationEP(TomcruEndpoint):
+
+    def __init__(self, route, method, group, lamb_name, layers, role, auth, opts):
         """
 
-        :param group:
         :param route:
         :param method:
-        :param lamb_name:
-        :param layers:
-        :param role:
-        :param auth:
+        :param group: lambda group (parent directory)
+        :param lamb_name: lambda name (lambda's directory name)
+        :param layers: lambda layers attached
+        :param role: execution role
+        :param auth: authorizer attached
         """
-        super().__init__(group, route, method, auth, opts)
+        super().__init__(route, method, auth, opts)
 
+        self.group = group
         self.lamb = lamb_name
         self.layers = layers
         self.role = role
 
     @property
     def integ_id(self):
-        return self.lamb
+        return self.lambda_id
 
     @property
     def method_name(self):
         return f'{self.method.lower()}_{self.integ_id}'
 
     @property
     def lambda_id(self):
@@ -88,24 +89,23 @@
 
     def __iter__(self):
         yield self.lamb
         yield self.layers
         yield self.role
 
 
-class TomcruSwaggerIntegrationDescription(TomcruEndpointDescriptor):
-    def __init__(self, group, route, method, type):
+class TomcruSwaggerIntegrationEP(TomcruEndpoint):
+    def __init__(self, route, method, type):
         """
 
-        :param group:
         :param route:
         :param method:
         :param type:
         """
-        super().__init__(group, route, method, None)
+        super().__init__(route, method, None)
 
         self.type = type
         if self.type == 'spec':
             _, req_content = os.path.splitext(self.route)
             self.req_content = req_content.lstrip('.')
         elif self.type == 'ui':
             self.req_content = 'html'
@@ -117,27 +117,29 @@
         return self.type + '_' + self.req_content
 
     @property
     def method_name(self):
         return f'{self.method.lower()}_{self.integ_id}'
 
 
-class TomcruMockedIntegrationDescription(TomcruEndpointDescriptor):
-    def __init__(self, group, route, method, filename):
+class TomcruMockedIntegrationEP(TomcruEndpoint):
+    def __init__(self, route, method, operationId, file, example):
         """
 
-        :param group:
         :param route:
         :param method:
-        :param filename:
+        :param resp:
         """
-        super().__init__(group, route, method, None)
+        super().__init__(route, method, None)
 
-        self.filename = filename
+        self.file = file
+        self.exmple = example
+        self.source = 'file' if file else 'example'
+        self.operationId = operationId
 
     @property
     def integ_id(self):
-        return os.path.basename(self.filename)
+        return os.path.basename(self.operationId)
 
     @property
     def method_name(self):
         return f'{self.method.lower()}_{self.integ_id}'
```

### Comparing `tomcru-0.1.3/tomcru/core/cfg/proj.py` & `tomcru-0.2.3/tomcru/core/cfg/proj.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os.path
 from collections import defaultdict
 
-from .api import TomcruApiAuthorizerDescriptor, TomcruApiDescriptor
+from .api import TomcruApiAuthorizerEP, TomcruApiEP
 from ..utils.toml_custom import SettingWrapper
 
 
 class TomcruProjectCfg:
     def __init__(self):
-        self.apis: dict[str, TomcruApiDescriptor] = {}
-        self.authorizers: dict[str, TomcruApiAuthorizerDescriptor] = {}
+        self.apis: dict[str, TomcruApiEP] = {}
+        self.authorizers: dict[str, TomcruApiAuthorizerEP] = {}
 
         self.layers = []
         self.services: dict[str, SettingWrapper] = {}
 
     def update(self, cfg: 'TomcruProjectCfg'):
         self.authorizers.update(cfg.authorizers)
 
         self.layers.extend(cfg.layers)
 
         # additive merge, not override
-        api: TomcruApiDescriptor
+        api: TomcruApiEP
         for api_name, api in cfg.apis.items():
             if api_name in self.apis:
                 self.apis[api_name].update(api)
             else:
                 self.apis[api_name] = api
 
         for serv_id, serv_cfg in cfg.services.items():
```

### Comparing `tomcru-0.1.3/tomcru/core/obj_store.py` & `tomcru-0.2.3/tomcru/core/obj_store.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/core/project.py` & `tomcru-0.2.3/tomcru/core/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from deprecated import deprecated
 
 from .obj_store import ObjStore
 from .servmgr import ServiceManager
 from ..appbuilders.envmapping import map_env_to_appbuilder
 from ..cfgparsers import BaseCfgParser, _parsers
 from .cfg.proj import TomcruSubProjectCfg, TomcruEnvCfg
 from ..appbuilders.faas.InjectableAppBase import InjectableAppBase
@@ -62,34 +61,34 @@
             _cfg = self.cfg if cfg_id is None else self.cfgs[cfg_id]
 
             # todo: itt: return EnvAppBuilder
             _env = map_env_to_appbuilder(self, _cfg, self.envcfgs[env_id])
             self.envs[env_id] = _env
 
         return _env
-
-    @deprecated("Don't call services from the project, instead use environment")
-    def serv(self, name):
-        env = self.find_env_from_legacy_name(name)
-
-        # load service into cache; cfg
-        return self.env(env.env_id).serv(name)
-
-    @deprecated("Don't call services from the project, instead use environment")
-    def find_env_from_legacy_name(self, name) -> TomcruEnvCfg:
-        n = name.split(':')
-        vendor, target, service_id = n
-        if not target:
-            target = ''
-        if not vendor:
-            vendor = 'general'
-
-        if target == 'onpremise':
-            # @note: hosted frameworks were incorrectly labeled as onpremise
-            target = 'hosted'
-
-        env: TomcruEnvCfg = next(filter(lambda env: env.target == target and vendor in env.vendors, self.envcfgs.values()), None)
-
-        if env is None:
-            raise Exception(f"Service not found: {name}")
-
-        return env
+    #
+    # @deprecated("Don't call services from the project, instead use environment")
+    # def serv(self, name):
+    #     env = self.find_env_from_legacy_name(name)
+    #
+    #     # load service into cache; cfg
+    #     return self.env(env.env_id).serv(name)
+    #
+    # @deprecated("Don't call services from the project, instead use environment")
+    # def find_env_from_legacy_name(self, name) -> TomcruEnvCfg:
+    #     n = name.split(':')
+    #     vendor, target, service_id = n
+    #     if not target:
+    #         target = ''
+    #     if not vendor:
+    #         vendor = 'general'
+    #
+    #     if target == 'onpremise':
+    #         # @note: hosted frameworks were incorrectly labeled as onpremise
+    #         target = 'hosted'
+    #
+    #     env: TomcruEnvCfg = next(filter(lambda env: env.target == target and vendor in env.vendors, self.envcfgs.values()), None)
+    #
+    #     if env is None:
+    #         raise Exception(f"Service not found: {name}")
+    #
+    #     return env
```

### Comparing `tomcru-0.1.3/tomcru/core/servmgr.py` & `tomcru-0.2.3/tomcru/core/servmgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
                 module_name = target_solution + '_b'
             else:
                 module_name = serv_id + '_b'
 
             # load service config
             search_path = os.path.join(pck_path, 'services', env.vendors[0], *target)
 
-            # @TODO: ITT
             # try:
             srv_builder = load_serv(search_path, module_name, debug=self.p.debug)
                 # print("        OKOK", module_name, search_path)
             # except ModuleNotFoundError:
             #     print("        NOK", module_name, search_path)
             #    raise Exception("Service not found: " + module_name)
```

### Comparing `tomcru-0.1.3/tomcru/core/utils/MyMetaLoader.py` & `tomcru-0.2.3/tomcru/core/utils/MyMetaLoader.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/core/utils/toml_custom.py` & `tomcru-0.2.3/tomcru/core/utils/toml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/core/utils/yaml_custom.py` & `tomcru-0.2.3/tomcru/core/utils/yaml_custom.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/ServiceBase.py` & `tomcru-0.2.3/tomcru/services/ServiceBase.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/integration/ExternalLambdaAuthorizerIntegration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
 
 from .TomcruApiGWHttpIntegration import TomcruApiGWAuthorizerIntegration
-from tomcru import TomcruApiLambdaAuthorizerDescriptor
+from tomcru import TomcruApiLambdaAuthorizerEP
 
 
 class ExternalLambdaAuthorizerIntegration(TomcruApiGWAuthorizerIntegration):
-    def __init__(self, cfg: TomcruApiLambdaAuthorizerDescriptor, apigw_cfg: dict):
+    def __init__(self, cfg: TomcruApiLambdaAuthorizerEP, apigw_cfg: dict):
         super().__init__(cfg)
         self.cfg = cfg
 
         group, lamb = cfg.lambda_id.split('/')
 
         auth_resp_path = apigw_cfg['__fileloc__']
         with open(os.path.join(auth_resp_path, lamb+'_mock.json')) as fh:
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/integration/LambdaAuthorizerIntegration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .TomcruApiGWHttpIntegration import TomcruApiGWAuthorizerIntegration
-from tomcru import TomcruApiLambdaAuthorizerDescriptor
+from tomcru import TomcruApiLambdaAuthorizerEP
 
 
 class LambdaAuthorizerIntegration(TomcruApiGWAuthorizerIntegration):
 
-    def __init__(self, cfg: TomcruApiLambdaAuthorizerDescriptor, auth_cfg, lambda_builder, env=None):
+    def __init__(self, cfg: TomcruApiLambdaAuthorizerEP, auth_cfg, lambda_builder, env=None):
         super().__init__(cfg)
 
         self.lambda_builder = lambda_builder
 
         self.lambda_folder = cfg.lambda_source
         self.lambda_id = cfg.lambda_id
         self.env = env
@@ -22,15 +22,15 @@
             self.source = 'queryStringParameters'
         else:
             self.source += 's'
 
         if self.source == 'cookies':
             raise NotImplementedError("Cookies are not yet supported in tomcru authorization (in local FaaS)")
 
-        self.lambda_builder.build_lambda(self.lambda_id, env=self.env)
+        self.lambda_builder.build_lambda(self.lambda_id)
 
     def authorize(self, event: dict):
         """
         Runs lambda
 
         :param event: api gw integration events
         :param source: provided source of authorization token (headers | params | body)
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/integration/OIDCAuthorizerIntegration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import jwt
-
 import requests
 
 from .TomcruApiGWHttpIntegration import TomcruApiGWAuthorizerIntegration
-from tomcru import TomcruApiOIDCAuthorizerDescriptor
+from tomcru import TomcruApiOIDCAuthorizerEP
 
 class AWSOIDCException(Exception):
     pass
 
 
 class OIDCAuthorizerIntegration(TomcruApiGWAuthorizerIntegration):
 
-    def __init__(self, cfg: TomcruApiOIDCAuthorizerDescriptor, auth_cfg, env=None):
+    def __init__(self, cfg: TomcruApiOIDCAuthorizerEP, auth_cfg, env=None):
         super().__init__(cfg)
         self.env = env
 
         self.oidc_ep = cfg.endpoint_url
         self.audience = cfg.audience
         self.scopes = cfg.scopes # this is redundant (scopes_supported is fetched from OIDC ep); but AWS requires to be checked
 
@@ -32,16 +31,24 @@
             return None
         token_jwt: str = event['headers']['authorization'].removeprefix('Bearer ')
 
         try:
             # base64 decode JWT & get JWK for it
             signing_key = self.jwks_client.get_signing_key_from_jwt(token_jwt)
 
+            # force convert to bytes (pyjwt has a bug of type mismatch between cryptography's _RSAPublicKey vs its own RSAPublicKey...)
+            from cryptography.hazmat.primitives import serialization
+            from cryptography.hazmat.primitives.hashes import SHA256, HashAlgorithm
+
+
+            pem = signing_key.key.public_bytes(encoding=serialization.Encoding.PEM,
+                                         format=serialization.PublicFormat.PKCS1)
+
             # verify JWT
-            data = jwt.decode(token_jwt, signing_key.key, algorithms=["RS256"], audience=self.audience, issuer=self.issuer)
+            data = jwt.decode(token_jwt, pem, algorithms=["RS256"], audience=self.audience, issuer=self.issuer)
             #headers = jwt.get_unverified_header(token_jwt)
             # jwk = next(filter(lambda x: x['kid'] == kid, jwks))
 
             scopes = self.verify_claims(data)
 
             if data:
                 # integrate into event
@@ -50,14 +57,15 @@
                         'claims': data,
                         'scopes': scopes
                     }
                 }
 
             return data
         except (jwt.InvalidTokenError, AWSOIDCException) as e:
+            raise e
             # invalidated claims -> authorizer refuses the token
             print("Auth error: ", e)
             return None
 
     def verify_claims(self, data: dict):
         # TODO: ITT: what other stuff we need to check that JWT lib doesn't?
         _scope = data.get('scp', data.get('scope', None))
@@ -77,14 +85,15 @@
         # fetch OIDC endpoint and find JWKS
         headers = {'Accept': 'application/json'}
         try:
             r = requests.get(self.oidc_ep, headers=headers)
         except requests.exceptions.ConnectionError:
             raise AWSOIDCException()
 
+        # TODO: ITT: how to refer to localhost instead of pythonanywhere?
         if r.status_code != 200:
             raise AWSOIDCException()
         oidc = r.json()
 
         self.issuer = oidc['issuer']
         self.scopes_supported = oidc['scopes_supported']
         # validate: The token must include at least one of the scopes in the route's authorizationScopes
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/api_shared/integration/TomcruApiGWHttpIntegration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from abc import ABCMeta, abstractmethod
 
-from tomcru import TomcruApiAuthorizerDescriptor
+from tomcru import TomcruApiAuthorizerEP
 
 
 class TomcruApiGWHttpIntegration(metaclass=ABCMeta):
 
     @abstractmethod
     def on_request(self, **kwargs):
         raise NotImplementedError()
 
 
 class TomcruApiGWAuthorizerIntegration(metaclass=ABCMeta):
 
-    def __init__(self, cfg: TomcruApiAuthorizerDescriptor):
+    def __init__(self, cfg: TomcruApiAuthorizerEP):
         self.cfg = cfg
         self.authorizers_cache = {}
 
     def get_cache(self, cache_key):
         return self.authorizers_cache.get(cache_key) if cache_key else None
 
     def set_cache(self, cache_key, cache_result):
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/controllers/EmeProxyController.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/integration/LambdaIntegration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from flask import request, Response, jsonify
 
 from tomcru.services.aws.hosted.apigw.api_shared.integration import TomcruApiGWHttpIntegration, \
     LambdaAuthorizerIntegration
-from tomcru import TomcruApiDescriptor, TomcruLambdaIntegrationDescription, TomcruEndpointDescriptor
+from tomcru import TomcruApiEP, TomcruLambdaIntegrationEP, TomcruEndpoint
 
 
 base_headers = {
     "content-type": "application/json"
 }
 
 
 class LambdaIntegration(TomcruApiGWHttpIntegration):
 
-    def __init__(self, endpoint: TomcruLambdaIntegrationDescription, auth: LambdaAuthorizerIntegration, lambda_builder, env=None):
+    def __init__(self, endpoint: TomcruLambdaIntegrationEP, auth: LambdaAuthorizerIntegration, lambda_builder, env=None):
         self.endpoint = endpoint
         self.auth_integ = auth
         self.lambda_builder = lambda_builder
         self.env = env
 
         self.lambda_builder.build_lambda(endpoint.lambda_id)
 
@@ -42,15 +42,15 @@
                 "protocol": "HTTP/1.1",
                 #"httpMethod": self.endpoint.method,
                 "http": {
                     "method": self.endpoint.method,
                     "routeKey": route_key
                 },
             },
-            'body': request.data,
+            'body': request.data.decode('utf8'),
             'queryStringParameters': dict(request.args),
             'headers': dict((k.lower(), v) for k, v in request.headers.items()),
             'pathParameters': dict(request.view_args) | kwargs
         }
 
         # apply request parameters transformation
         if hasattr(self.endpoint, 'integ_opts') and 'requestParameters' in self.endpoint.integ_opts:
@@ -67,15 +67,16 @@
                 elif id_to.startswith('path'): src_to = event['pathParameters']
                 else: raise Exception(id_to)
 
                 # todo: process list
                 args_from = next(iter(id_from.split('.')[1:]))
                 args_to = next(iter(id_to.split('.')[1:]))
 
-                src_to[args_to] = src_from[args_from]
+                if args_from in src_from:
+                    src_to[args_to] = src_from[args_from]
 
         return event
 
     def parse_response(self, content: dict):
         """
         Parses HTTP lambda integration's response to flask response
         :param resp: lambda integration response (2.0 format)
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/integration/MockedIntegration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 import json
 
-from flask import request, Response, jsonify
+from flask import request, jsonify, Response
 
 from .LambdaIntegration import LambdaIntegration
-from tomcru import TomcruMockedIntegrationDescription
+from tomcru import TomcruMockedIntegrationEP
 from tomcru.services.aws.hosted.apigw.api_shared.integration.TomcruApiGWHttpIntegration import TomcruApiGWAuthorizerIntegration
 
 
 from tomcru_jerry.mockapi import transform_response
 
 
 base_headers = {
     "content-type": "application/json"
 }
 
 
 class MockedIntegration(LambdaIntegration):
 
-    def __init__(self, endpoint: TomcruMockedIntegrationDescription, auth: TomcruApiGWAuthorizerIntegration, filename: str, env=None):
+    def __init__(self, endpoint: TomcruMockedIntegrationEP, auth: TomcruApiGWAuthorizerIntegration, response: dict, env=None):
         self.endpoint = endpoint
         self.auth_integ = auth
         self.env = env
-        self.resp_tpls = {}
 
-        # todo: support yaml & toml for mocked api?
-        with open(filename) as fh:
-            response = json.load(fh)
-
-        self.resp_tpls[endpoint.endpoint_id] = response
+        self.response = response
 
     def on_request(self, **kwargs):
         evt = self.get_event(**kwargs)
 
         if not self.auth_integ or self.auth_integ.authorize(evt):
-            ep_id = request.endpoint
-            resp_tpl = self.resp_tpls[ep_id]
+            resp_tpl = self.response
 
             req = {
                 'headers': {k.lower(): v for k, v in request.headers.items()},
                 'params': dict(request.args),
             }
 
             if request.method != 'GET':
@@ -49,15 +43,19 @@
             if 'headers' not in resp_tpl:
                 resp_tpl['headers'] = {}
 
             resp2, status = transform_response(resp_tpl, req)
 
             resp2['headers'].update(base_headers)
 
-            r = jsonify(resp2['body'])
+            if isinstance(resp2['body'], (str, float, int)):
+                r = Response(resp2['body'])
+            else:
+                r = jsonify(resp2['body'])
+
             if 'headers' in resp2:
                 r.headers.update(resp2['headers'])
             r.status = status
 
             return r
         else:
             # todo: handle unauthenticated
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/flask_b/integration/SwaggerIntegration.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from io import StringIO
 
 
 from flask import Response, Flask
 from flask_swagger_ui import get_swaggerui_blueprint
 
 from tomcru.services.aws.hosted.apigw.api_shared.integration import TomcruApiGWHttpIntegration
-from tomcru import TomcruApiDescriptor, TomcruSwaggerIntegrationDescription, utils
+from tomcru import TomcruApiEP, TomcruSwaggerIntegrationEP, utils
 
 
 class SwaggerIntegration(TomcruApiGWHttpIntegration):
 
-    def __init__(self, api: TomcruApiDescriptor, endpoint: TomcruSwaggerIntegrationDescription, swagger_converter, env=None):
+    def __init__(self, api: TomcruApiEP, endpoint: TomcruSwaggerIntegrationEP, swagger_converter, env=None):
         # self.spec = api.spec
         # self.api_name = api.api_name
         self.api = api
         self.endpoint = endpoint
         self.env = env
         self.swagger_converter = swagger_converter
 
@@ -31,15 +31,15 @@
             swagger_content = self.get_swagger_content(self.api, self.endpoint)
 
             r = Response(swagger_content, status=200)
             r.headers['content-type'] = self.content_type
             return r
 
     @cache
-    def get_swagger_content(self, api: TomcruApiDescriptor, endpoint):
+    def get_swagger_content(self, api: TomcruApiEP, endpoint):
         self.content_type = f'application/{endpoint.req_content}'
 
         if not api.spec:
             # generate swagger from tomcru cfg
             api.spec = self.swagger_converter.convert_to_swagger(api)
 
         if 'json' == endpoint.req_content:
@@ -47,15 +47,15 @@
         else:
             sth = StringIO()
             utils.yaml.dump(api.spec, stream=sth)
             swagger_content = sth.getvalue()
 
         return swagger_content
 
-def integrate_swagger_ui_blueprint(app: Flask, swagger_endpoint: TomcruSwaggerIntegrationDescription, ui_endpoint: TomcruSwaggerIntegrationDescription):
+def integrate_swagger_ui_blueprint(app: Flask, swagger_endpoint: TomcruSwaggerIntegrationEP, ui_endpoint: TomcruSwaggerIntegrationEP):
     swaggerui_blueprint = get_swaggerui_blueprint(
         ui_endpoint.route,
         swagger_endpoint.route,
         config={
             # Swagger UI config overrides
             #'app_name':
         },
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/WsAppBuilder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tomcru import TomcruApiDescriptor, TomcruProject, TomcruRouteDescriptor, TomcruLambdaIntegrationDescription
+from tomcru import TomcruApiEP, TomcruProject, TomcruRouteEP, TomcruLambdaIntegrationEP
 
 from .apps.EmeWsApp import EmeWsApp
 
 from tomcru.services.aws.onpremise.aggr_api.ApiGwBuilderCore import ApiGwBuilderCore
 from .integration.LambdaIntegration import LambdaIntegration
 from .integration.WsEnRouteCachedAuthorizer import WsEnRouteCachedAuthorizer
 
@@ -14,15 +14,15 @@
         super().__init__(project, apigw_cfg)
 
         #self.api_serv = self.p.serv('aws:onpremise:aggr_api')
 
     def init(self):
         pass
 
-    def build_api(self, api_name, api: TomcruApiDescriptor, env: str):
+    def build_api(self, api_name, api: TomcruApiEP, env: str):
         self.env = env
 
         # build eme app object
         apiopts = self.apigw_cfg.get('__default__', {})
         apiopts.update(self.apigw_cfg.get(api_name, {}))
 
         self.app = EmeWsApp(self.cfg.apis[api_name], apiopts)
@@ -33,37 +33,37 @@
 
         return self.app
 
     def _build_groups(self, api):
         _connect_authorizer = None
 
         # find base authorizer (for connect)
-        ro: TomcruRouteDescriptor
+        ro: TomcruRouteEP
         for route, ro in api.routes.items():
 
-            endpoint: TomcruLambdaIntegrationDescription
+            endpoint: TomcruLambdaIntegrationEP
             for endpoint in ro.endpoints:
                 if endpoint.route == "$connect":
                     _connect_authorizer = self.authorizers[endpoint.auth] if endpoint.auth else api.default_authorizer
                     break
             else:
                 continue
             break # break when inner loop breaks :v
 
         _integ_authorizer = WsEnRouteCachedAuthorizer(_connect_authorizer)
 
         # write endpoints to lambda + integrations
-        ro: TomcruRouteDescriptor
+        ro: TomcruRouteEP
         for route, ro in api.routes.items():
 
-            endpoint: TomcruLambdaIntegrationDescription
+            endpoint: TomcruLambdaIntegrationEP
             for endpoint in ro.endpoints:
                 # if endpoint.route == "$connect":
 
-                if isinstance(endpoint, TomcruLambdaIntegrationDescription):
+                if isinstance(endpoint, TomcruLambdaIntegrationEP):
                     # build lambda integration
                     _integration = LambdaIntegration(self.app, endpoint, _integ_authorizer, self.p.serv('aws:onpremise:lambda_b'), env=self.env)
                 else:
                     # todo: for now we assume it's always lambda
                     raise NotImplementedError()
 
                 # refer to integration (proxy controller refers to self.on_request)
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/_jank.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.app = None
 
     def create_app(self, api_name, apiopts):
         self.app = EmeWsApp(self.cfg.apis[api_name], apiopts)
 
         return self.app
 
-    def add_method(self, endpoint: TomcruEndpointDescriptor):
+    def add_method(self, endpoint: TomcruEndpoint):
         """
         Adds method to EME/Flask app
         :param endpoint: endpoint url to hook to
         """
 
         #
         # # replace AWS APIGW route scheme to flask routing schema
@@ -41,15 +41,15 @@
         _app_path = os.path.join(self.cfg.app_path, 'groups')
         if os.path.exists(_app_path):
             self.app.load_groups(load_handlers(self.app, 'Group', path=_app_path), webcfg)
 
     def post_to_conn(self, **kwargs):
         raise NotImplementedError()
 
-    def get_called_endpoint(self, msid, user, client, token, data, route, **kwargs) -> TomcruEndpointDescriptor:
+    def get_called_endpoint(self, msid, user, client, token, data, route, **kwargs) -> TomcruEndpoint:
 
         return route
 
     def LambdaIntegration(self, *args, **kwargs):
         return LambdaWebsocketIntegration(self.app, *args, **kwargs)
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/apps/EmeWsApp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
 import time
 from types import SimpleNamespace
 from typing import Dict
 
 
-from tomcru import TomcruSubProjectCfg, TomcruApiDescriptor
+from tomcru import TomcruSubProjectCfg, TomcruApiEP
 
 
 class EmeWsApp(WebsocketApp):
-    def __init__(self, wsappcfg: TomcruApiDescriptor, cfg: dict):
+    def __init__(self, wsappcfg: TomcruApiEP, cfg: dict):
         self.debug = True
         self.api_name = wsappcfg.api_name
         self.api_type = 'ws'
         self.is_main_thread = False
 
         super().__init__({
             'websocket': {
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/LambdaIntegration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import inspect
 import json
 import time
 from datetime import datetime
 from urllib import parse
 
-from tomcru import TomcruLambdaIntegrationDescription
+from tomcru import TomcruLambdaIntegrationEP
 
 from .TomcruApiGWWsIntegration import TomcruApiGWWsIntegration
 
 
 class LambdaIntegration(TomcruApiGWWsIntegration):
 
-    def __init__(self, wsapp, endpoint: TomcruLambdaIntegrationDescription, auth, lambda_builder, env=None):
+    def __init__(self, wsapp, endpoint: TomcruLambdaIntegrationEP, auth, lambda_builder, env=None):
         self.app = wsapp
         self.endpoint = endpoint
         self.auth_integ = auth
         self.lambda_builder = lambda_builder
         self.env = env
 
         self.lambda_builder.build_lambda(endpoint.lambda_id, env=self.env)
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw/ws_b/aggr_ws/integration/WsEnRouteCachedAuthorizer.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/apigw_manager_b/ApiGWMgr.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/boto3_b/Boto3Builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class Boto3Builder(ServiceBase):
     INIT_PRIORITY = 1
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # self.boto3_obj: Boto3 | None = None
-        self.boto3_obj = Boto3(self.get_resource, self.opts.get('allowed.clients', cast=set), self.opts.get('allowed.resources', cast=set))
+        self.boto3_obj = Boto3(self, self.opts.get('allowed.clients', cast=set), self.opts.get('allowed.resources', cast=set))
 
     def init(self):
         """
         Builds onpremsie boto3 wrapper
 
         :param apigw_app_wrapper: local api implementation `
         :return:
@@ -37,11 +37,17 @@
 
         utils.inject('boto3', __dir__, self.boto3_obj)
 
     def deject_dependencies(self):
         utils.clean_inject('boto3')
 
     def add_resource(self, res_id, res):
+        return self.service('obj_store').add('boto3', 'res-'+res_id, res)
+
+    def add_client(self, res_id, res):
         return self.service('obj_store').add('boto3', res_id, res)
 
     def get_resource(self, res_id):
+        return self.service('obj_store').get('boto3', 'res-'+res_id)
+
+    def get_client(self, res_id):
         return self.service('obj_store').get('boto3', res_id)
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/boto3_b/boto3.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/boto3_b/boto3.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,22 +6,20 @@
         self._objs_getter = objgetter
         self.allowed_clients = allowed_clients
         self.allowed_resources = allowed_resources
 
     def client(self, resname, **kwargs):
         assert resname in self.allowed_clients
 
-        _obj = self._objs_getter(resname)
-        # if hasattr(_obj, 'as_boto3_resource'):
-        #     return _obj.as_boto3_resource(**kwargs)
+        _obj = self._objs_getter.get_client(resname)
+
         return _obj
 
     def resource(self, resname, **kwargs):
         assert resname in self.allowed_resources
 
-        _obj = self._objs_getter(resname)
-        # if hasattr(_obj, 'as_boto3_resource'):
-        #     return _obj.as_boto3_resource(**kwargs)
+        _obj = self._objs_getter.get_resource(resname)
+
         return _obj
 
     def Session(self):
         return self
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DdbTableAdapter.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DDBSqlAlchemyTable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import re
 from sqlalchemy.orm.attributes import flag_modified
 
 from botocore.exceptions import ClientError
 from sqlalchemy import text
 
 
-class DdbTableAdapter:
-    def __init__(self, sess, ent_obj, autocommit=True):
-        self.T = ent_obj
+class DDBSqlAlchemyTable:
+    def __init__(self, sess, mapped_model, tabledef, autocommit=True):
+        self.T = mapped_model
+        self.TableDef = tabledef
         self.session = sess
-        self.table_name = self.T.__tablename__
 
-        self.partition_key = ent_obj.partition_key
-        self.sort_key = ent_obj.sort_key
+        self.table_name = self.TableDef.fullname
+        self.partition_key = self.TableDef.primary_key.columns[0].name
+        self.sort_key = None
+        # todo: support sort_key!
+
         self._autocommit = autocommit
 
     def _get_ent(self, Key):
         if self.sort_key:
             _reldbkey = (Key[self.partition_key], Key[self.sort_key])
         else:
             _reldbkey = Key[self.partition_key]
@@ -34,18 +37,32 @@
         #self.ent2dict(ent)
         return {
             'Item': ent.ddb_content
         }
 
     def put_item(self, Item, **kwargs):
         # check if already exists
-        ent = self._get_ent(self._get_key(Item))
+        key = self._get_key(Item)
+        ent = self._get_ent(key)
 
         if not ent:
-            ent = self.T(**Item)
+            ent = self.T()
+
+            setattr(ent, self.partition_key, key[self.partition_key])
+            if self.sort_key:
+                setattr(ent, self.sort_key, key[self.sort_key])
+
+            setattr(ent, 'ddb_content', Item.copy())
+            #         for k,v in kwargs.items():
+            #             setattr(self, k, v)
+            #
+            #         self.ddb_content = kwargs.copy()
+
+            print(1)
+            #ent = self.T(**Item)
         else:
             ent.ddb_content = Item
 
         self.session.add(ent)
 
         if self._autocommit:
             self.session.commit()
@@ -232,7 +249,9 @@
             _key[self.sort_key] = Item[self.sort_key]
 
         return _key
 
     def _truncate(self):
         self.session.execute(f'''TRUNCATE TABLE "{self.table_name}"''')
         self.session.commit()
+
+
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/DynamoDBBuilder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from .DdbSqlalchemyAdapter import DdbSqlAlchemyAdapter
+from .boto3_proxy import DDBResource
 from .dal_ddb import build_database
 from tomcru.services.ServiceBase import ServiceBase
 
+from .DDBSqlAlchemyTable import DDBSqlAlchemyTable
+from .boto3_proxy import DDBClient, DDBResource
+
 
 class DynamoDBBuilder(ServiceBase):
     INIT_PRIORITY = 2
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.ddb = None
+        self.cli = None
+        self.res = None
 
     def init(self):
-        if self.ddb:
-            raise Exception("Already initialized")
+        if self.cli:
+            raise Exception("DDB: Already initialized")
 
+        # todo: later: group obj instances by AWS-REGION ?
         sess, tables = build_database(self.env.app_path, self.opts.get('conn.dsn'), self.cfg.conf.get('tables'))
+        tables = {k: DDBSqlAlchemyTable(sess, *t) for k,t in tables.items()}
+        self.cli = DDBClient(tables)
+        self.res = DDBResource(tables)
 
-        # todo: later: group obj instances by AWS-REGION
-        self.ddb = DdbSqlAlchemyAdapter(sess, tables)
-
-        self.service('boto3').add_resource('dynamodb', self.ddb)
+        self.service('boto3').add_resource('dynamodb', self.res)
+        self.service('boto3').add_client('dynamodb', self.cli)
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/ddb/sqlalchemy_b/SqlAlchemyJSONType.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/lambda_b/EmeLambdaContext.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/lambda_b/LambdaHostedPyContext.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 import time
 
 
-class EmeLambdaContext:
+class LambdaHostedPyContext:
     def __init__(self, ctx_cfg: dict):
         self.max_lambda_time_ms = ctx_cfg.get('timeout', 900)
         self.start = time.time()
 
     def get_remaining_time_in_millis(self):
         return self.max_lambda_time_ms - 1000*(time.time()-self.start)
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/s3_b/S3AdapterLocal.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         for bucket, bucket_cfg in self.buckets.items():
             path = bucket_cfg.get('path', os.path.join(_default_bucket_path, bucket))
             bucket_cfg['path'] = os.path.join(app_path, path)
 
             if not os.path.exists(bucket_cfg['path']):
                 print("S3AdapterLocal: creating bucket directory:", bucket_cfg['path'])
                 os.makedirs(bucket_cfg['path'])
+
     def _get_path(self, Bucket, Key):
         return os.path.join(self.buckets[Bucket]['path'], Key)
 
     def upload_file(self, Filename, Bucket, Key):
         # with open(Filename, 'b') as fh:
         #     self.upload_fileobj(fh, **kwargs)
 
@@ -52,14 +53,15 @@
         if isinstance(Body, bytes):
             raise NotImplementedError()
         else:
             with open(_path, 'b') as fh:
                 shutil.copyfileobj(Body, fh)
                 #fh.write(Body.read())
 
+
     def download_file(self, Bucket, Key, Filename, ExtraArgs=None, Callback=None, Config=None):
         from_path = self._get_path(Bucket, Key)
 
         if os.path.exists(from_path) and os.path.exists(Filename) and \
             os.path.samefile(from_path, Filename):
             # noop, used in dev environments
             return
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/hosted/s3_b/S3Service.py` & `tomcru-0.2.3/tomcru/services/aws/hosted/s3_b/S3Service.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py` & `tomcru-0.2.3/tomcru/services/aws/onpremise/model_checker/SwaggerResponseModelValidator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import json
 
-from tomcru import TomcruApiDescriptor, TomcruProject, TomcruEndpointDescriptor, TomcruSwaggerIntegrationDescription
+from tomcru import TomcruApiEP, TomcruProject, TomcruEndpoint, TomcruSwaggerIntegrationEP
 
 from flask import Flask, request, jsonify, Response, Request
 
 
 class SwaggerResponseModelValidator:
 
     def __init__(self, project: TomcruProject, mock_cfg):
         self.cfg = project.cfg
         self.p = project
 
-    def check_response(self, api: TomcruApiDescriptor, ep: TomcruEndpointDescriptor, response: Response, env: str):
-        if isinstance(ep, TomcruSwaggerIntegrationDescription):
+    def check_response(self, api: TomcruApiEP, ep: TomcruEndpoint, response: Response, env: str):
+        if isinstance(ep, TomcruSwaggerIntegrationEP):
             # ignore all swagger endpoints, no need to validate
             return
 
         content_type = response.headers['content-type']
         _paths = api.spec_resolved_schemas['paths']
 
         if ep.route not in _paths:
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py` & `tomcru-0.2.3/tomcru/services/aws/onpremise/s3_static/S3StaticBuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 import shutil
 import subprocess
 import json
 
 import eme.static, eme.entities
-from tomcru import TomcruApiDescriptor, TomcruProject
+from tomcru import TomcruApiEP, TomcruProject
 
 
 class S3StaticBuilder:
 
     def __init__(self, project: TomcruProject, static_cfg):
         self.cfg = project.cfg
         self.opts = static_cfg
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/_junk/SamTplBuilder.py` & `tomcru-0.2.3/tomcru/services/aws/sam/_junk/SamTplBuilder.py`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/_junk/core.yaml` & `tomcru-0.2.3/tomcru/services/aws/sam/_junk/core.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/_junk/httpapi.yaml` & `tomcru-0.2.3/tomcru/services/aws/sam/_junk/httpapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/_junk/integ_ws.yaml` & `tomcru-0.2.3/tomcru/services/aws/sam/_junk/integ_ws.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/_junk/template.yaml` & `tomcru-0.2.3/tomcru/services/aws/sam/_junk/template.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/_junk/wsapi.yaml` & `tomcru-0.2.3/tomcru/services/aws/sam/_junk/wsapi.yaml`

 * *Files identical despite different names*

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py` & `tomcru-0.2.3/tomcru/services/aws/sam/lambda_b/LambdaBuilder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tomcru import TomcruEndpointDescriptor, TomcruProject, TomcruLambdaIntegrationDescription
+from tomcru import TomcruEndpoint, TomcruProject, TomcruLambdaIntegrationEP
 
 
 class LambdaBuilder:
     def __init__(self, project: TomcruProject, opts: dict):
         self.cfg = project.cfg
         self.opts = opts
         self.lambdas = set()
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/params_b/ParametersBuilder.py` & `tomcru-0.2.3/tomcru/services/aws/sam/params_b/ParametersBuilder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from collections import defaultdict
 
-from tomcru import TomcruEndpointDescriptor, TomcruProject, TomcruLambdaIntegrationDescription
+from tomcru import TomcruEndpoint, TomcruProject, TomcruLambdaIntegrationEP
 
 
 class ParametersBuilder:
     def __init__(self, project: TomcruProject, opts: dict):
         self.cfg = project.cfg
         self.opts = opts
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py` & `tomcru-0.2.3/tomcru/services/aws/sam/spec_api_b/SwaggerApiTemplater.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tomcru import TomcruProject, TomcruApiDescriptor, TomcruEndpointDescriptor, TomcruLambdaIntegrationDescription, TomcruApiLambdaAuthorizerDescriptor, TomcruApiOIDCAuthorizerDescriptor, TomcruRouteDescriptor
+from tomcru import TomcruProject, TomcruApiEP, TomcruEndpoint, TomcruLambdaIntegrationEP, TomcruApiLambdaAuthorizerEP, TomcruApiOIDCAuthorizerEP, TomcruRouteEP
 
 from .integrations.SAMLambdaBuilder import SAMLambdaBuilder
 from .authorizers.SAMLambdaAuthBuilder import SAMLambdaAuthBuilder
 from .authorizers.SAMOIDCAuthBuilder import SAMOIDCAuthBuilder
 
 
 class SwaggerApiTemplater:
@@ -10,23 +10,23 @@
     def __init__(self, project: TomcruProject, opts: dict):
         self.cfg = project.cfg
         self.opts = opts
         self.lambda_builder = project.serv('aws:sam:lambda_b')
         self.param_builder = project.serv('aws:sam:params_b')
 
         self.integrations_b: dict[type, object] = {
-            TomcruLambdaIntegrationDescription: SAMLambdaBuilder(self.param_builder, self.lambda_builder)
+            TomcruLambdaIntegrationEP: SAMLambdaBuilder(self.param_builder, self.lambda_builder)
         }
 
         self.authorizers_b: dict[type, object] = {
-            TomcruApiLambdaAuthorizerDescriptor: SAMLambdaAuthBuilder(self.param_builder, self.lambda_builder, self.opts['external_authorizers']),
-            TomcruApiOIDCAuthorizerDescriptor: SAMOIDCAuthBuilder(self.param_builder)
+            TomcruApiLambdaAuthorizerEP: SAMLambdaAuthBuilder(self.param_builder, self.lambda_builder, self.opts['external_authorizers']),
+            TomcruApiOIDCAuthorizerEP: SAMOIDCAuthBuilder(self.param_builder)
         }
 
-    def build_api(self, api: TomcruApiDescriptor, env: str):
+    def build_api(self, api: TomcruApiEP, env: str):
         # todo: stage var
         # todo: env var?
 
         # hat tesomsz mit kell ezt csurni-csavarni
         spec = dict(api.spec)
 
         self._build_authorizers(spec, api)
@@ -37,33 +37,33 @@
             'Type': 'AWS::Serverless::HttpApi',
             'Properties': {
                 'StageName': 'v1',
                 'DefinitionBody': spec
             }
         }
 
-    def _build_authorizers(self, spec, api: TomcruApiDescriptor):
+    def _build_authorizers(self, spec, api: TomcruApiEP):
         components = spec.get('components', {})
 
         if 'securitySchemes' in components:
             for auth_id, auth_spec in components['securitySchemes'].items():
                 auth = self.cfg.authorizers[auth_id]
 
                 apiopts = self.opts.get('__default__', {})
                 apiopts.update(self.opts.get(api.api_name, {}))
 
                 auth_builder = self.authorizers_b[type(auth)]
                 auth_spec['x-amazon-apigateway-authorizer'] = auth_builder.build(auth_id, auth, apiopts)
 
-    def _build_endpoints(self, spec, api: TomcruApiDescriptor):
+    def _build_endpoints(self, spec, api: TomcruApiEP):
 
-        ro: TomcruRouteDescriptor
+        ro: TomcruRouteEP
         for route, ro in api.routes.items():
 
-            endpoint: TomcruEndpointDescriptor
+            endpoint: TomcruEndpoint
             for endpoint in ro.endpoints:
                 op = endpoint.spec_ref
 
                 if not op:
                     print("        MISSING SWAGGER REF for", endpoint)
                     continue
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py` & `tomcru-0.2.3/tomcru/services/aws/sam/spec_api_b/authorizers/SAMLambdaAuthBuilder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from tomcru import TomcruApiLambdaAuthorizerDescriptor
+from tomcru import TomcruApiLambdaAuthorizerEP
 from core.utils.yaml_custom import Ref, Join
 
 
 class SAMLambdaAuthBuilder:
     def __init__(self, param_builder, lambda_builder, external_authorizers):
         self.param_builder = param_builder
         self.lambda_builder = lambda_builder
         self.external_authorizers = external_authorizers
 
-    def build(self, auth_id, auth: TomcruApiLambdaAuthorizerDescriptor, apiopts):
+    def build(self, auth_id, auth: TomcruApiLambdaAuthorizerEP, apiopts):
         role_id = self.param_builder.store('LambdaAccessRole', apiopts['access_role'])
 
         auth_integ = {
             'type': 'request',
             'identitySource': f"$request.{auth.src_in}.{auth.src_name}",
             'authorizerResultTtlInSeconds': 3600,
             'authorizerPayloadFormatVersion': 2.0,
```

### Comparing `tomcru-0.1.3/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py` & `tomcru-0.2.3/tomcru/services/aws/sam/spec_api_b/integrations/SAMLambdaBuilder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from tomcru import TomcruRouteDescriptor, TomcruLambdaIntegrationDescription
+from tomcru import TomcruRouteEP, TomcruLambdaIntegrationEP
 from core.utils.yaml_custom import GetAtt, Ref
 
 
 class SAMLambdaBuilder:
     def __init__(self, param_builder, lambda_builder):
         self.param_builder = param_builder
         self.lambda_builder = lambda_builder
 
-    def build(self, integ_cfg: TomcruLambdaIntegrationDescription):
+    def build(self, integ_cfg: TomcruLambdaIntegrationEP):
         integ = {
             'type': "aws_proxy",
             'httpMethod': "POST",
             'uri': GetAtt(f"{integ_cfg.group}_{integ_cfg.lambda_id}.Arn"),
             # todo: configure timeout?
             'timeoutInMillis': 3000,
             'payloadFormatVersion': "2.0"
```

### Comparing `tomcru-0.1.3/tomcru/services/general/eme2swagger/Eme2Swagger.py` & `tomcru-0.2.3/tomcru/services/general/eme2swagger/Eme2Swagger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections import defaultdict
 
-from tomcru import TomcruProject, TomcruApiDescriptor, TomcruLambdaIntegrationDescription, TomcruApiLambdaAuthorizerDescriptor, TomcruSwaggerIntegrationDescription
+from tomcru import TomcruProject, TomcruApiEP, TomcruLambdaIntegrationEP, TomcruApiLambdaAuthorizerEP, TomcruSwaggerIntegrationEP
 
 
 class Eme2Swagger:
 
     def __init__(self, project: TomcruProject, opts: dict):
         self.p = project
         self.cfg = project.cfg
         self.opts = opts
 
-    def convert_to_swagger(self, api: TomcruApiDescriptor):
+    def convert_to_swagger(self, api: TomcruApiEP):
         paths = defaultdict(dict)
 
         # define authorizers used by this api, based on the lambda integrations
         api_authorizers = set()
 
         for route, route_cfg in api.routes.items():
             for endpoint in route_cfg.endpoints:
@@ -52,20 +52,20 @@
             }
         }
 
     def get_integ(self, endpoint, authorizers_discovered: set):
         if endpoint.auth:
             authorizers_discovered.add(endpoint.auth)
 
-        if isinstance(endpoint, TomcruLambdaIntegrationDescription):
+        if isinstance(endpoint, TomcruLambdaIntegrationEP):
             return {
                 'x-lambda': {
                     'lambda-id': endpoint.lambda_id,
                     'role': endpoint.role,
                     'layers': endpoint.layers,
                     'auth': endpoint.auth
                 }
             }
-        elif isinstance(endpoint, TomcruSwaggerIntegrationDescription):
+        elif isinstance(endpoint, TomcruSwaggerIntegrationEP):
             return {}
         else:
             raise NotImplementedError(str(endpoint))
```

### Comparing `tomcru-0.1.3/PKG-INFO` & `tomcru-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomcru
-Version: 0.1.3
+Version: 0.2.3
 Summary: Serverless app framework
 Author: Rajmund Csombordi
 Author-email: rajmund.csombordi@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

