# Comparing `tmp/descope-1.1.1.tar.gz` & `tmp/descope-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descope-1.1.1.tar", max compression
+gzip compressed data, was "descope-1.5.0.tar", max compression
```

## Comparing `descope-1.1.1.tar` & `descope-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1064 2023-04-20 15:32:22.171015 descope-1.1.1/LICENSE
--rw-r--r--   0        0        0    28342 2023-04-20 15:32:22.171015 descope-1.1.1/README.md
--rw-r--r--   0        0        0      531 2023-04-20 15:32:22.171015 descope-1.1.1/descope/__init__.py
--rw-r--r--   0        0        0    20073 2023-04-20 15:32:22.171015 descope-1.1.1/descope/auth.py
--rw-r--r--   0        0        0        0 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/__init__.py
--rw-r--r--   0        0        0     4956 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/enchantedlink.py
--rw-r--r--   0        0        0     5451 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/magiclink.py
--rw-r--r--   0        0        0     1588 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/oauth.py
--rw-r--r--   0        0        0    10008 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/otp.py
--rw-r--r--   0        0        0     8200 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/password.py
--rw-r--r--   0        0        0     1541 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/saml.py
--rw-r--r--   0        0        0     5181 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/totp.py
--rw-r--r--   0        0        0     6759 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/webauthn.py
--rw-r--r--   0        0        0     4267 2023-04-20 15:32:22.171015 descope-1.1.1/descope/common.py
--rw-r--r--   0        0        0    11188 2023-04-20 15:32:22.171015 descope-1.1.1/descope/descope_client.py
--rw-r--r--   0        0        0     1353 2023-04-20 15:32:22.171015 descope-1.1.1/descope/exceptions.py
--rw-r--r--   0        0        0     5661 2023-04-20 15:32:22.171015 descope-1.1.1/descope/management/access_key.py
--rw-r--r--   0        0        0     3426 2023-04-20 15:32:22.171015 descope-1.1.1/descope/management/common.py
--rw-r--r--   0        0        0     3911 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/group.py
--rw-r--r--   0        0        0     1019 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/jwt.py
--rw-r--r--   0        0        0     2591 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/permission.py
--rw-r--r--   0        0        0     2989 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/role.py
--rw-r--r--   0        0        0     5200 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/sso_settings.py
--rw-r--r--   0        0        0     3477 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/tenant.py
--rw-r--r--   0        0        0    23454 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/user.py
--rw-r--r--   0        0        0     1408 2023-04-20 15:32:22.175015 descope-1.1.1/descope/mgmt.py
--rw-r--r--   0        0        0     1125 2023-04-20 15:32:46.674681 descope-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    29435 1970-01-01 00:00:00.000000 descope-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-07 10:57:55.656598 descope-1.5.0/LICENSE
+-rw-r--r--   0        0        0    29105 2023-05-07 10:57:55.656598 descope-1.5.0/README.md
+-rw-r--r--   0        0        0      531 2023-05-07 10:57:55.660598 descope-1.5.0/descope/__init__.py
+-rw-r--r--   0        0        0      211 2023-05-07 10:57:55.660598 descope-1.5.0/descope/_auth_base.py
+-rw-r--r--   0        0        0    20959 2023-05-07 10:57:55.660598 descope-1.5.0/descope/auth.py
+-rw-r--r--   0        0        0        0 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/__init__.py
+-rw-r--r--   0        0        0     5319 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/enchantedlink.py
+-rw-r--r--   0        0        0     6200 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/magiclink.py
+-rw-r--r--   0        0        0     1528 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/oauth.py
+-rw-r--r--   0        0        0    11067 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/otp.py
+-rw-r--r--   0        0        0     8146 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/password.py
+-rw-r--r--   0        0        0     1481 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/saml.py
+-rw-r--r--   0        0        0     5128 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/totp.py
+-rw-r--r--   0        0        0     6705 2023-05-07 10:57:55.660598 descope-1.5.0/descope/authmethod/webauthn.py
+-rw-r--r--   0        0        0     4296 2023-05-07 10:57:55.660598 descope-1.5.0/descope/common.py
+-rw-r--r--   0        0        0    11310 2023-05-07 10:57:55.660598 descope-1.5.0/descope/descope_client.py
+-rw-r--r--   0        0        0     1420 2023-05-07 10:57:55.660598 descope-1.5.0/descope/exceptions.py
+-rw-r--r--   0        0        0     5798 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/access_key.py
+-rw-r--r--   0        0        0     3811 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/common.py
+-rw-r--r--   0        0        0     3394 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/flow.py
+-rw-r--r--   0        0        0     3971 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/group.py
+-rw-r--r--   0        0        0      959 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/jwt.py
+-rw-r--r--   0        0        0     2531 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/permission.py
+-rw-r--r--   0        0        0     3094 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/role.py
+-rw-r--r--   0        0        0     5895 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/sso_settings.py
+-rw-r--r--   0        0        0     3685 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/tenant.py
+-rw-r--r--   0        0        0    27563 2023-05-07 10:57:55.660598 descope-1.5.0/descope/management/user.py
+-rw-r--r--   0        0        0     1556 2023-05-07 10:57:55.660598 descope-1.5.0/descope/mgmt.py
+-rw-r--r--   0        0        0     1152 2023-05-07 10:58:19.424900 descope-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    30198 1970-01-01 00:00:00.000000 descope-1.5.0/PKG-INFO
```

### Comparing `descope-1.1.1/LICENSE` & `descope-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `descope-1.1.1/README.md` & `descope-1.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -558,14 +558,17 @@
 ```
 
 ### Manage SSO Setting
 
 You can manage SSO settings and map SSO group roles and user attributes.
 
 ```Python
+# You can get SSO settings for a tenant
+sso_settings_res = descope_client.mgmt.sso.get_settings("tenant-id")
+
 # You can configure SSO settings manually by setting the required fields directly
 descope_client.mgmt.sso.configure(
     tenant_id, # Which tenant this configuration is for
     idp_url="https://idp.com",
     entity_id="my-idp-entity-id",
     idp_cert="<your-cert-here>",
     redirect_url="https://your.domain.com", # Global redirection after successful authentication
@@ -649,14 +652,40 @@
 # Load all roles
 roles_resp = descope_client.mgmt.role.load_all()
 roles = roles_resp["roles"]
     for role in roles:
         # Do something
 ```
 
+### Manage Flows and Theme
+
+You can export and import your project flows and theme:
+
+```Python
+# Export a selected flow by id for the flow and matching screens.
+exported_flow_and_screens = descope_client.mgmt.flow.export_flow(
+    flow_id="sign-up-or-in",
+)
+
+# Import a given flow and screens to the flow matching the id provided.
+imported_flow_and_screens = descope_client.mgmt.flow.import_flow(
+    flow_id="sign-up-or-in",
+    flow={},
+    screens=[]
+)
+
+# Export your project theme.
+exported_theme = descope_client.mgmt.flow.export_theme()
+
+# Import a theme to your project.
+imported_theme = descope_client.mgmt.flow.import_flow(
+    theme={}
+)
+```
+
 ### Query SSO Groups
 
 You can query SSO groups:
 
 ```Python
 # Load all groups for a given tenant id
 groups_resp = descope_client.mgmt.group.load_all_groups(
```

### Comparing `descope-1.1.1/descope/__init__.py` & `descope-1.5.0/descope/__init__.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.1/descope/auth.py` & `descope-1.5.0/descope/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pkg_resources
 import requests
 from email_validator import EmailNotValidError, validate_email
 
 from descope.common import (
     COOKIE_DATA_NAME,
     DEFAULT_BASE_URL,
+    DEFAULT_TIMEOUT_SECONDS,
     PHONE_REGEX,
     REFRESH_SESSION_COOKIE_NAME,
     REFRESH_SESSION_TOKEN_NAME,
     SESSION_TOKEN_NAME,
     DeliveryMethod,
     EndpointsV1,
     EndpointsV2,
@@ -38,14 +39,15 @@
 
     def __init__(
         self,
         project_id: str = None,
         public_key: str = None,
         skip_verify: bool = False,
         management_key: str = None,
+        timeout_seconds: float = DEFAULT_TIMEOUT_SECONDS,
     ):
         self.lock_public_keys = Lock()
         # validate project id
         if not project_id:
             # try get the project_id from env
             project_id = os.getenv("DESCOPE_PROJECT_ID", "")
             if project_id == "":
@@ -57,14 +59,15 @@
         self.project_id = project_id
 
         self.secure = True
         if skip_verify:
             self.secure = False
 
         self.base_url = os.getenv("DESCOPE_BASE_URI", None) or DEFAULT_BASE_URL
+        self.timeout_seconds = timeout_seconds
 
         if not management_key:
             management_key = os.getenv("DESCOPE_MANAGEMENT_KEY", None)
         self.management_key = management_key
 
         if not public_key:
             public_key = os.getenv("DESCOPE_PUBLIC_KEY", None)
@@ -99,14 +102,15 @@
     ) -> requests.Response:
         response = requests.get(
             f"{self.base_url}{uri}",
             headers=self._get_default_headers(pswd),
             params=params,
             allow_redirects=allow_redirects,
             verify=self.secure,
+            timeout=self.timeout_seconds,
         )
         if not response.ok:
             if response.status_code == 429:
                 self._raise_rate_limit_exception(response)  # Raise RateLimitException
             raise AuthException(
                 response.status_code, ERROR_TYPE_SERVER_ERROR, response.text
             )
@@ -118,14 +122,32 @@
         response = requests.post(
             f"{self.base_url}{uri}",
             headers=self._get_default_headers(pswd),
             data=json.dumps(body),
             allow_redirects=False,
             verify=self.secure,
             params=params,
+            timeout=self.timeout_seconds,
+        )
+        if not response.ok:
+            if response.status_code == 429:
+                self._raise_rate_limit_exception(response)  # Raise RateLimitException
+
+            raise AuthException(
+                response.status_code, ERROR_TYPE_SERVER_ERROR, response.text
+            )
+        return response
+
+    def do_delete(self, uri: str, pswd: str = None) -> requests.Response:
+        response = requests.delete(
+            f"{self.base_url}{uri}",
+            headers=self._get_default_headers(pswd),
+            allow_redirects=False,
+            verify=self.secure,
+            timeout=self.timeout_seconds,
         )
         if not response.ok:
             if response.status_code == 429:
                 self._raise_rate_limit_exception(response)  # Raise RateLimitException
 
             raise AuthException(
                 response.status_code, ERROR_TYPE_SERVER_ERROR, response.text
@@ -214,15 +236,15 @@
             )
 
     @staticmethod
     def get_method_string(method: DeliveryMethod) -> str:
         if method is DeliveryMethod.EMAIL:
             return "email"
         elif method is DeliveryMethod.SMS:
-            return "phone"
+            return "sms"
         elif method is DeliveryMethod.WHATSAPP:
             return "whatsapp"
         else:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, f"Unknown delivery method: {method}"
             )
 
@@ -323,14 +345,15 @@
 
     def _fetch_public_keys(self) -> None:
         # This function called under mutex protection so no need to acquire it once again
         response = requests.get(
             f"{self.base_url}{EndpointsV2.public_key_path}/{self.project_id}",
             headers=self._get_default_headers(),
             verify=self.secure,
+            timeout=self.timeout_seconds,
         )
 
         if not response.ok:
             if response.status_code == 429:
                 self._raise_rate_limit_exception(response)  # Raise RateLimitException
             raise AuthException(
                 response.status_code,
```

### Comparing `descope-1.1.1/descope/authmethod/enchantedlink.py` & `descope-1.5.0/descope/authmethod/enchantedlink.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 import string
 
 import requests
 
+from descope._auth_base import AuthBase
 from descope.auth import Auth
 from descope.common import (
     REFRESH_SESSION_COOKIE_NAME,
     DeliveryMethod,
     EndpointsV1,
     LoginOptions,
     validate_refresh_token_provided,
 )
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 
-class EnchantedLink:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class EnchantedLink(AuthBase):
     def sign_in(
         self,
         login_id: str,
         uri: str,
         login_options: LoginOptions = None,
         refresh_token: str = None,
     ) -> dict:
@@ -75,23 +71,32 @@
         return jwt_response
 
     def verify(self, token: str):
         uri = EndpointsV1.verify_enchantedlink_auth_path
         body = EnchantedLink._compose_verify_body(token)
         self._auth.do_post(uri, body, None)
 
-    def update_user_email(self, login_id: str, email: str, refresh_token: str) -> dict:
+    def update_user_email(
+        self,
+        login_id: str,
+        email: str,
+        refresh_token: str,
+        add_to_login_ids: bool = False,
+        on_merge_use_existing: bool = False,
+    ) -> dict:
         if not login_id:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "Identifier cannot be empty"
             )
 
         Auth.validate_email(email)
 
-        body = EnchantedLink._compose_update_user_email_body(login_id, email)
+        body = EnchantedLink._compose_update_user_email_body(
+            login_id, email, add_to_login_ids, on_merge_use_existing
+        )
         uri = EndpointsV1.update_user_email_otp_path
         response = self._auth.do_post(uri, body, None, refresh_token)
         return EnchantedLink._get_pending_ref_from_response(response)
 
     @staticmethod
     def _compose_signin_url() -> str:
         return Auth.compose_url(
@@ -137,16 +142,23 @@
         return body
 
     @staticmethod
     def _compose_verify_body(token: string) -> dict:
         return {"token": token}
 
     @staticmethod
-    def _compose_update_user_email_body(login_id: str, email: str) -> dict:
-        return {"loginId": login_id, "email": email}
+    def _compose_update_user_email_body(
+        login_id: str, email: str, add_to_login_ids: bool, on_merge_use_existing: bool
+    ) -> dict:
+        return {
+            "loginId": login_id,
+            "email": email,
+            "addToLoginIDs": add_to_login_ids,
+            "onMergeUseExisting": on_merge_use_existing,
+        }
 
     @staticmethod
     def _compose_get_session_body(pending_ref: str) -> dict:
         return {"pendingRef": pending_ref}
 
     @staticmethod
     def _get_pending_ref_from_response(response: requests.Response) -> dict:
```

### Comparing `descope-1.1.1/descope/authmethod/magiclink.py` & `descope-1.5.0/descope/authmethod/magiclink.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import string
 
+from descope._auth_base import AuthBase
 from descope.auth import Auth
 from descope.common import (
     REFRESH_SESSION_COOKIE_NAME,
     DeliveryMethod,
     EndpointsV1,
     LoginOptions,
     validate_refresh_token_provided,
 )
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 
-class MagicLink:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class MagicLink(AuthBase):
     def sign_in(
         self,
         method: DeliveryMethod,
         login_id: str,
         uri: str,
         login_options: LoginOptions = None,
         refresh_token: str = None,
@@ -39,15 +35,14 @@
 
         response = self._auth.do_post(uri, body, None, refresh_token)
         return Auth.extract_masked_address(response.json(), method)
 
     def sign_up(
         self, method: DeliveryMethod, login_id: str, uri: str, user: dict = None
     ) -> str:
-
         if not user:
             user = {}
 
         if not self._auth.verify_delivery_method(method, login_id, user):
             raise AuthException(
                 400,
                 ERROR_TYPE_INVALID_ARGUMENT,
@@ -71,38 +66,55 @@
         response = self._auth.do_post(uri, body, None)
         resp = response.json()
         jwt_response = self._auth.generate_jwt_response(
             resp, response.cookies.get(REFRESH_SESSION_COOKIE_NAME, None)
         )
         return jwt_response
 
-    def update_user_email(self, login_id: str, email: str, refresh_token: str) -> str:
+    def update_user_email(
+        self,
+        login_id: str,
+        email: str,
+        refresh_token: str,
+        add_to_login_ids: bool = False,
+        on_merge_use_existing: bool = False,
+    ) -> str:
         if not login_id:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "Identifier cannot be empty"
             )
 
         Auth.validate_email(email)
 
-        body = MagicLink._compose_update_user_email_body(login_id, email)
+        body = MagicLink._compose_update_user_email_body(
+            login_id, email, add_to_login_ids, on_merge_use_existing
+        )
         uri = EndpointsV1.update_user_email_magiclink_path
         response = self._auth.do_post(uri, body, None, refresh_token)
         return Auth.extract_masked_address(response.json(), DeliveryMethod.EMAIL)
 
     def update_user_phone(
-        self, method: DeliveryMethod, login_id: str, phone: str, refresh_token: str
+        self,
+        method: DeliveryMethod,
+        login_id: str,
+        phone: str,
+        refresh_token: str,
+        add_to_login_ids: bool = False,
+        on_merge_use_existing: bool = False,
     ) -> str:
         if not login_id:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "Identifier cannot be empty"
             )
 
         Auth.validate_phone(method, phone)
 
-        body = MagicLink._compose_update_user_phone_body(login_id, phone)
+        body = MagicLink._compose_update_user_phone_body(
+            login_id, phone, add_to_login_ids, on_merge_use_existing
+        )
         uri = EndpointsV1.update_user_phone_magiclink_path
         response = self._auth.do_post(uri, body, None, refresh_token)
         return Auth.extract_masked_address(response.json(), DeliveryMethod.SMS)
 
     @staticmethod
     def _compose_signin_url(method: DeliveryMethod) -> str:
         return Auth.compose_url(EndpointsV1.sign_in_auth_magiclink_path, method)
@@ -147,13 +159,27 @@
         return body
 
     @staticmethod
     def _compose_verify_body(token: string) -> dict:
         return {"token": token}
 
     @staticmethod
-    def _compose_update_user_email_body(login_id: str, email: str) -> dict:
-        return {"loginId": login_id, "email": email}
+    def _compose_update_user_email_body(
+        login_id: str, email: str, add_to_login_ids: bool, on_merge_use_existing: bool
+    ) -> dict:
+        return {
+            "loginId": login_id,
+            "email": email,
+            "addToLoginIDs": add_to_login_ids,
+            "onMergeUseExisting": on_merge_use_existing,
+        }
 
     @staticmethod
-    def _compose_update_user_phone_body(login_id: str, phone: str) -> dict:
-        return {"loginId": login_id, "phone": phone}
+    def _compose_update_user_phone_body(
+        login_id: str, phone: str, add_to_login_ids: bool, on_merge_use_existing: bool
+    ) -> dict:
+        return {
+            "loginId": login_id,
+            "phone": phone,
+            "addToLoginIDs": add_to_login_ids,
+            "onMergeUseExisting": on_merge_use_existing,
+        }
```

### Comparing `descope-1.1.1/descope/authmethod/oauth.py` & `descope-1.5.0/descope/authmethod/oauth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.common import EndpointsV1, LoginOptions, validate_refresh_token_provided
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 
-class OAuth:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class OAuth(AuthBase):
     def start(
         self,
         provider: str,
         return_url: str = "",
         login_options: LoginOptions = None,
         refresh_token: str = None,
     ) -> dict:
```

### Comparing `descope-1.1.1/descope/authmethod/otp.py` & `descope-1.5.0/descope/authmethod/otp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,20 @@
+from descope._auth_base import AuthBase
 from descope.auth import Auth
 from descope.common import (
     REFRESH_SESSION_COOKIE_NAME,
     DeliveryMethod,
     EndpointsV1,
     LoginOptions,
     validate_refresh_token_provided,
 )
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 
-class OTP:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class OTP(AuthBase):
     def sign_in(
         self,
         method: DeliveryMethod,
         login_id: str,
         login_options: LoginOptions = None,
         refresh_token: str = None,
     ) -> str:
@@ -133,15 +129,22 @@
 
         resp = response.json()
         jwt_response = self._auth.generate_jwt_response(
             resp, response.cookies.get(REFRESH_SESSION_COOKIE_NAME, None)
         )
         return jwt_response
 
-    def update_user_email(self, login_id: str, email: str, refresh_token: str) -> str:
+    def update_user_email(
+        self,
+        login_id: str,
+        email: str,
+        refresh_token: str,
+        add_to_login_ids: bool = False,
+        on_merge_use_existing: bool = False,
+    ) -> str:
         """
         Update the email address of an end user, after verifying the authenticity of the end user using OTP.
 
         Args:
         login_id (str): The login ID of the user whose information is being updated
         email (str): The new email address. If an email address already exists for this end user, it will be overwritten
         refresh_token (str): The session's refresh token (used for verification)
@@ -154,43 +157,56 @@
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "Identifier cannot be empty"
             )
 
         Auth.validate_email(email)
 
         uri = EndpointsV1.update_user_email_otp_path
-        body = OTP._compose_update_user_email_body(login_id, email)
+        body = OTP._compose_update_user_email_body(
+            login_id, email, add_to_login_ids, on_merge_use_existing
+        )
         response = self._auth.do_post(uri, body, None, refresh_token)
         return Auth.extract_masked_address(response.json(), DeliveryMethod.EMAIL)
 
     def update_user_phone(
-        self, method: DeliveryMethod, login_id: str, phone: str, refresh_token: str
+        self,
+        method: DeliveryMethod,
+        login_id: str,
+        phone: str,
+        refresh_token: str,
+        add_to_login_ids: bool = False,
+        on_merge_use_existing: bool = False,
     ) -> str:
         """
         Update the phone number of an existing end user, after verifying the authenticity of the end user using OTP.
 
         Args:
         method (DeliveryMethod): The method to use for delivering the OTP verification code, for example phone or email
         login_id (str): The login ID of the user whose information is being updated
         phone (str): The new phone number. If a phone number already exists for this end user, it will be overwritten
         refresh_token (str): The session's refresh token (used for OTP verification)
+        add_to_login_ids (bool): Defaults to false, determine whether to add this email to the login ids of hte user or not
+        on_merge_use_existing (bool): Defaults to false, In case add_to_login_ids and there is such a user already
+            determine whether keep the existing user, or this new one
 
         Raise:
         AuthException: raised if OTP verification fails or if token verification fails
         """
 
         if not login_id:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "Identifier cannot be empty"
             )
 
         Auth.validate_phone(method, phone)
 
         uri = OTP._compose_update_phone_url(method)
-        body = OTP._compose_update_user_phone_body(login_id, phone)
+        body = OTP._compose_update_user_phone_body(
+            login_id, phone, add_to_login_ids, on_merge_use_existing
+        )
         response = self._auth.do_post(uri, body, None, refresh_token)
         return Auth.extract_masked_address(response.json(), DeliveryMethod.SMS)
 
     @staticmethod
     def _compose_signup_url(method: DeliveryMethod) -> str:
         return Auth.compose_url(EndpointsV1.sign_up_auth_otp_path, method)
 
@@ -228,13 +244,27 @@
         }
 
     @staticmethod
     def _compose_verify_code_body(login_id: str, code: str) -> dict:
         return {"loginId": login_id, "code": code}
 
     @staticmethod
-    def _compose_update_user_email_body(login_id: str, email: str) -> dict:
-        return {"loginId": login_id, "email": email}
+    def _compose_update_user_email_body(
+        login_id: str, email: str, add_to_login_ids: bool, on_merge_use_existing: bool
+    ) -> dict:
+        return {
+            "loginId": login_id,
+            "email": email,
+            "addToLoginIDs": add_to_login_ids,
+            "onMergeUseExisting": on_merge_use_existing,
+        }
 
     @staticmethod
-    def _compose_update_user_phone_body(login_id: str, phone: str) -> dict:
-        return {"loginId": login_id, "phone": phone}
+    def _compose_update_user_phone_body(
+        login_id: str, phone: str, add_to_login_ids: bool, on_merge_use_existing: bool
+    ) -> dict:
+        return {
+            "loginId": login_id,
+            "phone": phone,
+            "addToLoginIDs": add_to_login_ids,
+            "onMergeUseExisting": on_merge_use_existing,
+        }
```

### Comparing `descope-1.1.1/descope/authmethod/password.py` & `descope-1.5.0/descope/authmethod/password.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.common import REFRESH_SESSION_COOKIE_NAME, EndpointsV1
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 
-class Password:
-    _auth: Auth
-
-    def __init__(self, auth):
-        self._auth = auth
-
+class Password(AuthBase):
     def sign_up(self, login_id: str, password: str, user: dict = None) -> dict:
         """
         Sign up (create) a new user using a login ID and password.
             (optional) Include additional user metadata that you wish to save.
 
         Args:
         login_id (str): The login ID of the user being signed up
```

### Comparing `descope-1.1.1/descope/authmethod/saml.py` & `descope-1.5.0/descope/authmethod/saml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.common import EndpointsV1, LoginOptions, validate_refresh_token_provided
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 
-class SAML:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class SAML(AuthBase):
     def start(
         self,
         tenant: str,
         return_url: str = None,
         login_options: LoginOptions = None,
         refresh_token: str = None,
     ) -> dict:
```

### Comparing `descope-1.1.1/descope/authmethod/totp.py` & `descope-1.5.0/descope/authmethod/totp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.common import (
     REFRESH_SESSION_COOKIE_NAME,
     EndpointsV1,
     LoginOptions,
     validate_refresh_token_provided,
 )
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 
-class TOTP:
-    _auth: Auth
-
-    def __init__(self, auth):
-        self._auth = auth
-
+class TOTP(AuthBase):
     def sign_up(self, login_id: str, user: dict = None) -> dict:
         """
         Sign up (create) a new user using their email or phone number.
             (optional) Include additional user metadata that you wish to save.
 
         Args:
         login_id (str): The login ID of the user being validated
-        user (dict) optional: Preserve additional user metadata in the form of
+        user (dict) optional: Preserve additional user metadata in the form of,
              {"name": "Desmond Copeland", "phone": "2125551212", "email": "des@cope.com"}
 
         Return value (dict):
         Return dict in the format
              {"provisioningURL": "", "image": "", "key": ""}
         Includes 3 different ways to allow the user to save their credentials in
         their authenticator app, either by clicking the provisioning URL, scanning the QR
```

### Comparing `descope-1.1.1/descope/authmethod/webauthn.py` & `descope-1.5.0/descope/authmethod/webauthn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.common import (
     REFRESH_SESSION_COOKIE_NAME,
     EndpointsV1,
     LoginOptions,
     validate_refresh_token_provided,
 )
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 
-class WebAuthn:
-    _auth: Auth
-
-    def __init__(self, auth):
-        self._auth = auth
-
+class WebAuthn(AuthBase):
     def sign_up_start(self, login_id: str, origin: str, user: dict = None) -> dict:
         """
         Docs
         """
         if not login_id:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "Identifier cannot be empty"
```

### Comparing `descope-1.1.1/descope/common.py` & `descope-1.5.0/descope/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 DEFAULT_BASE_URL = "https://api.descope.com"  # pragma: no cover
+DEFAULT_TIMEOUT_SECONDS = 60
 
 PHONE_REGEX = """^(?:(?:\\(?(?:00|\\+)([1-4]\\d\\d|[1-9]\\d?)\\)?)?[\\-\\.\\ \\\\/]?)?((?:\\(?\\d{1,}\\)?[\\-\\.\\ \\\\/]?){0,})(?:[\\-\\.\\ \\\\/]?(?:#|ext\\.?|extension|x)[\\-\\.\\ \\\\/]?(\\d+))?$"""
 
 SESSION_COOKIE_NAME = "DS"
 REFRESH_SESSION_COOKIE_NAME = "DSR"
 
 SESSION_TOKEN_NAME = "sessionToken"
```

### Comparing `descope-1.1.1/descope/descope_client.py` & `descope-1.5.0/descope/descope_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 from descope.authmethod.magiclink import MagicLink  # noqa: F401
 from descope.authmethod.oauth import OAuth  # noqa: F401
 from descope.authmethod.otp import OTP  # noqa: F401
 from descope.authmethod.password import Password  # noqa: F401
 from descope.authmethod.saml import SAML  # noqa: F401
 from descope.authmethod.totp import TOTP  # noqa: F401
 from descope.authmethod.webauthn import WebAuthn  # noqa: F401
-from descope.common import EndpointsV1
+from descope.common import DEFAULT_TIMEOUT_SECONDS, EndpointsV1
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 from descope.mgmt import MGMT  # noqa: F401
 
 
 class DescopeClient:
     ALGORITHM_KEY = "alg"
 
     def __init__(
         self,
         project_id: str = None,
         public_key: str = None,
         skip_verify: bool = False,
         management_key: str = None,
+        timeout_seconds: float = DEFAULT_TIMEOUT_SECONDS,
     ):
-        auth = Auth(project_id, public_key, skip_verify, management_key)
+        auth = Auth(
+            project_id, public_key, skip_verify, management_key, timeout_seconds
+        )
         self._auth = auth
         self._mgmt = MGMT(auth)
         self._magiclink = MagicLink(auth)
         self._enchantedlink = EnchantedLink(auth)
         self._oauth = OAuth(auth)
         self._saml = SAML(auth)
         self._otp = OTP(auth)
```

### Comparing `descope-1.1.1/descope/exceptions.py` & `descope-1.5.0/descope/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,21 +29,23 @@
 class RateLimitException(Exception):
     def __init__(
         self,
         status_code: int = None,
         error_type: str = None,
         error_description: str = None,
         error_message: str = None,
-        rate_limit_parameters: dict = {},
+        rate_limit_parameters: dict = None,
         **kwargs,
     ):
         self.status_code = status_code
         self.error_type = error_type
         self.error_description = error_description
         self.error_message = error_message
-        self.rate_limit_parameters = rate_limit_parameters
+        self.rate_limit_parameters = (
+            {} if rate_limit_parameters is None else rate_limit_parameters
+        )
 
     def __repr__(self):
         return f"Error {self.__dict__}"
 
     def __str__(self):
         return str(self.__dict__)
```

### Comparing `descope-1.1.1/descope/management/access_key.py` & `descope-1.5.0/descope/management/access_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 from typing import List
 
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.management.common import (
     AssociatedTenant,
     MgmtV1,
     associated_tenants_to_dict,
 )
 
 
-class AccessKey:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class AccessKey(AuthBase):
     def create(
         self,
         name: str,
         expire_time: int = 0,
-        role_names: List[str] = [],
-        key_tenants: List[AssociatedTenant] = [],
+        role_names: List[str] = None,
+        key_tenants: List[AssociatedTenant] = None,
     ) -> dict:
         """
         Create a new access key.
 
         Args:
         name (str): Access key name.
         expire_time (int): Access key expiration. Leave at 0 to make it indefinite.
@@ -40,14 +35,17 @@
             }
         Containing the created access key information and its cleartext. The key cleartext will only be returned on creation.
         Make sure to save it securely.
 
         Raise:
         AuthException: raised if create operation fails
         """
+        role_names = [] if role_names is None else role_names
+        key_tenants = [] if key_tenants is None else key_tenants
+
         response = self._auth.do_post(
             MgmtV1.access_key_create_path,
             AccessKey._compose_create_body(name, expire_time, role_names, key_tenants),
             pswd=self._auth.management_key,
         )
         return response.json()
 
@@ -74,15 +72,15 @@
             {"id": id},
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def search_all_access_keys(
         self,
-        tenant_ids: List[str] = [],
+        tenant_ids: List[str] = None,
     ) -> dict:
         """
         Search all access keys.
 
         Args:
         tenant_ids (List[str]): Optional list of tenant IDs to filter by
 
@@ -90,14 +88,16 @@
         Return dict in the format
              {"keys": []}
         "keys" contains a list of all of the found users and their information
 
         Raise:
         AuthException: raised if search operation fails
         """
+        tenant_ids = [] if tenant_ids is None else tenant_ids
+
         response = self._auth.do_post(
             MgmtV1.access_keys_search_path,
             {"tenantIds": tenant_ids},
             pswd=self._auth.management_key,
         )
         return response.json()
```

### Comparing `descope-1.1.1/descope/management/common.py` & `descope-1.5.0/descope/management/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     user_delete_all_test_users_path = "/v1/mgmt/user/test/delete/all"
     user_load_path = "/v1/mgmt/user"
     users_search_path = "/v1/mgmt/user/search"
     user_update_status_path = "/v1/mgmt/user/update/status"
     user_update_email_path = "/v1/mgmt/user/update/email"
     user_update_phone_path = "/v1/mgmt/user/update/phone"
     user_update_name_path = "/v1/mgmt/user/update/name"
+    user_update_picture_path = "/v1/mgmt/user/update/picture"
+    user_update_custom_attribute_path = "/v1/mgmt/user/update/customAttribute"
     user_add_role_path = "/v1/mgmt/user/update/role/add"
     user_remove_role_path = "/v1/mgmt/user/update/role/remove"
     user_add_tenant_path = "/v1/mgmt/user/update/tenant/add"
     user_remove_tenant_path = "/v1/mgmt/user/update/tenant/remove"
     user_generate_otp_for_test_path = "/v1/mgmt/tests/generate/otp"
     user_generate_magic_link_for_test_path = "/v1/mgmt/tests/generate/magiclink"
     user_generate_enchanted_link_for_test_path = "/v1/mgmt/tests/generate/enchantedlink"
@@ -33,15 +35,15 @@
     access_keys_search_path = "/v1/mgmt/accesskey/search"
     access_key_update_path = "/v1/mgmt/accesskey/update"
     access_key_deactivate_path = "/v1/mgmt/accesskey/deactivate"
     access_key_activate_path = "/v1/mgmt/accesskey/activate"
     access_key_delete_path = "/v1/mgmt/accesskey/delete"
 
     # sso
-    sso_configure_path = "/v1/mgmt/sso/settings"
+    sso_settings_path = "/v1/mgmt/sso/settings"
     sso_metadata_path = "/v1/mgmt/sso/metadata"
     sso_mapping_path = "/v1/mgmt/sso/mapping"
 
     # jwt
     update_jwt_path = "/v1/mgmt/jwt/update"
 
     # permission
@@ -52,30 +54,38 @@
 
     # role
     role_create_path = "/v1/mgmt/role/create"
     role_update_path = "/v1/mgmt/role/update"
     role_delete_path = "/v1/mgmt/role/delete"
     role_load_all_path = "/v1/mgmt/role/all"
 
+    # flow
+    flow_import_path = "/v1/mgmt/flow/import"
+    flow_export_path = "/v1/mgmt/flow/export"
+
+    # theme
+    theme_import_path = "/v1/mgmt/theme/import"
+    theme_export_path = "/v1/mgmt/theme/export"
+
     # group
     group_load_all_path = "/v1/mgmt/group/all"
     group_load_all_for_member_path = "/v1/mgmt/group/member/all"
     group_load_all_group_members_path = "/v1/mgmt/group/members"
 
 
 class AssociatedTenant:
     """
     Represents a tenant association for a User or Access Key. The tenant_id is required to denote
     which tenant the user or access key belongs to. The role_names array is an optional list of
     roles for the user or access key in this specific tenant.
     """
 
-    def __init__(self, tenant_id: str, role_names: List[str] = []):
+    def __init__(self, tenant_id: str, role_names: List[str] = None):
         self.tenant_id = tenant_id
-        self.role_names = role_names
+        self.role_names = [] if role_names is None else role_names
 
 
 def associated_tenants_to_dict(associated_tenants: List[AssociatedTenant]) -> list:
     associated_tenant_list = []
     if associated_tenants:
         for associated_tenant in associated_tenants:
             associated_tenant_list.append(
```

### Comparing `descope-1.1.1/descope/management/group.py` & `descope-1.5.0/descope/management/group.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from typing import List
 
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.management.common import MgmtV1
 
 
-class Group:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class Group(AuthBase):
     def load_all_groups(
         self,
         tenant_id: str,
     ) -> dict:
         """
         Load all groups for a specific tenant id.
 
@@ -48,16 +43,16 @@
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def load_all_groups_for_members(
         self,
         tenant_id: str,
-        user_ids: List[str] = [],
-        login_ids: List[str] = [],
+        user_ids: List[str] = None,
+        login_ids: List[str] = None,
     ) -> dict:
         """
         Load all groups for the provided user IDs or login IDs.
 
         Args:
         tenant_id (str): Tenant ID to load groups from.
         user_ids (List[str]): Optional List of user IDs, with the format of "U2J5ES9S8TkvCgOvcrkpzUgVTEBM" (example), which can be found on the user's JWT.
@@ -79,14 +74,17 @@
                 }
             ]
         Containing the loaded groups information.
 
         Raise:
         AuthException: raised if load operation fails
         """
+        user_ids = [] if user_ids is None else user_ids
+        login_ids = [] if login_ids is None else login_ids
+
         response = self._auth.do_post(
             MgmtV1.group_load_all_for_member_path,
             {
                 "tenantId": tenant_id,
                 "loginIds": login_ids,
                 "userIds": user_ids,
             },
```

### Comparing `descope-1.1.1/descope/management/jwt.py` & `descope-1.5.0/descope/management/jwt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 from descope.management.common import MgmtV1
 
 
-class JWT:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class JWT(AuthBase):
     def update_jwt(self, jwt: str, custom_claims: dict) -> str:
         """
         Given a valid JWT, update it with custom claims, and update its authz claims as well
 
         Args:
         token (str): valid jwt.
         custom_claims (dict): Custom claims to add to JWT, system claims will be filtered out
```

### Comparing `descope-1.1.1/descope/management/permission.py` & `descope-1.5.0/descope/management/permission.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.management.common import MgmtV1
 
 
-class Permission:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class Permission(AuthBase):
     def create(
         self,
         name: str,
         description: str = None,
     ):
         """
         Create a new permission.
```

### Comparing `descope-1.1.1/descope/management/role.py` & `descope-1.5.0/descope/management/role.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from typing import List
 
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.management.common import MgmtV1
 
 
-class Role:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class Role(AuthBase):
     def create(
         self,
         name: str,
         description: str = None,
-        permission_names: List[str] = [],
+        permission_names: List[str] = None,
     ):
         """
         Create a new role.
 
         Args:
         name (str): role name.
         description (str): Optional description to briefly explain what this role allows.
         permission_names (List[str]): Optional list of names of permissions this role grants.
 
         Raise:
         AuthException: raised if creation operation fails
         """
+        permission_names = [] if permission_names is None else permission_names
+
         self._auth.do_post(
             MgmtV1.role_create_path,
             {
                 "name": name,
                 "description": description,
                 "permissionNames": permission_names,
             },
@@ -38,29 +35,30 @@
         )
 
     def update(
         self,
         name: str,
         new_name: str,
         description: str = None,
-        permission_names: List[str] = [],
+        permission_names: List[str] = None,
     ):
         """
         Update an existing role with the given various fields. IMPORTANT: All parameters are used as overrides
         to the existing role. Empty fields will override populated fields. Use carefully.
 
         Args:
         name (str): role name.
         new_name (str): role updated name.
         description (str): Optional description to briefly explain what this role allows.
         permission_names (List[str]): Optional list of names of permissions this role grants.
 
         Raise:
         AuthException: raised if update operation fails
         """
+        permission_names = [] if permission_names is None else permission_names
         self._auth.do_post(
             MgmtV1.role_update_path,
             {
                 "name": name,
                 "newName": new_name,
                 "description": description,
                 "permissionNames": permission_names,
```

### Comparing `descope-1.1.1/descope/management/sso_settings.py` & `descope-1.5.0/descope/management/sso_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.management.common import MgmtV1
 
 
 class RoleMapping:
     """Map IDP group names to the Descope role name"""
 
     def __init__(self, groups: List[str], role_name: str):
@@ -24,19 +24,37 @@
     ):
         self.name = name
         self.email = email
         self.phone_number = phone_number
         self.group = group
 
 
-class SSOSettings:
-    _auth: Auth
+class SSOSettings(AuthBase):
+    def get_settings(
+        self,
+        tenant_id: str,
+    ) -> dict:
+        """
+        Get SSO setting for the provided tenant_id.
+
+        Args:
+        tenant_id (str): The tenant ID of the desired SSO Settings
+
+        Return value (dict):
+        Containing the loaded SSO settings information.
 
-    def __init__(self, auth: Auth):
-        self._auth = auth
+        Raise:
+        AuthException: raised if configuration operation fails
+        """
+        response = self._auth.do_get(
+            MgmtV1.sso_settings_path,
+            {"tenantId": tenant_id},
+            pswd=self._auth.management_key,
+        )
+        return response.json()
 
     def configure(
         self,
         tenant_id: str,
         idp_url: str,
         entity_id: str,
         idp_cert: str,
@@ -54,15 +72,15 @@
         redirect_url (str): An Optional Redirect URL after successful authentication.
         domain (str): An optional domain used to associate users authenticating via SSO with this tenant
 
         Raise:
         AuthException: raised if configuration operation fails
         """
         self._auth.do_post(
-            MgmtV1.sso_configure_path,
+            MgmtV1.sso_settings_path,
             SSOSettings._compose_configure_body(
                 tenant_id, idp_url, entity_id, idp_cert, redirect_url, domain
             ),
             pswd=self._auth.management_key,
         )
 
     def configure_via_metadata(
@@ -85,28 +103,31 @@
             SSOSettings._compose_metadata_body(tenant_id, idp_metadata_url),
             pswd=self._auth.management_key,
         )
 
     def mapping(
         self,
         tenant_id: str,
-        role_mappings: List[RoleMapping] = [],
-        attribute_mapping: AttributeMapping = [],
+        role_mappings: List[RoleMapping] = None,
+        attribute_mapping: AttributeMapping = None,
     ):
         """
         Configure SSO role mapping from the IDP groups to the Descope roles.
 
         Args:
         tenant_id (str): The tenant ID to be configured
         role_mappings (List[RoleMapping]): A mapping between IDP groups and Descope roles.
         attribute_mapping (AttributeMapping): A mapping between IDP user attributes and descope attributes.
 
         Raise:
         AuthException: raised if configuration operation fails
         """
+        role_mappings = [] if role_mappings is None else role_mappings
+        attribute_mapping = [] if attribute_mapping is None else attribute_mapping
+
         self._auth.do_post(
             MgmtV1.sso_mapping_path,
             SSOSettings._compose_mapping_body(
                 tenant_id, role_mappings, attribute_mapping
             ),
             pswd=self._auth.management_key,
         )
```

### Comparing `descope-1.1.1/descope/management/tenant.py` & `descope-1.5.0/descope/management/tenant.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 from typing import List
 
-from descope.auth import Auth
+from descope._auth_base import AuthBase
 from descope.management.common import MgmtV1
 
 
-class Tenant:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class Tenant(AuthBase):
     def create(
         self,
         name: str,
         id: str = None,
-        self_provisioning_domains: List[str] = [],
+        self_provisioning_domains: List[str] = None,
     ) -> dict:
         """
         Create a new tenant with the given name. Tenant IDs are provisioned automatically, but can be provided
         explicitly if needed. Both the name and ID must be unique per project.
 
         Args:
         name (str): The tenant's name
@@ -29,41 +24,49 @@
         Return value (dict):
         Return dict in the format
              {"id": <id>}
 
         Raise:
         AuthException: raised if creation operation fails
         """
+        self_provisioning_domains = (
+            [] if self_provisioning_domains is None else self_provisioning_domains
+        )
+
         uri = MgmtV1.tenant_create_path
         response = self._auth.do_post(
             uri,
             Tenant._compose_create_update_body(name, id, self_provisioning_domains),
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def update(
         self,
         id: str,
         name: str,
-        self_provisioning_domains: List[str] = [],
+        self_provisioning_domains: List[str] = None,
     ):
         """
         Update an existing tenant with the given name and domains. IMPORTANT: All parameters are used as overrides
         to the existing tenant. Empty fields will override populated fields. Use carefully.
 
         Args:
         id (str): The ID of the tenant to update.
         name (str): Updated tenant name
         self_provisioning_domains (List[str]): An optional list of domain that are associated with this tenant.
             Users authenticating from these domains will be associated with this tenant.
 
         Raise:
         AuthException: raised if creation operation fails
         """
+        self_provisioning_domains = (
+            [] if self_provisioning_domains is None else self_provisioning_domains
+        )
+
         uri = MgmtV1.tenant_update_path
         self._auth.do_post(
             uri,
             Tenant._compose_create_update_body(name, id, self_provisioning_domains),
             pswd=self._auth.management_key,
         )
```

### Comparing `descope-1.1.1/descope/management/user.py` & `descope-1.5.0/descope/management/user.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,86 @@
-from typing import List
+from typing import List, Union
 
+from descope._auth_base import AuthBase
 from descope.auth import Auth
 from descope.common import DeliveryMethod
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 from descope.management.common import (
     AssociatedTenant,
     MgmtV1,
     associated_tenants_to_dict,
 )
 
 
-class User:
-    _auth: Auth
-
-    def __init__(self, auth: Auth):
-        self._auth = auth
-
+class User(AuthBase):
     def create(
         self,
         login_id: str,
         email: str = None,
         phone: str = None,
         display_name: str = None,
-        role_names: List[str] = [],
-        user_tenants: List[AssociatedTenant] = [],
+        role_names: List[str] = None,
+        user_tenants: List[AssociatedTenant] = None,
+        picture: str = None,
+        custom_attributes: dict = None,
     ) -> dict:
         """
         Create a new user. Users can have any number of optional fields, including email, phone number and authorization.
 
         Args:
         login_id (str): user login ID.
         email (str): Optional user email address.
         phone (str): Optional user phone number.
         display_name (str): Optional user display name.
         role_names (List[str]): An optional list of the user's roles without tenant association. These roles are
             mutually exclusive with the `user_tenant` roles.
         user_tenants (List[AssociatedTenant]): An optional list of the user's tenants, and optionally, their roles per tenant. These roles are
             mutually exclusive with the general `role_names`.
+        picture (str): Optional url for user picture
+        custom_attributes (dict): Optional, set the different custom attributes values of the keys that were previously configured in Descope console app
 
         Return value (dict):
         Return dict in the format
              {"user": {}}
         Containing the created user information.
 
         Raise:
         AuthException: raised if update operation fails
         """
+        role_names = [] if role_names is None else role_names
+        user_tenants = [] if user_tenants is None else user_tenants
+
         response = self._auth.do_post(
             MgmtV1.user_create_path,
             User._compose_create_body(
                 login_id,
                 email,
                 phone,
                 display_name,
                 role_names,
                 user_tenants,
                 False,
                 False,
+                picture,
+                custom_attributes,
             ),
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def create_test_user(
         self,
         login_id: str,
         email: str = None,
         phone: str = None,
         display_name: str = None,
-        role_names: List[str] = [],
-        user_tenants: List[AssociatedTenant] = [],
+        role_names: List[str] = None,
+        user_tenants: List[AssociatedTenant] = None,
+        picture: str = None,
+        custom_attributes: dict = None,
     ) -> dict:
         """
         Create a new test user.
         The login_id is required and will determine what the user will use to sign in.
         Make sure the login id is unique for test. All other fields are optional.
 
         Args:
@@ -81,105 +88,134 @@
         email (str): Optional user email address.
         phone (str): Optional user phone number.
         display_name (str): Optional user display name.
         role_names (List[str]): An optional list of the user's roles without tenant association. These roles are
             mutually exclusive with the `user_tenant` roles.
         user_tenants (List[AssociatedTenant]): An optional list of the user's tenants, and optionally, their roles per tenant. These roles are
             mutually exclusive with the general `role_names`.
+        picture (str): Optional url for user picture
+        custom_attributes (dict): Optional, set the different custom attributes values of the keys that were previously configured in Descope console app
 
         Return value (dict):
         Return dict in the format
              {"user": {}}
         Containing the created test user information.
 
         Raise:
         AuthException: raised if update operation fails
         """
+        role_names = [] if role_names is None else role_names
+        user_tenants = [] if user_tenants is None else user_tenants
+
         response = self._auth.do_post(
             MgmtV1.user_create_path,
             User._compose_create_body(
                 login_id,
                 email,
                 phone,
                 display_name,
                 role_names,
                 user_tenants,
                 False,
                 True,
+                picture,
+                custom_attributes,
             ),
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def invite(
         self,
         login_id: str,
         email: str = None,
         phone: str = None,
         display_name: str = None,
-        role_names: List[str] = [],
-        user_tenants: List[AssociatedTenant] = [],
+        role_names: List[str] = None,
+        user_tenants: List[AssociatedTenant] = None,
+        picture: str = None,
+        custom_attributes: dict = None,
     ) -> dict:
         """
         Create a new user and invite them via an email message.
 
         Functions exactly the same as the `create` function with the additional invitation
             behavior. See the documentation above for the general creation behavior.
 
         IMPORTANT: Since the invitation is sent by email, make sure either
             the email is explicitly set, or the login_id itself is an email address.
             You must configure the invitation URL in the Descope console prior to
             calling the method.
         """
+        role_names = [] if role_names is None else role_names
+        user_tenants = [] if user_tenants is None else user_tenants
+
         response = self._auth.do_post(
             MgmtV1.user_create_path,
             User._compose_create_body(
                 login_id,
                 email,
                 phone,
                 display_name,
                 role_names,
                 user_tenants,
                 True,
                 False,
+                picture,
+                custom_attributes,
             ),
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def update(
         self,
         login_id: str,
         email: str = None,
         phone: str = None,
         display_name: str = None,
-        role_names: List[str] = [],
-        user_tenants: List[AssociatedTenant] = [],
+        role_names: List[str] = None,
+        user_tenants: List[AssociatedTenant] = None,
+        picture: str = None,
+        custom_attributes: dict = None,
     ):
         """
         Update an existing user with the given various fields. IMPORTANT: All parameters are used as overrides
         to the existing user. Empty fields will override populated fields. Use carefully.
 
         Args:
         login_id (str): The login ID of the user to update.
         email (str): Optional user email address.
         phone (str): Optional user phone number.
         display_name (str): Optional user display name.
         role_names (List[str]): An optional list of the user's roles without tenant association. These roles are
             mutually exclusive with the `user_tenant` roles.
         user_tenants (List[AssociatedTenant]): An optional list of the user's tenants, and optionally, their roles per tenant. These roles are
             mutually exclusive with the general `role_names`.
+        picture (str): Optional url for user picture
+        custom_attributes (dict): Optional, set the different custom attributes values of the keys that were previously configured in Descope console app
 
         Raise:
         AuthException: raised if creation operation fails
         """
+        role_names = [] if role_names is None else role_names
+        user_tenants = [] if user_tenants is None else user_tenants
+
         self._auth.do_post(
             MgmtV1.user_update_path,
             User._compose_update_body(
-                login_id, email, phone, display_name, role_names, user_tenants, False
+                login_id,
+                email,
+                phone,
+                display_name,
+                role_names,
+                user_tenants,
+                False,
+                picture,
+                custom_attributes,
             ),
             pswd=self._auth.management_key,
         )
 
     def delete(
         self,
         login_id: str,
@@ -204,17 +240,16 @@
     ):
         """
         Delete all test users in the project. IMPORTANT: This action is irreversible. Use carefully.
 
         Raise:
         AuthException: raised if creation operation fails
         """
-        self._auth.do_post(
+        self._auth.do_delete(
             MgmtV1.user_delete_all_test_users_path,
-            {},
             pswd=self._auth.management_key,
         )
 
     def load(
         self,
         login_id: str,
     ) -> dict:
@@ -263,20 +298,21 @@
             {"userId": user_id},
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def search_all(
         self,
-        tenant_ids: List[str] = [],
-        role_names: List[str] = [],
+        tenant_ids: List[str] = None,
+        role_names: List[str] = None,
         limit: int = 0,
         page: int = 0,
         test_users_only: bool = False,
         with_test_user: bool = False,
+        custom_attributes: dict = None,
     ) -> dict:
         """
         Search all users.
 
         Args:
         tenant_ids (List[str]): Optional list of tenant IDs to filter by
         role_names (List[str]): Optional list of role names to filter by
@@ -289,34 +325,40 @@
         Return dict in the format
              {"users": []}
         "users" contains a list of all of the found users and their information
 
         Raise:
         AuthException: raised if search operation fails
         """
+        tenant_ids = [] if tenant_ids is None else tenant_ids
+        role_names = [] if role_names is None else role_names
+
         if limit < 0:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "limit must be non-negative"
             )
 
         if page < 0:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "page must be non-negative"
             )
+        body = {
+            "tenantIds": tenant_ids,
+            "roleNames": role_names,
+            "limit": limit,
+            "page": page,
+            "testUsersOnly": test_users_only,
+            "withTestUser": with_test_user,
+        }
+        if custom_attributes is not None:
+            body["customAttributes"] = custom_attributes
 
         response = self._auth.do_post(
             MgmtV1.users_search_path,
-            {
-                "tenantIds": tenant_ids,
-                "roleNames": role_names,
-                "limit": limit,
-                "page": page,
-                "testUsersOnly": test_users_only,
-                "withTestUser": with_test_user,
-            },
+            body=body,
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def activate(
         self,
         login_id: str,
@@ -448,14 +490,71 @@
         response = self._auth.do_post(
             MgmtV1.user_update_name_path,
             {"loginId": login_id, "displayName": display_name},
             pswd=self._auth.management_key,
         )
         return response.json()
 
+    def update_picture(
+        self,
+        login_id: str,
+        picture: str = None,
+    ) -> dict:
+        """
+        Update the picture for an existing user.
+
+        Args:
+        login_id (str): The login ID of the user to update.
+        picture (str): Optional url to user avatar. Leave empty to remove.
+
+        Return value (dict):
+        Return dict in the format
+             {"user": {}}
+        Containing the updated user information.
+
+        Raise:
+        AuthException: raised if the update operation fails
+        """
+        response = self._auth.do_post(
+            MgmtV1.user_update_picture_path,
+            {"loginId": login_id, "picture": picture},
+            pswd=self._auth.management_key,
+        )
+        return response.json()
+
+    def update_custom_attribute(
+        self, login_id: str, attribute_key: str, attribute_val: Union[str, int, bool]
+    ) -> dict:
+        """
+        Update a custom attribute of an existing user.
+
+        Args:
+        login_id (str): The login ID of the user to update.
+        attribute_key (str): The custom attribute that needs to be updated, this attribute needs to exists in Descope console app
+        attribute_val: The value to be updated
+
+        Return value (dict):
+        Return dict in the format
+             {"user": {}}
+        Containing the updated user information.
+
+        Raise:
+        AuthException: raised if the update operation fails
+        """
+        response = self._auth.do_post(
+            MgmtV1.user_update_custom_attribute_path,
+            {
+                "loginId": login_id,
+                "attributeKey": attribute_key,
+                "attributeValue": attribute_val,
+            },
+            pswd=self._auth.management_key,
+        )
+        return response.json()
+
     def add_roles(
         self,
         login_id: str,
         role_names: List[str],
     ) -> dict:
         """
         Add roles to a user without tenant association. Use add_tenant_roles
@@ -718,33 +817,47 @@
         email: str,
         phone: str,
         display_name: str,
         role_names: List[str],
         user_tenants: List[AssociatedTenant],
         invite: bool,
         test: bool,
+        picture: str,
+        custom_attributes: dict,
     ) -> dict:
         body = User._compose_update_body(
-            login_id, email, phone, display_name, role_names, user_tenants, test
+            login_id,
+            email,
+            phone,
+            display_name,
+            role_names,
+            user_tenants,
+            test,
+            picture,
+            custom_attributes,
         )
         body["invite"] = invite
         return body
 
     @staticmethod
     def _compose_update_body(
         login_id: str,
         email: str,
         phone: str,
         display_name: str,
         role_names: List[str],
         user_tenants: List[AssociatedTenant],
         test: bool,
+        picture: str,
+        custom_attributes: dict,
     ) -> dict:
         return {
             "loginId": login_id,
             "email": email,
             "phone": phone,
             "displayName": display_name,
             "roleNames": role_names,
             "userTenants": associated_tenants_to_dict(user_tenants),
             "test": test,
+            "picture": picture,
+            "customAttributes": custom_attributes,
         }
```

### Comparing `descope-1.1.1/descope/mgmt.py` & `descope-1.5.0/descope/mgmt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from descope.auth import Auth
 from descope.management.access_key import AccessKey  # noqa: F401
+from descope.management.flow import Flow  # noqa: F401
 from descope.management.group import Group  # noqa: F401
 from descope.management.jwt import JWT  # noqa: F401
 from descope.management.permission import Permission  # noqa: F401
 from descope.management.role import Role  # noqa: F401
 from descope.management.sso_settings import SSOSettings  # noqa: F401
 from descope.management.tenant import Tenant  # noqa: F401
 from descope.management.user import User  # noqa: F401
@@ -18,14 +19,15 @@
         self._user = User(auth)
         self._access_key = AccessKey(auth)
         self._sso = SSOSettings(auth)
         self._jwt = JWT(auth)
         self._permission = Permission(auth)
         self._role = Role(auth)
         self._group = Group(auth)
+        self._flow = Flow(auth)
 
     @property
     def tenant(self):
         return self._tenant
 
     @property
     def user(self):
@@ -50,7 +52,11 @@
     @property
     def role(self):
         return self._role
 
     @property
     def group(self):
         return self._group
+
+    @property
+    def flow(self):
+        return self._flow
```

### Comparing `descope-1.1.1/pyproject.toml` & `descope-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "descope"
-version = "1.1.1"
+version = "1.5.0"
 description = "Descope Python SDK"
 authors = ["Descope <info@descope.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://descope.com/"
 repository = "https://github.com/descope/python-sdk"
 documentation = "https://docs.descope.com"
@@ -23,24 +23,25 @@
 "Bug Tracker" = "https://github.com/descope/python-sdk/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = "2.28.2"
 PyJWT = "==2.6.0"
-cryptography = "==40.0.1"
+cryptography = "==40.0.2"
 email-validator = "==1.3.1"
 
 [tool.poetry.group.dev.dependencies]
-mock = "5.0.1"
+mock = "5.0.2"
 pre-commit = "2.21.0"
-Flask = "2.2.3"
+Flask = "2.2.5"
 flake8 = "5.0.4"
+flake8-bugbear = "22.12.6"
 pytest-cov = "4.0.0"
-pytest = "7.2.2"
+pytest = "7.3.1"
 black = "23.3.0"
 liccheck = "0.8.3"
 isort = "5.11.4"
 pep8-naming = "0.13.3"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
```

### Comparing `descope-1.1.1/PKG-INFO` & `descope-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descope
-Version: 1.1.1
+Version: 1.5.0
 Summary: Descope Python SDK
 Home-page: https://descope.com/
 License: MIT
 Author: Descope
 Author-email: info@descope.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyJWT (==2.6.0)
-Requires-Dist: cryptography (==40.0.1)
+Requires-Dist: cryptography (==40.0.2)
 Requires-Dist: email-validator (==1.3.1)
 Requires-Dist: requests (==2.28.2)
 Project-URL: Bug Tracker, https://github.com/descope/python-sdk/issues
 Project-URL: Documentation, https://docs.descope.com
 Project-URL: Repository, https://github.com/descope/python-sdk
 Description-Content-Type: text/markdown
 
@@ -586,14 +586,17 @@
 ```
 
 ### Manage SSO Setting
 
 You can manage SSO settings and map SSO group roles and user attributes.
 
 ```Python
+# You can get SSO settings for a tenant
+sso_settings_res = descope_client.mgmt.sso.get_settings("tenant-id")
+
 # You can configure SSO settings manually by setting the required fields directly
 descope_client.mgmt.sso.configure(
     tenant_id, # Which tenant this configuration is for
     idp_url="https://idp.com",
     entity_id="my-idp-entity-id",
     idp_cert="<your-cert-here>",
     redirect_url="https://your.domain.com", # Global redirection after successful authentication
@@ -677,14 +680,40 @@
 # Load all roles
 roles_resp = descope_client.mgmt.role.load_all()
 roles = roles_resp["roles"]
     for role in roles:
         # Do something
 ```
 
+### Manage Flows and Theme
+
+You can export and import your project flows and theme:
+
+```Python
+# Export a selected flow by id for the flow and matching screens.
+exported_flow_and_screens = descope_client.mgmt.flow.export_flow(
+    flow_id="sign-up-or-in",
+)
+
+# Import a given flow and screens to the flow matching the id provided.
+imported_flow_and_screens = descope_client.mgmt.flow.import_flow(
+    flow_id="sign-up-or-in",
+    flow={},
+    screens=[]
+)
+
+# Export your project theme.
+exported_theme = descope_client.mgmt.flow.export_theme()
+
+# Import a theme to your project.
+imported_theme = descope_client.mgmt.flow.import_flow(
+    theme={}
+)
+```
+
 ### Query SSO Groups
 
 You can query SSO groups:
 
 ```Python
 # Load all groups for a given tenant id
 groups_resp = descope_client.mgmt.group.load_all_groups(
```

