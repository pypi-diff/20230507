# Comparing `tmp/strawberry_django_auth-0.374.3.tar.gz` & `tmp/strawberry_django_auth-0.374.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_auth-0.374.3.tar", max compression
+gzip compressed data, was "strawberry_django_auth-0.374.4.tar", max compression
```

## Comparing `strawberry_django_auth-0.374.3.tar` & `strawberry_django_auth-0.374.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1075 2023-04-06 20:13:17.061743 strawberry_django_auth-0.374.3/LICENSE
--rw-r--r--   0        0        0     4043 2023-04-06 20:13:17.061743 strawberry_django_auth-0.374.3/README.md
--rw-r--r--   0        0        0       24 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/__init__.py
--rw-r--r--   0        0        0      168 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/admin.py
--rw-r--r--   0        0        0      215 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/apps.py
--rw-r--r--   0        0        0        0 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/captcha/__init__.py
--rw-r--r--   0        0        0     1267 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/captcha/captcha_factorty.py
--rw-r--r--   0        0        0     6602 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/captcha/create.py
--rw-r--r--   0        0        0    16724 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/captcha/fonts/Nehama.ttf
--rw-r--r--   0        0        0   221328 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
--rw-r--r--   0        0        0    45448 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/captcha/fonts/pltwide.ttf
--rwxr-xr-x   0        0        0    22768 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/captcha/fonts/stam.ttf
--rw-r--r--   0        0        0     3248 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/captcha/models.py
--rw-r--r--   0        0        0      448 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/captcha/types_.py
--rw-r--r--   0        0        0        0 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/__init__.py
--rw-r--r--   0        0        0     1995 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/constants.py
--rw-r--r--   0        0        0      724 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/directives.py
--rw-r--r--   0        0        0     1093 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/exceptions.py
--rw-r--r--   0        0        0      231 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/interfaces.py
--rw-r--r--   0        0        0     4549 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/middlewares.py
--rw-r--r--   0        0        0     1453 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/mixins.py
--rw-r--r--   0        0        0     1434 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/scalars.py
--rw-r--r--   0        0        0      857 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/types_.py
--rw-r--r--   0        0        0     3979 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/core/utils.py
--rw-r--r--   0        0        0        0 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/jwt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/jwt/tools.py
--rw-r--r--   0        0        0     7482 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/jwt/types_.py
--rw-r--r--   0        0        0     2969 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/migrations/__init__.py
--rw-r--r--   0        0        0     7322 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/models.py
--rw-r--r--   0        0        0        0 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/py.typed
--rw-r--r--   0        0        0      649 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/settings.py
--rw-r--r--   0        0        0     9830 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/settings_type.py
--rw-r--r--   0        0        0      171 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/templates/email/activation_email.html
--rw-r--r--   0        0        0       41 2023-04-06 20:13:17.109743 strawberry_django_auth-0.374.3/gqlauth/templates/email/activation_subject.txt
--rw-r--r--   0        0        0   176202 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
--rw-r--r--   0        0        0   100933 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
--rw-r--r--   0        0        0      162 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/templates/email/password_reset_email.html
--rw-r--r--   0        0        0       39 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/templates/email/password_reset_subject.txt
--rw-r--r--   0        0        0      160 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/templates/email/password_set_email.html
--rw-r--r--   0        0        0       37 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/templates/email/password_set_subject.txt
--rw-r--r--   0        0        0        0 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/__init__.py
--rw-r--r--   0        0        0     2177 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/arg_mutations.py
--rw-r--r--   0        0        0     1628 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/forms.py
--rw-r--r--   0        0        0     1218 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/helpers.py
--rw-r--r--   0        0        0     1104 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/queries.py
--rw-r--r--   0        0        0     2185 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/relay.py
--rw-r--r--   0        0        0    19054 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/resolvers.py
--rw-r--r--   0        0        0      450 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/signals.py
--rw-r--r--   0        0        0     2005 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/types_.py
--rw-r--r--   0        0        0      119 2023-04-06 20:13:17.113743 strawberry_django_auth-0.374.3/gqlauth/user/views.py
--rw-r--r--   0        0        0     3332 2023-04-06 20:13:30.838540 strawberry_django_auth-0.374.3/pyproject.toml
--rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 strawberry_django_auth-0.374.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-07 16:27:39.317448 strawberry_django_auth-0.374.4/LICENSE
+-rw-r--r--   0        0        0     3820 2023-05-07 16:27:39.317448 strawberry_django_auth-0.374.4/README.md
+-rw-r--r--   0        0        0       24 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/admin.py
+-rw-r--r--   0        0        0      215 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/apps.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/captcha/__init__.py
+-rw-r--r--   0        0        0     1267 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/captcha/captcha_factorty.py
+-rw-r--r--   0        0        0     6602 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/captcha/create.py
+-rw-r--r--   0        0        0    16724 2023-05-07 16:27:39.369448 strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/Nehama.ttf
+-rw-r--r--   0        0        0   221328 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/OpenSans-Semibold.ttf
+-rw-r--r--   0        0        0    45448 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/pltwide.ttf
+-rwxr-xr-x   0        0        0    22768 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/stam.ttf
+-rw-r--r--   0        0        0     3248 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/models.py
+-rw-r--r--   0        0        0      448 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/captcha/types_.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/__init__.py
+-rw-r--r--   0        0        0     1995 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/constants.py
+-rw-r--r--   0        0        0      724 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/directives.py
+-rw-r--r--   0        0        0     1093 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/exceptions.py
+-rw-r--r--   0        0        0      231 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/interfaces.py
+-rw-r--r--   0        0        0     4559 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/middlewares.py
+-rw-r--r--   0        0        0     1453 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/mixins.py
+-rw-r--r--   0        0        0     1516 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/scalars.py
+-rw-r--r--   0        0        0      857 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/types_.py
+-rw-r--r--   0        0        0     3979 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/jwt/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/jwt/tools.py
+-rw-r--r--   0        0        0     7498 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/jwt/types_.py
+-rw-r--r--   0        0        0     2969 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/migrations/__init__.py
+-rw-r--r--   0        0        0     7322 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/models.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/py.typed
+-rw-r--r--   0        0        0      649 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/settings.py
+-rw-r--r--   0        0        0     9830 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/settings_type.py
+-rw-r--r--   0        0        0      171 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/templates/email/activation_email.html
+-rw-r--r--   0        0        0       41 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/templates/email/activation_subject.txt
+-rw-r--r--   0        0        0   176202 2023-05-07 16:27:39.373448 strawberry_django_auth-0.374.4/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg
+-rw-r--r--   0        0        0   100933 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg
+-rw-r--r--   0        0        0      162 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/password_reset_email.html
+-rw-r--r--   0        0        0       39 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/password_reset_subject.txt
+-rw-r--r--   0        0        0      160 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/password_set_email.html
+-rw-r--r--   0        0        0       37 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/templates/email/password_set_subject.txt
+-rw-r--r--   0        0        0        0 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/__init__.py
+-rw-r--r--   0        0        0     2177 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/arg_mutations.py
+-rw-r--r--   0        0        0     1628 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/forms.py
+-rw-r--r--   0        0        0     1281 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/helpers.py
+-rw-r--r--   0        0        0     1104 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/queries.py
+-rw-r--r--   0        0        0     2277 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/relay.py
+-rw-r--r--   0        0        0    19509 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/resolvers.py
+-rw-r--r--   0        0        0      450 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/signals.py
+-rw-r--r--   0        0        0     2005 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/types_.py
+-rw-r--r--   0        0        0      119 2023-05-07 16:27:39.377448 strawberry_django_auth-0.374.4/gqlauth/user/views.py
+-rw-r--r--   0        0        0     3243 2023-05-07 16:27:57.249386 strawberry_django_auth-0.374.4/pyproject.toml
+-rw-r--r--   0        0        0     5340 1970-01-01 00:00:00.000000 strawberry_django_auth-0.374.4/PKG-INFO
```

### Comparing `strawberry_django_auth-0.374.3/LICENSE` & `strawberry_django_auth-0.374.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/README.md` & `strawberry_django_auth-0.374.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 ### Docs can be found [here](https://nrbnlulu.github.io/strawberry-django-auth/)
 
 ## Features
 
 * [x] Awesome docs!
-* [x] Captcha validation
+* [x] Captcha validation (with extra `strawberry-django-auth[captcha]`)
 * [x] Async/Sync supported!
 * [x] Works with default or custom user model
 * [x] Builtin JWT authentication using [PyJWT](https://github.com/jpadilla/pyjwt)
 * [x] User registration with email verification
 * [x] Retrieve/Update user
 * [x] Archive user
 * [x] Permanently delete user or make it inactive
@@ -47,31 +47,24 @@
 * [x] Passwordless registration
 
 
 ### Full schema features
 
 ```python
 
-@strawberry.type
-class AuthMutation:
-    # include here your mutations that interact with a user object from a token.
 
+@strawberry.type
+class Mutation:
     verify_token = mutations.VerifyToken.field
     update_account = mutations.UpdateAccount.field
     archive_account = mutations.ArchiveAccount.field
     delete_account = mutations.DeleteAccount.field
     password_change = mutations.PasswordChange.field
     swap_emails = mutations.SwapEmails.field
 
-@strawberry.type
-class Mutation:
-    @field(directives=[TokenRequired()])
-    def auth_entry(self) -> Union[AuthMutation, GQLAuthError]:
-        return AuthOutput(node=AuthMutation())
-
     # these are mutation that does not require authentication.
     captcha = Captcha.field
     token_auth = mutations.ObtainJSONWebToken.field
     register = mutations.Register.field
     verify_account = mutations.VerifyAccount.field
     resend_activation_email = mutations.ResendActivationEmail.field
     send_password_reset_email = mutations.SendPasswordResetEmail.field
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/captcha/captcha_factorty.py` & `strawberry_django_auth-0.374.4/gqlauth/captcha/captcha_factorty.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/captcha/create.py` & `strawberry_django_auth-0.374.4/gqlauth/captcha/create.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/captcha/fonts/Nehama.ttf` & `strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/Nehama.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/captcha/fonts/OpenSans-Semibold.ttf` & `strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/OpenSans-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/captcha/fonts/pltwide.ttf` & `strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/pltwide.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/captcha/fonts/stam.ttf` & `strawberry_django_auth-0.374.4/gqlauth/captcha/fonts/stam.ttf`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/captcha/models.py` & `strawberry_django_auth-0.374.4/gqlauth/captcha/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return obj
 
     def save(self, *args, **kwargs):
         self.text = self._format(self.text)
         super().save(*args, **kwargs)
 
     def validate(self, user_entry: str):
-        """validates input_.
+        """Validates input_.
 
         - if tried to validate more than 3 times obj will be deleted in the database
         - else increments by one
         - if reaches expiery date deletes the obj
         - returns bool for success state
         """
         if self.tries > app_settings.CAPTCHA_MAX_RETRIES:
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/core/constants.py` & `strawberry_django_auth-0.374.4/gqlauth/core/constants.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/core/directives.py` & `strawberry_django_auth-0.374.4/gqlauth/core/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/core/exceptions.py` & `strawberry_django_auth-0.374.4/gqlauth/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/core/middlewares.py` & `strawberry_django_auth-0.374.4/gqlauth/core/middlewares.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 if TYPE_CHECKING:
     pass
 
 
 class UserOrError:
     __slots__ = ("user", "error")
 
-    def __init__(self, user: USER_UNION = anon_user, error: Exception = None):
+    def __init__(self, user: USER_UNION = anon_user, error: Optional[Exception] = None):
         self.user = user
         self.error = error
 
     def authorized_user(self) -> Optional[USER_UNION]:
         if self.user.is_authenticated:  # real django user model always returns true.
             return self.user
         return None
@@ -103,15 +103,15 @@
             logic(request)
             return get_response(request)
 
     return middleware
 
 
 class JwtSchema(Schema):
-    """injects token to context."""
+    """Injects token to context."""
 
     def execute_sync(self, *args, **kwargs):
         self._inject_user_and_errors(kwargs)
         return super().execute_sync(*args, **kwargs)
 
     async def execute(self, *args, **kwargs):
         self._inject_user_and_errors(kwargs)
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/core/mixins.py` & `strawberry_django_auth-0.374.4/gqlauth/core/mixins.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/core/scalars.py` & `strawberry_django_auth-0.374.4/gqlauth/core/scalars.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import contextlib
 import typing
 from base64 import b64decode, b64encode
 
 import strawberry
-from PIL.Image import Image
 
 from gqlauth.core.exceptions import WrongUsage
 from gqlauth.core.utils import camelize
 
 
 def serialize_excpected_error(errors):
     if isinstance(errors, dict):
@@ -45,12 +45,15 @@
         ]
     }
     """,
     serialize=lambda value: serialize_excpected_error(value),
     parse_value=lambda value: value,
 )
 
-image = strawberry.scalar(
-    typing.NewType("image", Image),
-    serialize=lambda v: b64encode(v).decode("ascii"),
-    parse_value=lambda v: b64decode(v),
-)
+with contextlib.suppress(ImportError):
+    from PIL.Image import Image
+
+    image = strawberry.scalar(
+        typing.NewType("image", Image),
+        serialize=lambda v: b64encode(v).decode("ascii"),
+        parse_value=lambda v: b64decode(v),
+    )
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/core/types_.py` & `strawberry_django_auth-0.374.4/gqlauth/core/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/core/utils.py` & `strawberry_django_auth-0.374.4/gqlauth/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             cls.__annotations__[field.name] = field.type_annotation.annotation
         return cls
 
     return wrapped
 
 
 def inject_arguments(args: Dict[str, type]):
-    """injects arguments to the decorated resolver.
+    """Injects arguments to the decorated resolver.
 
     :param args: `dict[name, type]` of arguments to be injected.,
     """
 
     def wrapped(fn):
         sig = inspect.signature(fn)
         params = {
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/jwt/types_.py` & `strawberry_django_auth-0.374.4/gqlauth/jwt/types_.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             value = getattr(self, field.name)
             if isinstance(value, datetime):
                 ret[field.name] = value.strftime(app_settings.JWT_TIME_FORMAT)
         return ret
 
     @classmethod
     def from_dict(cls, data: dict) -> "TokenPayloadType":
-        for field in dataclasses.fields(cls):
+        for field in dataclasses.fields(cls):  # type: ignore
             value = data[field.name]
             if isinstance(value, str) and field.type is datetime:
                 data[field.name] = datetime.strptime(value, app_settings.JWT_TIME_FORMAT)
         return cls(**data)
 
 
 @strawberry.type(
@@ -107,15 +107,15 @@
         """Might raise TokenExpired."""
         token_type: TokenType = app_settings.JWT_DECODE_HANDLER(token)
         if token_type.is_expired():
             raise TokenExpired
         return token_type
 
     def get_user_instance(self) -> "UserProto":
-        """might raise not existed exception."""
+        """Might raise not existed exception."""
         pk_name = app_settings.JWT_PAYLOAD_PK.python_name
         query = {pk_name: getattr(self.payload, pk_name)}
         return USER_MODEL.objects.get(**query)  # type: ignore
 
 
 @strawberry.input
 @inject_fields(app_settings.LOGIN_FIELDS)
@@ -138,29 +138,29 @@
     token: Optional[TokenType] = None
     if app_settings.JWT_LONG_RUNNING_REFRESH_TOKEN:
         refresh_token: Optional[RefreshTokenType] = None
     errors: Optional[ExpectedErrorType] = None
 
     @classmethod
     def from_user(cls, user: "UserProto") -> "ObtainJSONWebTokenType":
-        """creates a new token and possibly a new refresh token based on the
+        """Creates a new token and possibly a new refresh token based on the
         user.
 
         *call this method only for trusted users.*
         """
         ret = ObtainJSONWebTokenType(
             success=True, user=cast(UserType, user), token=TokenType.from_user(user)
         )
         if app_settings.JWT_LONG_RUNNING_REFRESH_TOKEN:
             ret.refresh_token = cast(RefreshTokenType, RefreshToken.from_user(user))
         return ret
 
     @classmethod
     def authenticate(cls, info: Info, input_: ObtainJSONWebTokenInput) -> "ObtainJSONWebTokenType":
-        """return `ObtainJSONWebTokenType`. authenticates against django
+        """Return `ObtainJSONWebTokenType`. authenticates against django
         authentication backends.
 
         *creates a new token and possibly a refresh token.*
         """
         args = {
             USER_MODEL.USERNAME_FIELD: getattr(input_, USER_MODEL.USERNAME_FIELD),
             "password": input_.password,
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/migrations/0001_initial.py` & `strawberry_django_auth-0.374.4/gqlauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/models.py` & `strawberry_django_auth-0.374.4/gqlauth/models.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/settings.py` & `strawberry_django_auth-0.374.4/gqlauth/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/settings_type.py` & `strawberry_django_auth-0.374.4/gqlauth/settings_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,22 +161,22 @@
     function. This function will call each of our `AUTHENTICATION_BACKENDS`,
     And will return the user from one of them unless `PermissionDenied` was
     raised. You can pass any fields that would be accepted by your backends.
 
     **Note that `password field` is mandatory and cannot be removed.**
     """
     LOGIN_REQUIRE_CAPTCHA: bool = True
-    """whether login will require captcha verification."""
+    """Whether login will require captcha verification."""
     REGISTER_MUTATION_FIELDS: Set[StrawberryField] = field(
         default_factory=lambda: {email_field, username_field}
     )
     """Fields on register, plus password1 and password2, can be a dict like
     UPDATE_MUTATION_fieldS setting."""
     REGISTER_REQUIRE_CAPTCHA: bool = True
-    """whether register will require captcha verification."""
+    """Whether register will require captcha verification."""
     # captcha stuff
     #: captcha expiration delta.
     CAPTCHA_EXPIRATION_DELTA: timedelta = timedelta(seconds=120)
     #: max number of attempts for one captcha.
     CAPTCHA_MAX_RETRIES: int = 5
     CAPTCHA_TEXT_FACTORY: Callable = default_text_factory
     """A callable with no arguments that returns a string.
@@ -192,15 +192,15 @@
     CAPTCHA_SAVE_IMAGE: bool = False
     """If True, an png representation of the captcha will be saved under
     MEDIA_ROOT/captcha/<datetime>/<uuid>.png."""
     # optional fields on update account, can be list of fields
     UPDATE_MUTATION_FIELDS: Set[StrawberryField] = field(
         default_factory=lambda: {first_name_field, last_name_field}
     )
-    """fields on update account mutation."""
+    """Fields on update account mutation."""
 
     # email tokens
     EXPIRATION_ACTIVATION_TOKEN: timedelta = timedelta(days=7)
     EXPIRATION_PASSWORD_RESET_TOKEN: timedelta = timedelta(hours=1)
     EXPIRATION_PASSWORD_SET_TOKEN: timedelta = timedelta(hours=1)
     # email stuff
 
@@ -224,26 +224,26 @@
     ALLOW_DELETE_ACCOUNT: bool = False
     """If True, DeleteAcount mutation will permanently delete the user."""
     ALLOW_PASSWORDLESS_REGISTRATION: bool = False
     """Whether to allow registration with no password."""
     SEND_PASSWORD_SET_EMAIL: bool = False
     # JWT stuff
     JWT_SECRET_KEY: DjangoSetting[str] = DjangoSetting("SECRET_KEY")
-    """key used to sign the JWT token."""
+    """Key used to sign the JWT token."""
 
     JWT_ALGORITHM: str = "HS256"
     """Algorithm used for signing the token."""
     JWT_TIME_FORMAT: str = "%Y-%m-%dT%H:%M:%S.%f"
     """A valid 'strftime' string that will be used to encode the token
     payload."""
     JWT_PAYLOAD_HANDLER: Callable[["UserProto"], "TokenType"] = create_token_type
     """A custom function to generate the token datatype, its up to you to
     encode the token."""
     JWT_PAYLOAD_PK: StrawberryField = field(default_factory=lambda: username_field)
-    """field that will be used to generate the token from a user instance and
+    """Field that will be used to generate the token from a user instance and
     retrieve user based on the decoded token.
 
     *This filed must be unique in the database*
     """
     JWT_DECODE_HANDLER: Callable[[str], "TokenType"] = decode_jwt
 
     JWT_TOKEN_FINDER: Callable[[Union["HttpRequest", dict]], Optional[str]] = token_finder
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg` & `strawberry_django_auth-0.374.4/gqlauth/templates/email/images/gd4f267f778b22183ca1ded4dfae871eac04faaac23286dc27d9c228034ff735042cebd167fb684c47ea3bef8803094f5683f08a3728911b4b191f82a7c12de99_1280.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg` & `strawberry_django_auth-0.374.4/gqlauth/templates/email/images/windrader-wind-power-fichtelberg-wind-park.jpg`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/user/arg_mutations.py` & `strawberry_django_auth-0.374.4/gqlauth/user/arg_mutations.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/user/forms.py` & `strawberry_django_auth-0.374.4/gqlauth/user/forms.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/user/helpers.py` & `strawberry_django_auth-0.374.4/gqlauth/user/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import contextlib
 from typing import TYPE_CHECKING, Optional, Union
 
 from django.contrib.auth import get_user_model
 
-from gqlauth.captcha.models import Captcha as CaptchaModel
 from gqlauth.core.constants import Messages
 from gqlauth.core.types_ import MutationNormalOutput
 from gqlauth.core.utils import USER_UNION
 
 if TYPE_CHECKING:  # pragma: no cover
     from gqlauth.user.resolvers import ObtainJSONWebTokenInput, RegisterMixin
 
@@ -22,14 +22,18 @@
     assert isinstance(password, str)
     if user.check_password(password):
         return None
     errors = {password_arg: Messages.INVALID_PASSWORD}
     return MutationNormalOutput(success=False, errors=errors)
 
 
+with contextlib.suppress(ImportError):
+    from gqlauth.captcha.models import Captcha as CaptchaModel
+
+
 def check_captcha(input_: Union["RegisterMixin.RegisterInput", "ObtainJSONWebTokenInput"]):
     uuid = input_.identifier
     try:
         obj = CaptchaModel.objects.get(uuid=uuid)
     except CaptchaModel.DoesNotExist:
         return Messages.CAPTCHA_EXPIRED
     return obj.validate(input_.userEntry)
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/user/queries.py` & `strawberry_django_auth-0.374.4/gqlauth/user/queries.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/gqlauth/user/relay.py` & `strawberry_django_auth-0.374.4/gqlauth/user/relay.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import contextlib
+
 from gqlauth.core.mixins import RelayMixin
 from gqlauth.user.resolvers import (
     ArchiveAccountMixin,
-    Captcha,
     DeleteAccountMixin,
     ObtainJSONWebTokenMixin,
     PasswordChangeMixin,
     PasswordResetMixin,
     PasswordSetMixin,
     RefreshTokenMixin,
     RegisterMixin,
@@ -13,14 +14,16 @@
     RevokeTokenMixin,
     SendPasswordResetEmailMixin,
     UpdateAccountMixin,
     VerifyAccountMixin,
     VerifyTokenMixin,
 )
 
+with contextlib.suppress(ImportError):
+    from gqlauth.user.resolvers import Captcha
 __all__ = [
     "Register",
     "VerifyAccount",
     "ResendActivationEmail",
     "SendPasswordResetEmail",
     "PasswordSet",
     "PasswordReset",
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/user/resolvers.py` & `strawberry_django_auth-0.374.4/gqlauth/user/resolvers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 from dataclasses import asdict
 from smtplib import SMTPException
 from typing import Callable, cast
 from uuid import UUID
 
 import strawberry
 from django.contrib.auth import get_user_model
@@ -9,16 +10,14 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.signing import BadSignature, SignatureExpired
 from django.db import transaction
 from strawberry.field import StrawberryField
 from strawberry.types import Info
 from strawberry_django_plus import gql
 
-from gqlauth.captcha.models import Captcha as CaptchaModel
-from gqlauth.captcha.types_ import CaptchaType
 from gqlauth.core.constants import Messages, TokenAction
 from gqlauth.core.exceptions import (
     PasswordAlreadySetError,
     TokenScopeError,
     UserAlreadyVerified,
     UserNotVerified,
 )
@@ -62,40 +61,53 @@
                 if not user.status.verified:  # type: ignore
                     raise GQLAuthError(code=GQLAuthErrors.NOT_VERIFIED)
             except AttributeError:  # anonymous user has no status.
                 if user.is_anonymous:
                     raise GQLAuthError(code=GQLAuthErrors.UNAUTHENTICATED)
 
 
-class Captcha:
-    """Creates a brand-new captcha. Returns a base64 encoded string of the
-    captcha. And uuid representing the captcha id in the database. When you
-    will try to log in or register You will need submit that uuid With the user
-    input.
-
-    **The captcha will be invoked when the timeout expires**.
-    """
+class __CaptchaNotifyImportError:
+    @property
+    def field(self):
+        raise ImportError(
+            "you probably don't have pillow installed you'll need to add the [captcha] extra."
+        )
+
+
+Captcha = __CaptchaNotifyImportError()
 
-    @gql.django.field(description=__doc__)
-    def field(self) -> CaptchaType:
-        return CaptchaModel.create_captcha()
+with contextlib.suppress(ImportError):
+    from gqlauth.captcha.models import Captcha as CaptchaModel
+    from gqlauth.captcha.types_ import CaptchaType
+
+    class Captcha:  # type: ignore[no-redef]
+        """Creates a brand-new captcha. Returns a base64 encoded string of the
+        captcha. And uuid representing the captcha id in the database. When you
+        will try to log in or register You will need submit that uuid With the
+        user input.
+
+        **The captcha will be invoked when the timeout expires**.
+        """
+
+        @gql.django.field(description=__doc__)
+        def field(self) -> CaptchaType:
+            return CaptchaModel.create_captcha()
 
 
 class RegisterMixin(BaseMixin):
     """Register user with fields defined in the settings. If the email field of
     the user model is part of the registration fields (default), check if there
     is no user with that email.
 
-    If it exists, it does not register the user,
-    even if the email field is not defined as unique
-    (default of the default django user model).
-
-    When creating the user, it also creates a `UserStatus`
-    related to that user, making it possible to track
-    if the user is archived / verified.
+    If it exists, it does not register the user, even if the email field
+    is not defined as unique (default of the default django user model).
+
+    When creating the user, it also creates a `UserStatus` related to
+    that user, making it possible to track if the user is archived /
+    verified.
 
     Send account verification email.
 
     If allowed to not verified users login, return token.
     """
 
     @strawberry.input
@@ -118,15 +130,15 @@
         if app_settings.LOGIN_REQUIRE_CAPTCHA:
             check_res = check_captcha(input_)
             if check_res != Messages.CAPTCHA_VALID:
                 return MutationNormalOutput(success=False, errors={"captcha": check_res})
         email = getattr(input_, "email", False)
         try:
             with transaction.atomic():
-                f = cls.form(asdict(input_))
+                f = cls.form(asdict(input_))  # type: ignore
                 if f.is_valid():
                     user = f.save()
                     if email:
                         send_activation = app_settings.SEND_ACTIVATION_EMAIL is True
                         send_password_set = (
                             app_settings.ALLOW_PASSWORDLESS_REGISTRATION is True
                             and app_settings.SEND_PASSWORD_SET_EMAIL is True
@@ -169,20 +181,19 @@
         except (BadSignature, TokenScopeError):
             return MutationNormalOutput(success=False, errors=Messages.INVALID_TOKEN)
 
 
 class ResendActivationEmailMixin(BaseMixin):
     """Sends activation email.
 
-    It is called resend because theoretically
-    the first activation email was sent when
-    the user registered.
+    It is called resend because theoretically the first activation email
+    was sent when the user registered.
 
-    If there is no user with the requested email,
-    a successful response is returned.
+    If there is no user with the requested email, a successful response
+    is returned.
     """
 
     @strawberry.input
     class ResendActivationEmailInput:
         email: str
 
     @classmethod
@@ -202,19 +213,18 @@
         except UserAlreadyVerified:
             return MutationNormalOutput(success=False, errors={"email": Messages.ALREADY_VERIFIED})
 
 
 class SendPasswordResetEmailMixin(BaseMixin):
     """Send password reset email.
 
-    For non verified users, send an activation
-    email instead.
+    For non verified users, send an activation email instead.
 
-    If there is no user with the requested email,
-    a successful response is returned.
+    If there is no user with the requested email, a successful response
+    is returned.
     """
 
     @strawberry.input
     class SendPasswordResetEmailInput:
         email: str
 
     @classmethod
@@ -244,17 +254,16 @@
 
 
 class PasswordResetMixin(BaseMixin):
     """Change user password without old password.
 
     Receive the token that was sent by email.
 
-    If token and new passwords are valid, update
-    user password and in case of using refresh
-    tokens, revoke all of them.
+    If token and new passwords are valid, update user password and in
+    case of using refresh tokens, revoke all of them.
 
     Also, if user has not been verified yet, verify it.
     """
 
     @strawberry.input
     class PasswordResetInput:
         token: str
@@ -269,15 +278,15 @@
             payload = get_payload_from_token(
                 input_.token,
                 TokenAction.PASSWORD_RESET,
                 app_settings.EXPIRATION_PASSWORD_RESET_TOKEN,
             )
             user = UserModel._default_manager.get(**payload)
             status: "UserStatus" = getattr(user, "status")  # noqa: B009
-            f = cls.form(user, asdict(input_))
+            f = cls.form(user, asdict(input_))  # type: ignore
             if f.is_valid():
                 revoke_user_refresh_token(user)
                 user = f.save()  # type: ignore
                 if status.verified is False:
                     status.verified = True
                     status.save(update_fields=["verified"])
                     user_verified.send(sender=cls, user=user)
@@ -317,15 +326,15 @@
             token = input_.token
             payload = get_payload_from_token(
                 token,
                 TokenAction.PASSWORD_SET,
                 app_settings.EXPIRATION_PASSWORD_SET_TOKEN,
             )
             user = UserModel._default_manager.get(**payload)
-            f = cls.form(user, asdict(input_))
+            f = cls.form(user, asdict(input_))  # type: ignore
             if f.is_valid():
                 # Check if user has already set a password
                 if user.has_usable_password():
                     raise PasswordAlreadySetError
                 revoke_user_refresh_token(user)
                 user = f.save()  # type: ignore
                 status: "UserStatus" = getattr(user, "status")  # noqa: B009
@@ -343,22 +352,22 @@
         except PasswordAlreadySetError:
             return MutationNormalOutput(success=False, errors=Messages.PASSWORD_ALREADY_SET)
 
 
 class ObtainJSONWebTokenMixin(BaseMixin):
     """Obtain JSON web token for given user.
 
-    Allow to perform login with different fields,
-    The fields are defined on settings.
+    Allow to perform login with different fields, The fields are defined
+    on settings.
 
-    Not verified users can log in by default. This
-    can be changes on settings.
+    Not verified users can log in by default. This can be changes on
+    settings.
 
-    If user is archived, make it unarchived and
-    return `unarchiving=True` on OutputBase.
+    If user is archived, make it unarchived and return
+    `unarchiving=True` on OutputBase.
     """
 
     @classmethod
     def resolve_mutation(cls, info, input_: ObtainJSONWebTokenInput) -> ObtainJSONWebTokenType:
         if app_settings.LOGIN_REQUIRE_CAPTCHA:
             check_res = check_captcha(input_)
             if check_res != Messages.CAPTCHA_VALID:
@@ -394,16 +403,16 @@
         UserStatus.archive(user)
         revoke_user_refresh_token(user=user)
 
 
 class DeleteAccountMixin(ArchiveOrDeleteMixin):
     """Delete account permanently or make `user.is_active=False`.
 
-    The behavior is defined on settings.
-    Anyway user refresh tokens are revoked.
+    The behavior is defined on settings. Anyway user refresh tokens are
+    revoked.
 
     User must be verified and confirm password.
     """
 
     @classmethod
     def resolve_action(cls, user):
         if app_settings.ALLOW_DELETE_ACCOUNT:
@@ -426,17 +435,17 @@
     form = PasswordChangeForm
     REQUIRE_VERIFICATION = True
 
     @classmethod
     def resolve_mutation(cls, info: Info, input_: PasswordChangeInput) -> ObtainJSONWebTokenType:
         user = get_user(info)
         if error := confirm_password(user, input_):
-            return ObtainJSONWebTokenType(**asdict(error))
+            return ObtainJSONWebTokenType(**asdict(error))  # type: ignore
 
-        args = asdict(input_)
+        args = asdict(input_)  # type: ignore
         f = cls.form(user, args)  # type: ignore
         if f.is_valid():
             revoke_user_refresh_token(user)
             user = f.save()
             user_with_status = cast_to_status_user(user)
             return ObtainJSONWebTokenType.from_user(user_with_status)
         else:
@@ -457,15 +466,15 @@
     form = UpdateAccountForm
     REQUIRE_VERIFICATION = True
 
     @classmethod
     def resolve_mutation(cls, info, input_: UpdateAccountInput) -> MutationNormalOutput:
         user = get_user(info)
         f = cls.form(
-            asdict(input_),
+            asdict(input_),  # type: ignore
             instance=user,
         )
         if f.is_valid():
             f.save()
             return MutationNormalOutput(success=True)
         else:
             return MutationNormalOutput(success=False, errors=f.errors.get_json_data())
```

### Comparing `strawberry_django_auth-0.374.3/gqlauth/user/types_.py` & `strawberry_django_auth-0.374.4/gqlauth/user/types_.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_auth-0.374.3/pyproject.toml` & `strawberry_django_auth-0.374.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-auth"
-version = "0.374.3"
+version = "0.374.4"
 description = "Graphql authentication system with Strawberry for Django."
 license = "MIT"
 authors = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 readme = "README.md"
 classifiers = [
     'Environment :: Web Environment',
@@ -23,32 +23,31 @@
     { include = "gqlauth" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 Django = ">=3.2,<4.2"
 PyJWT = ">=2.6.0,<3.0"
-strawberry-graphql-django = { version = ">=0.2.5,<4.0", allow-prereleases = true }
-Pillow = "^9.2.0"
-strawberry-graphql = ">=0.128,<0.171.0"
 strawberry-django-plus = ">=1.25.2,<3.0.0"
+pillow = {version = "^9.5.0", extras = ["captcha"]}
+django-stubs = {extras = ["compatible-mypy"], version = "^4.2.0"}
+
+[tool.poetry.extras]
+captcha = ["pillow"]
 
 [tool.poetry.dev-dependencies]
 coverage = "^7.2"
 pytest = "^7.2"
 pytest-cov = "^4.0"
 pytest-django = "^4.0.0"
 types-cryptography = "^3.3.23"
 django-mock-queries = "^2.1.7"
 types-mock = "^5.0.0"
 types-jwt = "^0.1.0"
 types-pkg-resources = "^0.1.0"
-mypy = "^0.961"
-django-stubs = {extras = ["compatible-mypy"], version = "^1.12.0"}
-django-stubs-ext = "^0.7"
 mkdocs = "^1.3.0"
 mkdocs-markdownextradata-plugin = "^0.2.5"
 mkdocs-material = "^8.5.4"
 mkdocs-minify-plugin = "^0.5.0"
 pymdown-extensions = "^9.9"
 Markdown = "^3.4.1"
 Faker = "^18.2.0"
```

### Comparing `strawberry_django_auth-0.374.3/PKG-INFO` & `strawberry_django_auth-0.374.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-auth
-Version: 0.374.3
+Version: 0.374.4
 Summary: Graphql authentication system with Strawberry for Django.
 License: MIT
 Author: Nir.J Benlulu
 Author-email: nrbnlulu@gmail.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -20,20 +20,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: captcha
 Requires-Dist: Django (>=3.2,<4.2)
-Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: PyJWT (>=2.6.0,<3.0)
+Requires-Dist: django-stubs[compatible-mypy] (>=4.2.0,<5.0.0)
+Requires-Dist: pillow[captcha] (>=9.5.0,<10.0.0) ; extra == "captcha"
 Requires-Dist: strawberry-django-plus (>=1.25.2,<3.0.0)
-Requires-Dist: strawberry-graphql (>=0.128,<0.171.0)
-Requires-Dist: strawberry-graphql-django (>=0.2.5,<4.0)
 Project-URL: Documentation, https://nrbnlulu.github.io/strawberry-django-auth/
 Project-URL: Homepage, https://github.com/nrbnlulu/strawberry-django-auth
 Description-Content-Type: text/markdown
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/nrbnlulu/strawberry-django-auth/tests.yml?label=Tests&style=for-the-badge)](https://github.com/nrbnlulu/strawberry-django-auth/actions/workflows/tests.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/nrbnlulu/strawberry-django-auth?style=for-the-badge)](https://app.codecov.io/gh/nrbnlulu/strawberry-django-auth)
 [![Pypi](https://img.shields.io/pypi/v/strawberry-django-auth.svg?style=for-the-badge&logo=appveyor)](https://pypi.org/project/strawberry-django-auth/)
@@ -60,15 +60,15 @@
 
 
 ### Docs can be found [here](https://nrbnlulu.github.io/strawberry-django-auth/)
 
 ## Features
 
 * [x] Awesome docs!
-* [x] Captcha validation
+* [x] Captcha validation (with extra `strawberry-django-auth[captcha]`)
 * [x] Async/Sync supported!
 * [x] Works with default or custom user model
 * [x] Builtin JWT authentication using [PyJWT](https://github.com/jpadilla/pyjwt)
 * [x] User registration with email verification
 * [x] Retrieve/Update user
 * [x] Archive user
 * [x] Permanently delete user or make it inactive
@@ -83,31 +83,24 @@
 * [x] Passwordless registration
 
 
 ### Full schema features
 
 ```python
 
-@strawberry.type
-class AuthMutation:
-    # include here your mutations that interact with a user object from a token.
 
+@strawberry.type
+class Mutation:
     verify_token = mutations.VerifyToken.field
     update_account = mutations.UpdateAccount.field
     archive_account = mutations.ArchiveAccount.field
     delete_account = mutations.DeleteAccount.field
     password_change = mutations.PasswordChange.field
     swap_emails = mutations.SwapEmails.field
 
-@strawberry.type
-class Mutation:
-    @field(directives=[TokenRequired()])
-    def auth_entry(self) -> Union[AuthMutation, GQLAuthError]:
-        return AuthOutput(node=AuthMutation())
-
     # these are mutation that does not require authentication.
     captcha = Captcha.field
     token_auth = mutations.ObtainJSONWebToken.field
     register = mutations.Register.field
     verify_account = mutations.VerifyAccount.field
     resend_activation_email = mutations.ResendActivationEmail.field
     send_password_reset_email = mutations.SendPasswordResetEmail.field
```

