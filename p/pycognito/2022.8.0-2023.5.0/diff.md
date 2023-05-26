# Comparing `tmp/pycognito-2022.8.0.tar.gz` & `tmp/pycognito-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycognito-2022.8.0.tar", last modified: Mon Aug  1 11:17:00 2022, max compression
+gzip compressed data, was "pycognito-2023.5.0.tar", last modified: Fri May 26 13:41:56 2023, max compression
```

## Comparing `pycognito-2022.8.0.tar` & `pycognito-2023.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 11:17:00.653770 pycognito-2022.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-01 11:16:47.000000 pycognito-2022.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    21828 2022-08-01 11:17:00.653770 pycognito-2022.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20971 2022-08-01 11:16:47.000000 pycognito-2022.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 11:17:00.653770 pycognito-2022.8.0/pycognito/
--rw-r--r--   0 runner    (1001) docker     (121)    36523 2022-08-01 11:16:47.000000 pycognito-2022.8.0/pycognito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12260 2022-08-01 11:16:47.000000 pycognito-2022.8.0/pycognito/aws_srp.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-08-01 11:16:47.000000 pycognito-2022.8.0/pycognito/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-08-01 11:16:47.000000 pycognito-2022.8.0/pycognito/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-01 11:17:00.653770 pycognito-2022.8.0/pycognito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21828 2022-08-01 11:17:00.000000 pycognito-2022.8.0/pycognito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-08-01 11:17:00.000000 pycognito-2022.8.0/pycognito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 11:17:00.000000 pycognito-2022.8.0/pycognito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-01 11:17:00.000000 pycognito-2022.8.0/pycognito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-01 11:17:00.000000 pycognito-2022.8.0/pycognito.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-01 11:17:00.000000 pycognito-2022.8.0/pycognito.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-08-01 11:17:00.653770 pycognito-2022.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-08-01 11:16:47.000000 pycognito-2022.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:41:56.079230 pycognito-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 13:41:45.000000 pycognito-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-05-26 13:41:56.079230 pycognito-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-05-26 13:41:45.000000 pycognito-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:41:56.079230 pycognito-2023.5.0/pycognito/
+-rw-r--r--   0 runner    (1001) docker     (123)    37205 2023-05-26 13:41:45.000000 pycognito-2023.5.0/pycognito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-05-26 13:41:45.000000 pycognito-2023.5.0/pycognito/aws_srp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-26 13:41:45.000000 pycognito-2023.5.0/pycognito/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-26 13:41:45.000000 pycognito-2023.5.0/pycognito/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:41:56.079230 pycognito-2023.5.0/pycognito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-05-26 13:41:56.000000 pycognito-2023.5.0/pycognito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-26 13:41:56.000000 pycognito-2023.5.0/pycognito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:41:56.000000 pycognito-2023.5.0/pycognito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 13:41:56.000000 pycognito-2023.5.0/pycognito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 13:41:56.000000 pycognito-2023.5.0/pycognito.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:41:56.000000 pycognito-2023.5.0/pycognito.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-26 13:41:56.083230 pycognito-2023.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-26 13:41:45.000000 pycognito-2023.5.0/setup.py
```

### Comparing `pycognito-2022.8.0/LICENSE` & `pycognito-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycognito-2022.8.0/PKG-INFO` & `pycognito-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pycognito
-Version: 2022.8.0
+Version: 2023.5.0
 Summary: Python class to integrate Boto3's Cognito client so it is easy to login users. With SRP support.
 Home-page: https://github.com/pvizeli/pycognito
+Download-URL: https://github.com/pvizeli/pycognito/tarball/2023.5.0
 Author: Pascal Vizeli
 Author-email: pvizeli@syshack.ch
 License: Apache License 2.0
-Download-URL: https://github.com/pvizeli/pycognito/tarball/2022.08.0
 Keywords: aws,cognito,api,gateway,serverless
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
@@ -713,9 +712,7 @@
   user_pool_id='eu-west-1_1234567',
   client_id='4dn6jbcbhqcofxyczo3ms9z4cc',
   user_pool_region='eu-west-1',
 )
 
 response = requests.get('http://test.com', auth=auth)
 ```
-
-
```

### Comparing `pycognito-2022.8.0/README.md` & `pycognito-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pycognito-2022.8.0/pycognito/__init__.py` & `pycognito-2023.5.0/pycognito/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,22 @@
     """
     if attr_map is None:
         attr_map = {}
     for key, value in attr_map.items():
         if value in attributes.keys():
             attributes[key] = attributes.pop(value)
 
-    return [{"Name": key, "Value": value} for key, value in attributes.items()]
+    def normalize(val):
+        if isinstance(val, bool):
+            return "true" if val else "false"
+        return val
+
+    return [
+        {"Name": key, "Value": normalize(value)} for key, value in attributes.items()
+    ]
 
 
 def camel_to_snake(camel_str):
     """
     :param camel_str: string
     :return: string converted from a CamelCase to a snake_case
     """
@@ -145,26 +152,28 @@
         refresh_token=None,
         access_token=None,
         client_secret=None,
         access_key=None,
         secret_key=None,
         session=None,
         botocore_config=None,
+        boto3_client_kwargs=None,
     ):
         """
         :param user_pool_id: Cognito User Pool ID
         :param client_id: Cognito User Pool Application client ID
         :param username: User Pool username
         :param id_token: ID Token returned by authentication
         :param refresh_token: Refresh Token returned by authentication
         :param access_token: Access Token returned by authentication
         :param access_key: AWS IAM access key
         :param secret_key: AWS IAM secret key
         :param session: Boto3 client session
         :param botocore_config: Botocore Config object for the client
+        :param boto3_client_kwargs: Keyword args to pass to Boto3 for client creation
         """
 
         self.user_pool_id = user_pool_id
         self.client_id = client_id
         self.user_pool_region = (
             user_pool_region if user_pool_region else self.user_pool_id.split("_")[0]
         )
@@ -177,44 +186,50 @@
         self.id_claims = None
         self.access_claims = None
         self.custom_attributes = None
         self.base_attributes = None
         self.pool_jwk = None
         self.mfa_tokens = None
 
-        boto3_client_kwargs = {}
+        if not boto3_client_kwargs:
+            boto3_client_kwargs = {}
         if access_key and secret_key:
             boto3_client_kwargs["aws_access_key_id"] = access_key
             boto3_client_kwargs["aws_secret_access_key"] = secret_key
+        self.pool_domain_url = boto3_client_kwargs.get("endpoint_url", None)
+
         if self.user_pool_region:
             boto3_client_kwargs["region_name"] = self.user_pool_region
         if botocore_config:
             boto3_client_kwargs["config"] = botocore_config
 
         if session:
             self.client = session.client("cognito-idp", **boto3_client_kwargs)
         else:
             self.client = boto3.client("cognito-idp", **boto3_client_kwargs)
 
     @property
     def user_pool_url(self):
+        if self.pool_domain_url:
+            return f"{self.pool_domain_url}/{self.user_pool_id}"
+
         return f"https://cognito-idp.{self.user_pool_region}.amazonaws.com/{self.user_pool_id}"
 
     def get_keys(self):
         if self.pool_jwk:
             return self.pool_jwk
 
         # Check for the dictionary in environment variables.
         pool_jwk_env = env("COGNITO_JWKS", {}, var_type="dict")
         if pool_jwk_env:
             self.pool_jwk = pool_jwk_env
         # If it is not there use the requests library to get it
         else:
             self.pool_jwk = requests.get(
-                f"{self.user_pool_url}/.well-known/jwks.json"
+                f"{self.user_pool_url}/.well-known/jwks.json", timeout=15
             ).json()
         return self.pool_jwk
 
     def get_key(self, kid):
         keys = self.get_keys().get("keys")
         key = list(filter(lambda x: x.get("kid") == kid, keys))
         return key[0]
@@ -263,22 +278,22 @@
         setattr(self, f"{token_use}_claims", verified)
         return verified
 
     def get_user_obj(
         self, username=None, attribute_list=None, metadata=None, attr_map=None
     ):
         """
-        Returns the specified
+        Returns the specified user
         :param username: Username of the user
         :param attribute_list: List of tuples that represent the user's
             attributes as returned by the admin_get_user or get_user boto3 methods
         :param metadata: Metadata about the user
         :param attr_map: Dictionary that maps the Cognito attribute names to
         what we'd like to display to the users
-        :return:
+        :return: dictionary of the Cognito user response
         """
         return self.user_class(
             username=username,
             attribute_list=attribute_list,
             cognito_obj=self,
             metadata=metadata,
             attr_map=attr_map,
@@ -333,15 +348,15 @@
             custom_attributes[new_key] = value
 
         self.custom_attributes = custom_attributes
 
     def register(self, username, password, attr_map=None, client_metadata=None):
         """
         Register the user. Other base attributes from AWS Cognito User Pools
-        are  address, birthdate, email, family_name (last name), gender,
+        are address, birthdate, email, family_name (last name), gender,
         given_name (first name), locale, middle_name, name, nickname,
         phone_number, picture, preferred_username, profile, zoneinfo,
         updated at, website
         :param username: User Pool username
         :param password: User Pool password
         :param attr_map: Attribute map to Cognito's attributes
         :param client_metadata: Metadata about the user that will be used for ClientMetadata
@@ -520,15 +535,15 @@
 
     def get_user(self, attr_map=None):
         """
         Returns a UserObj (or whatever the self.user_class is) by using the
         user's access token.
         :param attr_map: Dictionary map from Cognito attributes to attribute
         names we would like to show to our users
-        :return:
+        :return: UserObj dictionary
         """
         user = self.client.get_user(AccessToken=self.access_token)
 
         user_metadata = {
             "username": user.get("Username"),
             "id_token": self.id_token,
             "access_token": self.access_token,
@@ -571,23 +586,25 @@
         ]
 
     def admin_get_user(self, attr_map=None):
         """
         Get the user's details using admin super privileges.
         :param attr_map: Dictionary map from Cognito attributes to attribute
         names we would like to show to our users
-        :return: UserObj object
+        :return: UserObj dictionary
         """
         user = self.client.admin_get_user(
             UserPoolId=self.user_pool_id, Username=self.username
         )
         user_metadata = {
             "enabled": user.get("Enabled"),
             "user_status": user.get("UserStatus"),
             "username": user.get("Username"),
+            "create_date": user.get("UserCreateDate"),
+            "modified_date": user.get("UserLastModifiedDate"),
             "id_token": self.id_token,
             "access_token": self.access_token,
             "refresh_token": self.refresh_token,
         }
         return self.get_user_obj(
             username=self.username,
             attribute_list=user.get("UserAttributes"),
@@ -603,61 +620,62 @@
         attr_map=None,
         **kwargs,
     ):
         """
         Create a user using admin super privileges.
         :param username: User Pool username
         :param temporary_password: The temporary password to give the user.
-        Leave blank to make Cognito generate a temporary password for the user.
+        Pass None or omit this to make Cognito generate a temporary password for the user.
         :param additional_kwargs: Dictionary with request params, such as MessageAction.
         :param attr_map: Attribute map to Cognito's attributes
         :param kwargs: Additional User Pool attributes
         :return response: Response from Cognito
         """
         if additional_kwargs is None:
             additional_kwargs = {}
+        if temporary_password:
+            additional_kwargs["TemporaryPassword"] = temporary_password
         response = self.client.admin_create_user(
             UserPoolId=self.user_pool_id,
             Username=username,
             UserAttributes=dict_to_cognito(kwargs, attr_map),
-            TemporaryPassword=temporary_password,
             **additional_kwargs,
         )
         kwargs.update(username=username)
         self._set_attributes(response, kwargs)
 
         response.pop("ResponseMetadata")
         return response
 
     def send_verification(self, attribute="email"):
         """
         Sends the user an attribute verification code for the specified attribute name.
-        :param attribute: Attribute to confirm
+        :param attribute: Attribute to confirm. Defaults to "email"
         """
         self.check_token()
         self.client.get_user_attribute_verification_code(
             AccessToken=self.access_token, AttributeName=attribute
         )
 
     def validate_verification(self, confirmation_code, attribute="email"):
         """
         Verifies the specified user attributes in the user pool.
         :param confirmation_code: Code sent to user upon intiating verification
-        :param attribute: Attribute to confirm
+        :param attribute: Attribute to confirm. Defaults to "email"
         """
         self.check_token()
         return self.client.verify_user_attribute(
             AccessToken=self.access_token,
             AttributeName=attribute,
             Code=confirmation_code,
         )
 
     def renew_access_token(self):
         """
-        Sets a new access token on the User using the refresh token.
+        Sets a new access token on the User using the cached refresh token.
         """
         auth_params = {"REFRESH_TOKEN": self.refresh_token}
         self._add_secret_hash(auth_params, "SECRET_HASH")
         refresh_response = self.client.initiate_auth(
             ClientId=self.client_id,
             AuthFlow="REFRESH_TOKEN_AUTH",
             AuthParameters=auth_params,
@@ -669,33 +687,33 @@
         Sends a verification code to the user to use to change their password.
         """
         params = {"ClientId": self.client_id, "Username": self.username}
         self._add_secret_hash(params, "SecretHash")
         self.client.forgot_password(**params)
 
     def delete_user(self):
-
         self.client.delete_user(AccessToken=self.access_token)
 
     def admin_delete_user(self):
         self.client.admin_delete_user(
             UserPoolId=self.user_pool_id, Username=self.username
         )
 
     def admin_reset_password(self, username, client_metadata=None):
+        if client_metadata is None:
+            client_metadata = {}
         self.client.admin_reset_user_password(
             UserPoolId=self.user_pool_id,
             Username=username,
             ClientMetadata=client_metadata,
         )
 
     def confirm_forgot_password(self, confirmation_code, password):
         """
-        Allows a user to enter a code provided when they reset their password
-        to update their password.
+        Allows a user to provide their verification code and choose a new password.
         :param confirmation_code: The confirmation code sent by a user's request
         to retrieve a forgotten password
         :param password: New password
         """
         params = {
             "ClientId": self.client_id,
             "Username": self.username,
@@ -742,39 +760,38 @@
             self.refresh_token = tokens["AuthenticationResult"]["RefreshToken"]
         self.token_type = tokens["AuthenticationResult"]["TokenType"]
 
     def _set_attributes(self, response, attribute_dict):
         """
         Set user attributes based on response code
         :param response: HTTP response from Cognito
-        :attribute dict: Dictionary of attribute name and values
+        :param attribute_dict: Dictionary of attribute names and values
         """
         status_code = response.get(
             "HTTPStatusCode", response["ResponseMetadata"]["HTTPStatusCode"]
         )
         if status_code == 200:
             for key, value in attribute_dict.items():
                 setattr(self, key, value)
 
     def get_group(self, group_name):
         """
-        Get a group by a name
+        Get a group by name
         :param group_name: name of a group
         :return: instance of the self.group_class
         """
         response = self.client.get_group(
             GroupName=group_name, UserPoolId=self.user_pool_id
         )
         return self.get_group_obj(response.get("Group"))
 
     def get_groups(self):
         """
-        Returns all groups for a user pool. Returns instances of the
-        self.group_class.
-        :return: list of instances
+        Returns all groups for a user pool.
+        :return: list of instances of self.group_class
         """
         response = self.client.list_groups(UserPoolId=self.user_pool_id)
         return [self.get_group_obj(group_data) for group_data in response.get("Groups")]
 
     def admin_add_user_to_group(self, username, group_name):
         """
         Add the user to the specified group
@@ -801,15 +818,15 @@
             GroupName=group_name,
         )
 
     def admin_list_groups_for_user(self, username):
         """
         Get the list of groups a user belongs to
         :param username:
-        :return: List
+        :return: List of group objects
         """
 
         def process_groups_response(groups_response):
             groups = []
             for group_dict in groups_response["Groups"]:
                 groups.append(group_dict["GroupName"])
             return groups
@@ -846,15 +863,15 @@
         """
         Disable a user
         :param username:
         :return:
         """
         self.client.admin_disable_user(
             UserPoolId=self.user_pool_id,
-            Username=self.username,
+            Username=username,
         )
 
     def admin_create_identity_provider(
         self, pool_id, provider_name, provider_type, provider_details, **kwargs
     ):
         """
         Creates an identity provider
@@ -870,15 +887,15 @@
             ProviderType=provider_type,
             ProviderDetails=provider_details,
             **kwargs,
         )
 
     def admin_describe_identity_provider(self, pool_id, provider_name):
         """
-        Updates an existing identity provider
+        Describes an existing identity provider
         :param pool_id: The user pool ID
         :param provider_name: The identity provider name
         :return: dict of identity provider
         """
         return self.client.describe_identity_provider(
             UserPoolId=pool_id, ProviderName=provider_name
         )
@@ -918,22 +935,22 @@
             UserPoolId=pool_id,
             ClientId=client_id,
             **kwargs,
         )
 
     def associate_software_token(self):
         """
-        Get the SecretCode used for Software Token. SecretCode use to set up Software Token MFA.
-        :return: SecretCode
+        Get the Secret code used for Software Token MFA.
+        :return: Secret code
         :rtype: string
         """
         response = self.client.associate_software_token(AccessToken=self.access_token)
         return response["SecretCode"]
 
-    def verify_software_token(self, code, device_name):
+    def verify_software_token(self, code, device_name=""):
         """
         Verify the value generated by TOTP to complete the registration of Software Token MFA.
         :param code: The value generated by TOTP
         :param device_name: Device name to register (optional)
         :return: verify success
         :rtype: bool
         """
@@ -945,47 +962,47 @@
     def set_user_mfa_preference(self, sms_mfa, software_token_mfa, preferred=None):
         """
         Register the preference of MFA.
         :param sms_mfa: Enable SMS MFA.
         :type sms_mfa: bool
         :param software_token_mfa: Enable Software Token MFA.
         :type software_token_mfa: bool
-        :param preferred: Which is the priority, SMS or Software Token? The expected value is "SMS" or "SOFTWARE_TOKEN". However, it is not needed only if both of the previous arguments are False.
+        :param preferred: "SMS" or "SOFTWARE_TOKEN", or None if both of the previous arguments are False.
         :type preferred: string
         :return:
         """
         sms_mfa_settings = {"Enabled": bool(sms_mfa), "PreferredMfa": False}
         software_token_mfa_settings = {
             "Enabled": bool(software_token_mfa),
             "PreferredMfa": False,
         }
         if not (bool(sms_mfa) or bool(software_token_mfa)):
             # Disable MFA
             pass
-        if preferred == "SMS":
+        elif preferred == "SMS":
             sms_mfa_settings["PreferredMfa"] = True
         elif preferred == "SOFTWARE_TOKEN":
             software_token_mfa_settings["PreferredMfa"] = True
         else:
             raise ValueError(
-                "preferred is not the correct value.\nThe expected value is SMS or SOFTWARE_TOKEN."
+                "preferred must have a value of 'SMS', 'SOFTWARE_TOKEN', or None."
             )
         self.client.set_user_mfa_preference(
             SMSMfaSettings=sms_mfa_settings,
             SoftwareTokenMfaSettings=software_token_mfa_settings,
             AccessToken=self.access_token,
         )
 
     def respond_to_software_token_mfa_challenge(self, code, mfa_tokens=None):
         """
-        Respons challenge to software token of MFA.
+        Response to software token MFA challenge.
         :param code: software token MFA code.
         :type code: string
-        :param code: mfa_token stored in MFAChallengeException. Not required if you have not regenerated the Cognito instance.
-        :type code: string
+        :param mfa_token: Token stored in MFAChallengeException. Optional if you have not regenerated the Cognito instance.
+        :type mfa_token: string
         :return:
         """
         if not mfa_tokens:
             mfa_tokens = self.mfa_tokens
         challenge_responses = {
             "USERNAME": self.username,
             "SOFTWARE_TOKEN_MFA_CODE": str(code),
@@ -997,28 +1014,28 @@
             ChallengeName="SOFTWARE_TOKEN_MFA",
             ChallengeResponses=challenge_responses,
         )
         self._set_tokens(tokens)
 
     def respond_to_sms_mfa_challenge(self, code, mfa_tokens=None):
         """
-        Respons challenge to SMS MFA.
+        Response to SMS MFA challenge.
         :param code: SMS MFA code.
         :type code: string
-        :param code: mfa_token stored in MFAChallengeException. Not required if you have not regenerated the Cognito instance.
-        :type code: string
+        :param mfa_tokens: Token stored in MFAChallengeException. Optional if you have not regenerated the Cognito instance.
+        :type mfa_tokens: string
         :return:
         """
         if not mfa_tokens:
             mfa_tokens = self.mfa_tokens
         challenge_responses = {
             "USERNAME": self.username,
             "SMS_MFA_CODE": code,
         }
         self._add_secret_hash(challenge_responses, "SECRET_HASH")
         tokens = self.client.respond_to_auth_challenge(
             ClientId=self.client_id,
-            Session=self.mfa_tokens["Session"],
+            Session=mfa_tokens["Session"],
             ChallengeName="SMS_MFA",
             ChallengeResponses=challenge_responses,
         )
         self._set_tokens(tokens)
```

### Comparing `pycognito-2022.8.0/pycognito/aws_srp.py` & `pycognito-2023.5.0/pycognito/aws_srp.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,16 +221,18 @@
         hmac_obj = hmac.new(bytearray(client_secret, "utf-8"), message, hashlib.sha256)
         return base64.standard_b64encode(hmac_obj.digest()).decode("utf-8")
 
     @staticmethod
     def get_cognito_formatted_timestamp(input_datetime):
         return f"{WEEKDAY_NAMES[input_datetime.weekday()]} {MONTH_NAMES[input_datetime.month - 1]} {input_datetime.day:d} {input_datetime.hour:02d}:{input_datetime.minute:02d}:{input_datetime.second:02d} UTC {input_datetime.year:d}"
 
-    def process_challenge(self, challenge_parameters):
-        internal_username = challenge_parameters["USERNAME"]
+    def process_challenge(self, challenge_parameters, request_parameters):
+        internal_username = challenge_parameters.get(
+            "USERNAME", request_parameters["USERNAME"]
+        )
         user_id_for_srp = challenge_parameters["USER_ID_FOR_SRP"]
         salt_hex = challenge_parameters["SALT"]
         srp_b_hex = challenge_parameters["SRP_B"]
         secret_block_b64 = challenge_parameters["SECRET_BLOCK"]
         timestamp = self.get_cognito_formatted_timestamp(datetime.datetime.utcnow())
         hkdf = self.get_password_authentication_key(
             user_id_for_srp, self.password, hex_to_long(srp_b_hex), salt_hex
@@ -266,15 +268,17 @@
         auth_params = self.get_auth_params()
         response = boto_client.initiate_auth(
             AuthFlow="USER_SRP_AUTH",
             AuthParameters=auth_params,
             ClientId=self.client_id,
         )
         if response["ChallengeName"] == self.PASSWORD_VERIFIER_CHALLENGE:
-            challenge_response = self.process_challenge(response["ChallengeParameters"])
+            challenge_response = self.process_challenge(
+                response["ChallengeParameters"], auth_params
+            )
             tokens = boto_client.respond_to_auth_challenge(
                 ClientId=self.client_id,
                 ChallengeName=self.PASSWORD_VERIFIER_CHALLENGE,
                 ChallengeResponses=challenge_response,
                 **dict(ClientMetadata=client_metadata) if client_metadata else {},
             )
 
@@ -302,15 +306,17 @@
         auth_params = self.get_auth_params()
         response = boto_client.initiate_auth(
             AuthFlow="USER_SRP_AUTH",
             AuthParameters=auth_params,
             ClientId=self.client_id,
         )
         if response["ChallengeName"] == self.PASSWORD_VERIFIER_CHALLENGE:
-            challenge_response = self.process_challenge(response["ChallengeParameters"])
+            challenge_response = self.process_challenge(
+                response["ChallengeParameters"], auth_params
+            )
             tokens = boto_client.respond_to_auth_challenge(
                 ClientId=self.client_id,
                 ChallengeName=self.PASSWORD_VERIFIER_CHALLENGE,
                 ChallengeResponses=challenge_response,
             )
 
             if tokens["ChallengeName"] == self.NEW_PASSWORD_REQUIRED_CHALLENGE:
```

### Comparing `pycognito-2022.8.0/pycognito/exceptions.py` & `pycognito-2023.5.0/pycognito/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycognito-2022.8.0/pycognito/utils.py` & `pycognito-2023.5.0/pycognito/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,36 +41,39 @@
         user_pool_id: str = None,
         user_pool_region: str = None,
         client_id: str = None,
         cognito: Cognito = None,
         http_header: str = "Authorization",
         http_header_prefix: str = "Bearer ",
         auth_token_type: TokenType = TokenType.ACCESS_TOKEN,
+        boto3_client_kwargs=None,
     ):
         """
 
         :param username: Cognito User. Required if `cognito` not set
         :param password: Password of Cognito User. Required if `cognito` not set
         :param user_pool_id: Cognito User Pool. Required if `cognito` not set
         :param user_pool_region: Region of the Cognito User Pool. Required if `cognito` not set
         :param client_id: Cognito Client ID / Application. Required if :py:attr:`cognito` not set
         :param cognito: Provide a preconfigured `pycognito.Cognito` instead of `username`, `password` etc
         :param http_header: The HTTP Header to populate. Defaults to "Authorization" (Basic Authentication)
         :param http_header_prefix: Prefix a value before the token. Defaults to "Bearer ". (Note the space)
         :param auth_token_type: Whether to populate the header with ID or ACCESS_TOKEN. Defaults to "ACCESS_TOKEN"
+        :param boto3_client_kwargs: Keyword args to pass to Boto3 for client creation
         """
 
         if cognito:
             self.cognito_client = cognito
         else:
             self.cognito_client = Cognito(
                 user_pool_id=user_pool_id,
                 client_id=client_id,
                 user_pool_region=user_pool_region,
                 username=username,
+                boto3_client_kwargs=boto3_client_kwargs,
             )
 
         self.username = username
         self.__password = password
         self.http_header = http_header
         self.http_header_prefix = http_header_prefix
         self.token_type = auth_token_type
```

### Comparing `pycognito-2022.8.0/pycognito.egg-info/PKG-INFO` & `pycognito-2023.5.0/pycognito.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pycognito
-Version: 2022.8.0
+Version: 2023.5.0
 Summary: Python class to integrate Boto3's Cognito client so it is easy to login users. With SRP support.
 Home-page: https://github.com/pvizeli/pycognito
+Download-URL: https://github.com/pvizeli/pycognito/tarball/2023.5.0
 Author: Pascal Vizeli
 Author-email: pvizeli@syshack.ch
 License: Apache License 2.0
-Download-URL: https://github.com/pvizeli/pycognito/tarball/2022.08.0
 Keywords: aws,cognito,api,gateway,serverless
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Environment :: Web Environment
@@ -713,9 +712,7 @@
   user_pool_id='eu-west-1_1234567',
   client_id='4dn6jbcbhqcofxyczo3ms9z4cc',
   user_pool_region='eu-west-1',
 )
 
 response = requests.get('http://test.com', auth=auth)
 ```
-
-
```

### Comparing `pycognito-2022.8.0/setup.py` & `pycognito-2023.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from setuptools import setup, find_packages
 
-VERSION = "2022.08.0"
+VERSION = "2023.5.0"
 
 setup(
     name="pycognito",
     version=VERSION,
     description="Python class to integrate Boto3's Cognito client so it is easy to login users. With SRP support.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
```

