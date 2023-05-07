# Comparing `tmp/certifi-2022.9.24.tar.gz` & `tmp/certifi-2023.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certifi-2022.9.24.tar", last modified: Sat Sep 24 14:26:49 2022, max compression
+gzip compressed data, was "certifi-2023.5.7.tar", last modified: Sun May  7 07:30:51 2023, max compression
```

## Comparing `certifi-2022.9.24.tar` & `certifi-2023.5.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cory       (502) staff       (20)        0 2022-09-24 14:26:49.218689 certifi-2022.9.24/
--rw-r--r--   0 cory       (502) staff       (20)     1052 2022-07-20 11:27:58.000000 certifi-2022.9.24/LICENSE
--rw-r--r--   0 cory       (502) staff       (20)      119 2022-05-23 19:19:32.000000 certifi-2022.9.24/MANIFEST.in
--rw-r--r--   0 cory       (502) staff       (20)     2911 2022-09-24 14:26:49.218561 certifi-2022.9.24/PKG-INFO
--rw-r--r--   0 cory       (502) staff       (20)     1877 2022-05-18 19:10:22.000000 certifi-2022.9.24/README.rst
-drwxr-xr-x   0 cory       (502) staff       (20)        0 2022-09-24 14:26:49.217888 certifi-2022.9.24/certifi/
--rw-r--r--   0 cory       (502) staff       (20)       94 2022-09-24 14:26:39.000000 certifi-2022.9.24/certifi/__init__.py
--rw-r--r--   0 cory       (502) staff       (20)      243 2020-04-05 15:50:05.000000 certifi-2022.9.24/certifi/__main__.py
--rw-r--r--   0 cory       (502) staff       (20)   286370 2022-09-24 14:25:51.000000 certifi-2022.9.24/certifi/cacert.pem
--rw-r--r--   0 cory       (502) staff       (20)     4219 2022-09-13 20:15:32.000000 certifi-2022.9.24/certifi/core.py
--rw-r--r--   0 cory       (502) staff       (20)        0 2022-05-18 19:10:22.000000 certifi-2022.9.24/certifi/py.typed
-drwxr-xr-x   0 cory       (502) staff       (20)        0 2022-09-24 14:26:49.218402 certifi-2022.9.24/certifi.egg-info/
--rw-r--r--   0 cory       (502) staff       (20)     2911 2022-09-24 14:26:49.000000 certifi-2022.9.24/certifi.egg-info/PKG-INFO
--rw-r--r--   0 cory       (502) staff       (20)      285 2022-09-24 14:26:49.000000 certifi-2022.9.24/certifi.egg-info/SOURCES.txt
--rw-r--r--   0 cory       (502) staff       (20)        1 2022-09-24 14:26:49.000000 certifi-2022.9.24/certifi.egg-info/dependency_links.txt
--rw-r--r--   0 cory       (502) staff       (20)        1 2022-09-24 14:26:49.000000 certifi-2022.9.24/certifi.egg-info/not-zip-safe
--rw-r--r--   0 cory       (502) staff       (20)        8 2022-09-24 14:26:49.000000 certifi-2022.9.24/certifi.egg-info/top_level.txt
--rw-r--r--   0 cory       (502) staff       (20)       38 2022-09-24 14:26:49.218735 certifi-2022.9.24/setup.cfg
--rwxr-xr-x   0 cory       (502) staff       (20)     2302 2022-07-20 11:27:58.000000 certifi-2022.9.24/setup.py
+drwxr-xr-x   0 cory       (502) staff       (20)        0 2023-05-07 07:30:51.755347 certifi-2023.5.7/
+-rw-r--r--   0 cory       (502) staff       (20)     1052 2022-07-20 11:27:58.000000 certifi-2023.5.7/LICENSE
+-rw-r--r--   0 cory       (502) staff       (20)      119 2022-05-23 19:19:32.000000 certifi-2023.5.7/MANIFEST.in
+-rw-r--r--   0 cory       (502) staff       (20)     2190 2023-05-07 07:30:51.755232 certifi-2023.5.7/PKG-INFO
+-rw-r--r--   0 cory       (502) staff       (20)     1157 2023-01-14 18:45:41.000000 certifi-2023.5.7/README.rst
+drwxr-xr-x   0 cory       (502) staff       (20)        0 2023-05-07 07:30:51.754516 certifi-2023.5.7/certifi/
+-rw-r--r--   0 cory       (502) staff       (20)       94 2023-05-07 07:30:05.000000 certifi-2023.5.7/certifi/__init__.py
+-rw-r--r--   0 cory       (502) staff       (20)      243 2020-04-05 15:50:05.000000 certifi-2023.5.7/certifi/__main__.py
+-rw-r--r--   0 cory       (502) staff       (20)   278952 2023-05-07 07:25:48.000000 certifi-2023.5.7/certifi/cacert.pem
+-rw-r--r--   0 cory       (502) staff       (20)     4219 2022-09-13 20:15:32.000000 certifi-2023.5.7/certifi/core.py
+-rw-r--r--   0 cory       (502) staff       (20)        0 2022-05-18 19:10:22.000000 certifi-2023.5.7/certifi/py.typed
+drwxr-xr-x   0 cory       (502) staff       (20)        0 2023-05-07 07:30:51.755055 certifi-2023.5.7/certifi.egg-info/
+-rw-r--r--   0 cory       (502) staff       (20)     2190 2023-05-07 07:30:51.000000 certifi-2023.5.7/certifi.egg-info/PKG-INFO
+-rw-r--r--   0 cory       (502) staff       (20)      285 2023-05-07 07:30:51.000000 certifi-2023.5.7/certifi.egg-info/SOURCES.txt
+-rw-r--r--   0 cory       (502) staff       (20)        1 2023-05-07 07:30:51.000000 certifi-2023.5.7/certifi.egg-info/dependency_links.txt
+-rw-r--r--   0 cory       (502) staff       (20)        1 2023-05-07 07:30:51.000000 certifi-2023.5.7/certifi.egg-info/not-zip-safe
+-rw-r--r--   0 cory       (502) staff       (20)        8 2023-05-07 07:30:51.000000 certifi-2023.5.7/certifi.egg-info/top_level.txt
+-rw-r--r--   0 cory       (502) staff       (20)       38 2023-05-07 07:30:51.755389 certifi-2023.5.7/setup.cfg
+-rwxr-xr-x   0 cory       (502) staff       (20)     2302 2022-07-20 11:27:58.000000 certifi-2023.5.7/setup.py
```

### Comparing `certifi-2022.9.24/LICENSE` & `certifi-2023.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `certifi-2022.9.24/PKG-INFO` & `certifi-2023.5.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certifi
-Version: 2022.9.24
+Version: 2023.5.7
 Summary: Python package for providing Mozilla's CA Bundle.
 Home-page: https://github.com/certifi/python-certifi
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.com
 License: MPL-2.0
 Project-URL: Source, https://github.com/certifi/python-certifi
 Platform: UNKNOWN
@@ -52,28 +52,14 @@
 Or from the command line::
 
     $ python -m certifi
     /usr/local/lib/python3.7/site-packages/certifi/cacert.pem
 
 Enjoy!
 
-1024-bit Root Certificates
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Browsers and certificate authorities have concluded that 1024-bit keys are
-unacceptably weak for certificates, particularly root certificates. For this
-reason, Mozilla has removed any weak (i.e. 1024-bit key) certificate from its
-bundle, replacing it with an equivalent strong (i.e. 2048-bit or greater key)
-certificate from the same CA. Because Mozilla removed these certificates from
-its bundle, ``certifi`` removed them as well.
-
-In previous versions, ``certifi`` provided the ``certifi.old_where()`` function
-to intentionally re-add the 1024-bit roots back into your bundle. This was not
-recommended in production and therefore was removed at the end of 2018.
-
 .. _`Requests`: https://requests.readthedocs.io/en/master/
 
 Addition/Removal of Certificates
 --------------------------------
 
 Certifi does not support any addition/removal or other modification of the
 CA trust store content. This project is intended to provide a reliable and
```

### Comparing `certifi-2022.9.24/certifi/cacert.pem` & `certifi-2023.5.7/certifi/cacert.pem`

 * *Files 2% similar despite different names*

```diff
@@ -632,45 +632,14 @@
 IC9Bi5HcSEW88cbeunZrM8gALTFGTO3nnc+IlP8zwFboJIYmuNg4ON8qa90SzMc/
 RxdMosIGlgnW2/4/PEZB31jiVg88O8EckzXZOFKs7sjsLjBOlDW0JB9LeGna8gI4
 zJVSk/BwJVmcIGfE7vmLV2H0knZ9P4SNVbfo5azV8fUZVqZa+5Acr5Pr5RzUZ5dd
 BA6+C4OmF4O5MBKgxTMVBbkN+8cFduPYSo38NBejxiEovjBFMR7HeL5YYTisO+IB
 ZQ==
 -----END CERTIFICATE-----
 
-# Issuer: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Subject: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Label: "Network Solutions Certificate Authority"
-# Serial: 116697915152937497490437556386812487904
-# MD5 Fingerprint: d3:f3:a6:16:c0:fa:6b:1d:59:b1:2d:96:4d:0e:11:2e
-# SHA1 Fingerprint: 74:f8:a3:c3:ef:e7:b3:90:06:4b:83:90:3c:21:64:60:20:e5:df:ce
-# SHA256 Fingerprint: 15:f0:ba:00:a3:ac:7a:f3:ac:88:4c:07:2b:10:11:a0:77:bd:77:c0:97:f4:01:64:b2:f8:59:8a:bd:83:86:0c
------BEGIN CERTIFICATE-----
-MIID5jCCAs6gAwIBAgIQV8szb8JcFuZHFhfjkDFo4DANBgkqhkiG9w0BAQUFADBi
-MQswCQYDVQQGEwJVUzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMu
-MTAwLgYDVQQDEydOZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3Jp
-dHkwHhcNMDYxMjAxMDAwMDAwWhcNMjkxMjMxMjM1OTU5WjBiMQswCQYDVQQGEwJV
-UzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMuMTAwLgYDVQQDEydO
-ZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkwggEiMA0GCSqG
-SIb3DQEBAQUAA4IBDwAwggEKAoIBAQDkvH6SMG3G2I4rC7xGzuAnlt7e+foS0zwz
-c7MEL7xxjOWftiJgPl9dzgn/ggwbmlFQGiaJ3dVhXRncEg8tCqJDXRfQNJIg6nPP
-OCwGJgl6cvf6UDL4wpPTaaIjzkGxzOTVHzbRijr4jGPiFFlp7Q3Tf2vouAPlT2rl
-mGNpSAW+Lv8ztumXWWn4Zxmuk2GWRBXTcrA/vGp97Eh/jcOrqnErU2lBUzS1sLnF
-BgrEsEX1QV1uiUV7PTsmjHTC5dLRfbIR1PtYMiKagMnc/Qzpf14Dl847ABSHJ3A4
-qY5usyd2mFHgBeMhqxrVhSI8KbWaFsWAqPS7azCPL0YCorEMIuDTAgMBAAGjgZcw
-gZQwHQYDVR0OBBYEFCEwyfsA106Y2oeqKtCnLrFAMadMMA4GA1UdDwEB/wQEAwIB
-BjAPBgNVHRMBAf8EBTADAQH/MFIGA1UdHwRLMEkwR6BFoEOGQWh0dHA6Ly9jcmwu
-bmV0c29sc3NsLmNvbS9OZXR3b3JrU29sdXRpb25zQ2VydGlmaWNhdGVBdXRob3Jp
-dHkuY3JsMA0GCSqGSIb3DQEBBQUAA4IBAQC7rkvnt1frf6ott3NHhWrB5KUd5Oc8
-6fRZZXe1eltajSU24HqXLjjAV2CDmAaDn7l2em5Q4LqILPxFzBiwmZVRDuwduIj/
-h1AcgsLj4DKAv6ALR8jDMe+ZZzKATxcheQxpXN5eNK4CtSbqUN9/GGUsyfJj4akH
-/nxxH2szJGoeBfcFaMBqEssuXmHLrijTfsK0ZpEmXzwuJF/LWA/rKOyvEZbz3Htv
-wKeI8lN3s2Berq4o2jUsbzRF0ybh3uxbTydrFny9RAQYgrOJeRcQcT16ohZO9QHN
-pGxlaKFJdlxDydi8NmdspZS11My5vWo1ViHe2MPr+8ukYEywVaCge1ey
------END CERTIFICATE-----
-
 # Issuer: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Subject: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Label: "COMODO ECC Certification Authority"
 # Serial: 41578283867086692638256921589707938090
 # MD5 Fingerprint: 7c:62:ff:74:9d:31:53:5e:68:4a:d5:78:aa:1e:bf:23
 # SHA1 Fingerprint: 9f:74:4e:9f:2b:4d:ba:ec:0f:31:2c:50:b6:56:3b:8e:2d:93:c3:11
 # SHA256 Fingerprint: 17:93:92:7a:06:14:54:97:89:ad:ce:2f:8f:34:f7:f0:b6:6d:0f:3a:e3:a3:b8:4d:21:ec:15:db:ba:4f:ad:c7
@@ -2200,54 +2169,14 @@
 hOvRnkmSh5SHDDqFSmafnVmTTZdhBoZKo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYD
 VR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUPeYpSJvqB8ohREom3m7e0oPQn1kwCgYI
 KoZIzj0EAwMDaAAwZQIxAOVpEslu28YxuglB4Zf4+/2a4n0Sye18ZNPLBSWLVtmg
 515dTguDnFt2KaAJJiFqYgIwcdK1j1zqO+F4CYWodZI7yFz9SO8NdCKoCOJuxUnO
 xwy8p2Fp8fc74SrL+SvzZpA3
 -----END CERTIFICATE-----
 
-# Issuer: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Subject: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Label: "Staat der Nederlanden EV Root CA"
-# Serial: 10000013
-# MD5 Fingerprint: fc:06:af:7b:e8:1a:f1:9a:b4:e8:d2:70:1f:c0:f5:ba
-# SHA1 Fingerprint: 76:e2:7e:c1:4f:db:82:c1:c0:a6:75:b5:05:be:3d:29:b4:ed:db:bb
-# SHA256 Fingerprint: 4d:24:91:41:4c:fe:95:67:46:ec:4c:ef:a6:cf:6f:72:e2:8a:13:29:43:2f:9d:8a:90:7a:c4:cb:5d:ad:c1:5a
------BEGIN CERTIFICATE-----
-MIIFcDCCA1igAwIBAgIEAJiWjTANBgkqhkiG9w0BAQsFADBYMQswCQYDVQQGEwJO
-TDEeMBwGA1UECgwVU3RhYXQgZGVyIE5lZGVybGFuZGVuMSkwJwYDVQQDDCBTdGFh
-dCBkZXIgTmVkZXJsYW5kZW4gRVYgUm9vdCBDQTAeFw0xMDEyMDgxMTE5MjlaFw0y
-MjEyMDgxMTEwMjhaMFgxCzAJBgNVBAYTAk5MMR4wHAYDVQQKDBVTdGFhdCBkZXIg
-TmVkZXJsYW5kZW4xKTAnBgNVBAMMIFN0YWF0IGRlciBOZWRlcmxhbmRlbiBFViBS
-b290IENBMIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEA48d+ifkkSzrS
-M4M1LGns3Amk41GoJSt5uAg94JG6hIXGhaTK5skuU6TJJB79VWZxXSzFYGgEt9nC
-UiY4iKTWO0Cmws0/zZiTs1QUWJZV1VD+hq2kY39ch/aO5ieSZxeSAgMs3NZmdO3d
-Z//BYY1jTw+bbRcwJu+r0h8QoPnFfxZpgQNH7R5ojXKhTbImxrpsX23Wr9GxE46p
-rfNeaXUmGD5BKyF/7otdBwadQ8QpCiv8Kj6GyzyDOvnJDdrFmeK8eEEzduG/L13l
-pJhQDBXd4Pqcfzho0LKmeqfRMb1+ilgnQ7O6M5HTp5gVXJrm0w912fxBmJc+qiXb
-j5IusHsMX/FjqTf5m3VpTCgmJdrV8hJwRVXj33NeN/UhbJCONVrJ0yPr08C+eKxC
-KFhmpUZtcALXEPlLVPxdhkqHz3/KRawRWrUgUY0viEeXOcDPusBCAUCZSCELa6fS
-/ZbV0b5GnUngC6agIk440ME8MLxwjyx1zNDFjFE7PZQIZCZhfbnDZY8UnCHQqv0X
-cgOPvZuM5l5Tnrmd74K74bzickFbIZTTRTeU0d8JOV3nI6qaHcptqAqGhYqCvkIH
-1vI4gnPah1vlPNOePqc7nvQDs/nxfRN0Av+7oeX6AHkcpmZBiFxgV6YuCcS6/ZrP
-px9Aw7vMWgpVSzs4dlG4Y4uElBbmVvMCAwEAAaNCMEAwDwYDVR0TAQH/BAUwAwEB
-/zAOBgNVHQ8BAf8EBAMCAQYwHQYDVR0OBBYEFP6rAJCYniT8qcwaivsnuL8wbqg7
-MA0GCSqGSIb3DQEBCwUAA4ICAQDPdyxuVr5Os7aEAJSrR8kN0nbHhp8dB9O2tLsI
-eK9p0gtJ3jPFrK3CiAJ9Brc1AsFgyb/E6JTe1NOpEyVa/m6irn0F3H3zbPB+po3u
-2dfOWBfoqSmuc0iH55vKbimhZF8ZE/euBhD/UcabTVUlT5OZEAFTdfETzsemQUHS
-v4ilf0X8rLiltTMMgsT7B/Zq5SWEXwbKwYY5EdtYzXc7LMJMD16a4/CrPmEbUCTC
-wPTxGfARKbalGAKb12NMcIxHowNDXLldRqANb/9Zjr7dn3LDWyvfjFvO5QxGbJKy
-CqNMVEIYFRIYvdr8unRu/8G2oGTYqV9Vrp9canaW2HNnh/tNf1zuacpzEPuKqf2e
-vTY4SUmH9A4U8OmHuD+nT3pajnnUk+S7aFKErGzp85hwVXIy+TSrK0m1zSBi5Dp6
-Z2Orltxtrpfs/J92VoguZs9btsmksNcFuuEnL5O7Jiqik7Ab846+HUCjuTaPPoIa
-Gl6I6lD4WeKDRikL40Rc4ZW2aZCaFG+XroHPaO+Zmr615+F/+PoTRxZMzG0IQOeL
-eG9QgkRQP2YGiqtDhFZKDyAthg710tvSeopLzaXoTvFeJiUBWSOgftL2fiFX1ye8
-FVdMpEbB4IMeDExNH08GGeL5qPQ6gqGyeUN51q1veieQA6TqJIc/2b3Z6fJfUEkc
-7uzXLg==
------END CERTIFICATE-----
-
 # Issuer: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Subject: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Label: "IdenTrust Commercial Root CA 1"
 # Serial: 13298821034946342390520003877796839426
 # MD5 Fingerprint: b3:3e:77:73:75:ee:a0:d3:e3:7e:49:63:49:59:bb:c7
 # SHA1 Fingerprint: df:71:7e:aa:4a:d9:4e:c9:55:84:99:60:2d:48:de:5f:bc:f0:3a:25
 # SHA256 Fingerprint: 5d:56:49:9b:e4:d2:e0:8b:cf:ca:d0:8a:3e:38:72:3d:50:50:3b:de:70:69:48:e4:2f:55:60:30:19:e5:28:ae
@@ -2847,124 +2776,14 @@
 2c9Si1vIY9RCPqAzekYu9wogRlR+ak8x8YF+QnQ4ZXMn7sZ8uI7XpTrXmKGcjBBV
 09tL7ECQ8s1uV9JiDnxXk7Gnbc2dg7sq5+W2O3FYrf3RRbxake5TFW/TRQl1brqQ
 XR4EzzffHqhmsYzmIGrv/EhOdJhCrylvLmrH+33RZjEizIYAfmaDDEL0vTSSwxrq
 T8p+ck0LcIymSLumoRT2+1hEmRSuqguTaaApJUqlyyvdimYHFngVV3Eb7PVHhPOe
 MTd61X8kreS8/f3MboPoDKi3QWwH3b08hpcv0g==
 -----END CERTIFICATE-----
 
-# Issuer: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-1"
-# Serial: 15752444095811006489
-# MD5 Fingerprint: 6e:85:f1:dc:1a:00:d3:22:d5:b2:b2:ac:6b:37:05:45
-# SHA1 Fingerprint: ff:bd:cd:e7:82:c8:43:5e:3c:6f:26:86:5c:ca:a8:3a:45:5b:c3:0a
-# SHA256 Fingerprint: d4:0e:9c:86:cd:8f:e4:68:c1:77:69:59:f4:9e:a7:74:fa:54:86:84:b6:c4:06:f3:90:92:61:f4:dc:e2:57:5c
------BEGIN CERTIFICATE-----
-MIIEMDCCAxigAwIBAgIJANqb7HHzA7AZMA0GCSqGSIb3DQEBCwUAMIGkMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRydXN0Q29y
-IFJvb3RDZXJ0IENBLTEwHhcNMTYwMjA0MTIzMjE2WhcNMjkxMjMxMTcyMzE2WjCB
-pDELMAkGA1UEBhMCUEExDzANBgNVBAgMBlBhbmFtYTEUMBIGA1UEBwwLUGFuYW1h
-IENpdHkxJDAiBgNVBAoMG1RydXN0Q29yIFN5c3RlbXMgUy4gZGUgUi5MLjEnMCUG
-A1UECwweVHJ1c3RDb3IgQ2VydGlmaWNhdGUgQXV0aG9yaXR5MR8wHQYDVQQDDBZU
-cnVzdENvciBSb290Q2VydCBDQS0xMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
-CgKCAQEAv463leLCJhJrMxnHQFgKq1mqjQCj/IDHUHuO1CAmujIS2CNUSSUQIpid
-RtLByZ5OGy4sDjjzGiVoHKZaBeYei0i/mJZ0PmnK6bV4pQa81QBeCQryJ3pS/C3V
-seq0iWEk8xoT26nPUu0MJLq5nux+AHT6k61sKZKuUbS701e/s/OojZz0JEsq1pme
-9J7+wH5COucLlVPat2gOkEz7cD+PSiyU8ybdY2mplNgQTsVHCJCZGxdNuWxu72CV
-EY4hgLW9oHPY0LJ3xEXqWib7ZnZ2+AYfYW0PVcWDtxBWcgYHpfOxGgMFZA6dWorW
-hnAbJN7+KIor0Gqw/Hqi3LJ5DotlDwIDAQABo2MwYTAdBgNVHQ4EFgQU7mtJPHo/
-DeOxCbeKyKsZn3MzUOcwHwYDVR0jBBgwFoAU7mtJPHo/DeOxCbeKyKsZn3MzUOcw
-DwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYwDQYJKoZIhvcNAQELBQAD
-ggEBACUY1JGPE+6PHh0RU9otRCkZoB5rMZ5NDp6tPVxBb5UrJKF5mDo4Nvu7Zp5I
-/5CQ7z3UuJu0h3U/IJvOcs+hVcFNZKIZBqEHMwwLKeXx6quj7LUKdJDHfXLy11yf
-ke+Ri7fc7Waiz45mO7yfOgLgJ90WmMCV1Aqk5IGadZQ1nJBfiDcGrVmVCrDRZ9MZ
-yonnMlo2HD6CqFqTvsbQZJG2z9m2GM/bftJlo6bEjhcxwft+dtvTheNYsnd6djts
-L1Ac59v2Z3kf9YKVmgenFK+P3CghZwnS1k1aHBkcjndcw5QkPTJrS37UeJSDvjdN
-zl/HHk484IkzlQsPpTLWPFp5LBk=
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-2"
-# Serial: 2711694510199101698
-# MD5 Fingerprint: a2:e1:f8:18:0b:ba:45:d5:c7:41:2a:bb:37:52:45:64
-# SHA1 Fingerprint: b8:be:6d:cb:56:f1:55:b9:63:d4:12:ca:4e:06:34:c7:94:b2:1c:c0
-# SHA256 Fingerprint: 07:53:e9:40:37:8c:1b:d5:e3:83:6e:39:5d:ae:a5:cb:83:9e:50:46:f1:bd:0e:ae:19:51:cf:10:fe:c7:c9:65
------BEGIN CERTIFICATE-----
-MIIGLzCCBBegAwIBAgIIJaHfyjPLWQIwDQYJKoZIhvcNAQELBQAwgaQxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEfMB0GA1UEAwwWVHJ1c3RDb3Ig
-Um9vdENlcnQgQ0EtMjAeFw0xNjAyMDQxMjMyMjNaFw0zNDEyMzExNzI2MzlaMIGk
-MQswCQYDVQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEg
-Q2l0eTEkMCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYD
-VQQLDB5UcnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRy
-dXN0Q29yIFJvb3RDZXJ0IENBLTIwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIK
-AoICAQCnIG7CKqJiJJWQdsg4foDSq8GbZQWU9MEKENUCrO2fk8eHyLAnK0IMPQo+
-QVqedd2NyuCb7GgypGmSaIwLgQ5WoD4a3SwlFIIvl9NkRvRUqdw6VC0xK5mC8tkq
-1+9xALgxpL56JAfDQiDyitSSBBtlVkxs1Pu2YVpHI7TYabS3OtB0PAx1oYxOdqHp
-2yqlO/rOsP9+aij9JxzIsekp8VduZLTQwRVtDr4uDkbIXvRR/u8OYzo7cbrPb1nK
-DOObXUm4TOJXsZiKQlecdu/vvdFoqNL0Cbt3Nb4lggjEFixEIFapRBF37120Hape
-az6LMvYHL1cEksr1/p3C6eizjkxLAjHZ5DxIgif3GIJ2SDpxsROhOdUuxTTCHWKF
-3wP+TfSvPd9cW436cOGlfifHhi5qjxLGhF5DUVCcGZt45vz27Ud+ez1m7xMTiF88
-oWP7+ayHNZ/zgp6kPwqcMWmLmaSISo5uZk3vFsQPeSghYA2FFn3XVDjxklb9tTNM
-g9zXEJ9L/cb4Qr26fHMC4P99zVvh1Kxhe1fVSntb1IVYJ12/+CtgrKAmrhQhJ8Z3
-mjOAPF5GP/fDsaOGM8boXg25NSyqRsGFAnWAoOsk+xWq5Gd/bnc/9ASKL3x74xdh
-8N0JqSDIvgmk0H5Ew7IwSjiqqewYmgeCK9u4nBit2uBGF6zPXQIDAQABo2MwYTAd
-BgNVHQ4EFgQU2f4hQG6UnrybPZx9mCAZ5YwwYrIwHwYDVR0jBBgwFoAU2f4hQG6U
-nrybPZx9mCAZ5YwwYrIwDwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYw
-DQYJKoZIhvcNAQELBQADggIBAJ5Fngw7tu/hOsh80QA9z+LqBrWyOrsGS2h60COX
-dKcs8AjYeVrXWoSK2BKaG9l9XE1wxaX5q+WjiYndAfrs3fnpkpfbsEZC89NiqpX+
-MWcUaViQCqoL7jcjx1BRtPV+nuN79+TMQjItSQzL/0kMmx40/W5ulop5A7Zv2wnL
-/V9lFDfhOPXzYRZY5LVtDQsEGz9QLX+zx3oaFoBg+Iof6Rsqxvm6ARppv9JYx1RX
-CI/hOWB3S6xZhBqI8d3LT3jX5+EzLfzuQfogsL7L9ziUwOHQhQ+77Sxzq+3+knYa
-ZH9bDTMJBzN7Bj8RpFxwPIXAz+OQqIN3+tvmxYxoZxBnpVIt8MSZj3+/0WvitUfW
-2dCFmU2Umw9Lje4AWkcdEQOsQRivh7dvDDqPys/cA8GiCcjl/YBeyGBCARsaU1q7
-N6a3vLqE6R5sGtRk2tRD/pOLS/IseRYQ1JMLiI+h2IYURpFHmygk71dSTlxCnKr3
-Sewn6EAes6aJInKc9Q0ztFijMDvd1GpUk74aTfOTlPf8hAs/hCBcNANExdqtvArB
-As8e5ZTZ845b2EzwnexhF7sUMlQMAimTHpKG9n/v55IFDlndmQguLvqcAFLTxWYp
-5KeXRKQOKIETNcX2b2TmQcTVL8w0RSXPQQCWPUouwpaYT05KnJe32x+SMsj/D1Fu
-1uwJ
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor ECA-1"
-# Serial: 9548242946988625984
-# MD5 Fingerprint: 27:92:23:1d:0a:f5:40:7c:e9:e6:6b:9d:d8:f5:e7:6c
-# SHA1 Fingerprint: 58:d1:df:95:95:67:6b:63:c0:f0:5b:1c:17:4d:8b:84:0b:c8:78:bd
-# SHA256 Fingerprint: 5a:88:5d:b1:9c:01:d9:12:c5:75:93:88:93:8c:af:bb:df:03:1a:b2:d4:8e:91:ee:15:58:9b:42:97:1d:03:9c
------BEGIN CERTIFICATE-----
-MIIEIDCCAwigAwIBAgIJAISCLF8cYtBAMA0GCSqGSIb3DQEBCwUAMIGcMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxFzAVBgNVBAMMDlRydXN0Q29y
-IEVDQS0xMB4XDTE2MDIwNDEyMzIzM1oXDTI5MTIzMTE3MjgwN1owgZwxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEXMBUGA1UEAwwOVHJ1c3RDb3Ig
-RUNBLTEwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDPj+ARtZ+odnbb
-3w9U73NjKYKtR8aja+3+XzP4Q1HpGjORMRegdMTUpwHmspI+ap3tDvl0mEDTPwOA
-BoJA6LHip1GnHYMma6ve+heRK9jGrB6xnhkB1Zem6g23xFUfJ3zSCNV2HykVh0A5
-3ThFEXXQmqc04L/NyFIduUd+Dbi7xgz2c1cWWn5DkR9VOsZtRASqnKmcp0yJF4Ou
-owReUoCLHhIlERnXDH19MURB6tuvsBzvgdAsxZohmz3tQjtQJvLsznFhBmIhVE5/
-wZ0+fyCMgMsq2JdiyIMzkX2woloPV+g7zPIlstR8L+xNxqE6FXrntl019fZISjZF
-ZtS6mFjBAgMBAAGjYzBhMB0GA1UdDgQWBBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAf
-BgNVHSMEGDAWgBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAPBgNVHRMBAf8EBTADAQH/
-MA4GA1UdDwEB/wQEAwIBhjANBgkqhkiG9w0BAQsFAAOCAQEABT41XBVwm8nHc2Fv
-civUwo/yQ10CzsSUuZQRg2dd4mdsdXa/uwyqNsatR5Nj3B5+1t4u/ukZMjgDfxT2
-AHMsWbEhBuH7rBiVDKP/mZb3Kyeb1STMHd3BOuCYRLDE5D53sXOpZCz2HAF8P11F
-hcCF5yWPldwX8zyfGm6wyuMdKulMY/okYWLW2n62HGz1Ah3UKt1VkOsqEUc8Ll50
-soIipX1TH0XsJ5F95yIW6MBoNtjG8U+ARDL54dHRHareqKucBK+tIA5kmE2la8BI
-WJZpTdwHjFGTot+fDz2LYLSCjaoITmJF4PkL0uDgPFveXHEnJcLmA4GLEFPjx1Wi
-tJ/X5g==
------END CERTIFICATE-----
-
 # Issuer: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Subject: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Label: "SSL.com Root Certification Authority RSA"
 # Serial: 8875640296558310041
 # MD5 Fingerprint: 86:69:12:c0:70:f1:ec:ac:ac:c2:d5:bc:a5:5b:a1:29
 # SHA1 Fingerprint: b7:ab:33:08:d1:ea:44:77:ba:14:80:12:5a:6f:bd:a9:36:49:0c:bb
 # SHA256 Fingerprint: 85:66:6a:56:2e:e0:be:5c:e9:25:c1:d8:89:0a:6f:76:a8:7e:c1:6d:4d:7d:5f:29:ea:74:19:cf:20:12:3b:69
@@ -4702,7 +4521,69 @@
 AASkpW9gAwPDvTH00xecK4R1rOX9PVdu12O/5gSJko6BnOPpR27KkBLIE+Cnnfdl
 dB9sELLo5OnvbYUymUSxXv3MdhDYW72ixvnWQuRXdtyQwjWpS4g8EkdtXP9JTxpK
 ULGjQjBAMB0GA1UdDgQWBBSGHOf+LaVKiwj+KBH6vqNm+GBZLzAOBgNVHQ8BAf8E
 BAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAKBggqhkjOPQQDAwNoADBlAjAVXUI9/Lbu
 9zuxNuie9sRGKEkz0FhDKmMpzE2xtHqiuQ04pV1IKv3LsnNdo4gIxwwCMQDAqy0O
 be0YottT6SXbVQjgUMzfRGEWgqtJsLKB7HOHeLRMsmIbEvoWTSVLY70eN9k=
 -----END CERTIFICATE-----
+
+# Issuer: CN=BJCA Global Root CA1 O=BEIJING CERTIFICATE AUTHORITY
+# Subject: CN=BJCA Global Root CA1 O=BEIJING CERTIFICATE AUTHORITY
+# Label: "BJCA Global Root CA1"
+# Serial: 113562791157148395269083148143378328608
+# MD5 Fingerprint: 42:32:99:76:43:33:36:24:35:07:82:9b:28:f9:d0:90
+# SHA1 Fingerprint: d5:ec:8d:7b:4c:ba:79:f4:e7:e8:cb:9d:6b:ae:77:83:10:03:21:6a
+# SHA256 Fingerprint: f3:89:6f:88:fe:7c:0a:88:27:66:a7:fa:6a:d2:74:9f:b5:7a:7f:3e:98:fb:76:9c:1f:a7:b0:9c:2c:44:d5:ae
+-----BEGIN CERTIFICATE-----
+MIIFdDCCA1ygAwIBAgIQVW9l47TZkGobCdFsPsBsIDANBgkqhkiG9w0BAQsFADBU
+MQswCQYDVQQGEwJDTjEmMCQGA1UECgwdQkVJSklORyBDRVJUSUZJQ0FURSBBVVRI
+T1JJVFkxHTAbBgNVBAMMFEJKQ0EgR2xvYmFsIFJvb3QgQ0ExMB4XDTE5MTIxOTAz
+MTYxN1oXDTQ0MTIxMjAzMTYxN1owVDELMAkGA1UEBhMCQ04xJjAkBgNVBAoMHUJF
+SUpJTkcgQ0VSVElGSUNBVEUgQVVUSE9SSVRZMR0wGwYDVQQDDBRCSkNBIEdsb2Jh
+bCBSb290IENBMTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBAPFmCL3Z
+xRVhy4QEQaVpN3cdwbB7+sN3SJATcmTRuHyQNZ0YeYjjlwE8R4HyDqKYDZ4/N+AZ
+spDyRhySsTphzvq3Rp4Dhtczbu33RYx2N95ulpH3134rhxfVizXuhJFyV9xgw8O5
+58dnJCNPYwpj9mZ9S1WnP3hkSWkSl+BMDdMJoDIwOvqfwPKcxRIqLhy1BDPapDgR
+at7GGPZHOiJBhyL8xIkoVNiMpTAK+BcWyqw3/XmnkRd4OJmtWO2y3syJfQOcs4ll
+5+M7sSKGjwZteAf9kRJ/sGsciQ35uMt0WwfCyPQ10WRjeulumijWML3mG90Vr4Tq
+nMfK9Q7q8l0ph49pczm+LiRvRSGsxdRpJQaDrXpIhRMsDQa4bHlW/KNnMoH1V6XK
+V0Jp6VwkYe/iMBhORJhVb3rCk9gZtt58R4oRTklH2yiUAguUSiz5EtBP6DF+bHq/
+pj+bOT0CFqMYs2esWz8sgytnOYFcuX6U1WTdno9uruh8W7TXakdI136z1C2OVnZO
+z2nxbkRs1CTqjSShGL+9V/6pmTW12xB3uD1IutbB5/EjPtffhZ0nPNRAvQoMvfXn
+jSXWgXSHRtQpdaJCbPdzied9v3pKH9MiyRVVz99vfFXQpIsHETdfg6YmV6YBW37+
+WGgHqel62bno/1Afq8K0wM7o6v0PvY1NuLxxAgMBAAGjQjBAMB0GA1UdDgQWBBTF
+7+3M2I0hxkjk49cULqcWk+WYATAPBgNVHRMBAf8EBTADAQH/MA4GA1UdDwEB/wQE
+AwIBBjANBgkqhkiG9w0BAQsFAAOCAgEAUoKsITQfI/Ki2Pm4rzc2IInRNwPWaZ+4
+YRC6ojGYWUfo0Q0lHhVBDOAqVdVXUsv45Mdpox1NcQJeXyFFYEhcCY5JEMEE3Kli
+awLwQ8hOnThJdMkycFRtwUf8jrQ2ntScvd0g1lPJGKm1Vrl2i5VnZu69mP6u775u
++2D2/VnGKhs/I0qUJDAnyIm860Qkmss9vk/Ves6OF8tiwdneHg56/0OGNFK8YT88
+X7vZdrRTvJez/opMEi4r89fO4aL/3Xtw+zuhTaRjAv04l5U/BXCga99igUOLtFkN
+SoxUnMW7gZ/NfaXvCyUeOiDbHPwfmGcCCtRzRBPbUYQaVQNW4AB+dAb/OMRyHdOo
+P2gxXdMJxy6MW2Pg6Nwe0uxhHvLe5e/2mXZgLR6UcnHGCyoyx5JO1UbXHfmpGQrI
++pXObSOYqgs4rZpWDW+N8TEAiMEXnM0ZNjX+VVOg4DwzX5Ze4jLp3zO7Bkqp2IRz
+znfSxqxx4VyjHQy7Ct9f4qNx2No3WqB4K/TUfet27fJhcKVlmtOJNBir+3I+17Q9
+eVzYH6Eze9mCUAyTF6ps3MKCuwJXNq+YJyo5UOGwifUll35HaBC07HPKs5fRJNz2
+YqAo07WjuGS3iGJCz51TzZm+ZGiPTx4SSPfSKcOYKMryMguTjClPPGAyzQWWYezy
+r/6zcCwupvI=
+-----END CERTIFICATE-----
+
+# Issuer: CN=BJCA Global Root CA2 O=BEIJING CERTIFICATE AUTHORITY
+# Subject: CN=BJCA Global Root CA2 O=BEIJING CERTIFICATE AUTHORITY
+# Label: "BJCA Global Root CA2"
+# Serial: 58605626836079930195615843123109055211
+# MD5 Fingerprint: 5e:0a:f6:47:5f:a6:14:e8:11:01:95:3f:4d:01:eb:3c
+# SHA1 Fingerprint: f4:27:86:eb:6e:b8:6d:88:31:67:02:fb:ba:66:a4:53:00:aa:7a:a6
+# SHA256 Fingerprint: 57:4d:f6:93:1e:27:80:39:66:7b:72:0a:fd:c1:60:0f:c2:7e:b6:6d:d3:09:29:79:fb:73:85:64:87:21:28:82
+-----BEGIN CERTIFICATE-----
+MIICJTCCAaugAwIBAgIQLBcIfWQqwP6FGFkGz7RK6zAKBggqhkjOPQQDAzBUMQsw
+CQYDVQQGEwJDTjEmMCQGA1UECgwdQkVJSklORyBDRVJUSUZJQ0FURSBBVVRIT1JJ
+VFkxHTAbBgNVBAMMFEJKQ0EgR2xvYmFsIFJvb3QgQ0EyMB4XDTE5MTIxOTAzMTgy
+MVoXDTQ0MTIxMjAzMTgyMVowVDELMAkGA1UEBhMCQ04xJjAkBgNVBAoMHUJFSUpJ
+TkcgQ0VSVElGSUNBVEUgQVVUSE9SSVRZMR0wGwYDVQQDDBRCSkNBIEdsb2JhbCBS
+b290IENBMjB2MBAGByqGSM49AgEGBSuBBAAiA2IABJ3LgJGNU2e1uVCxA/jlSR9B
+IgmwUVJY1is0j8USRhTFiy8shP8sbqjV8QnjAyEUxEM9fMEsxEtqSs3ph+B99iK+
++kpRuDCK/eHeGBIK9ke35xe/J4rUQUyWPGCWwf0VHKNCMEAwHQYDVR0OBBYEFNJK
+sVF/BvDRgh9Obl+rg/xI1LCRMA8GA1UdEwEB/wQFMAMBAf8wDgYDVR0PAQH/BAQD
+AgEGMAoGCCqGSM49BAMDA2gAMGUCMBq8W9f+qdJUDkpd0m2xQNz0Q9XSSpkZElaA
+94M04TVOSG0ED1cxMDAtsaqdAzjbBgIxAMvMh1PLet8gUXOQwKhbYdDFUDn9hf7B
+43j4ptZLvZuHjw/l1lOWqzzIQNph91Oj9w==
+-----END CERTIFICATE-----
```

### Comparing `certifi-2022.9.24/certifi/core.py` & `certifi-2023.5.7/certifi/core.py`

 * *Files identical despite different names*

### Comparing `certifi-2022.9.24/certifi.egg-info/PKG-INFO` & `certifi-2023.5.7/certifi.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certifi
-Version: 2022.9.24
+Version: 2023.5.7
 Summary: Python package for providing Mozilla's CA Bundle.
 Home-page: https://github.com/certifi/python-certifi
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.com
 License: MPL-2.0
 Project-URL: Source, https://github.com/certifi/python-certifi
 Platform: UNKNOWN
@@ -52,28 +52,14 @@
 Or from the command line::
 
     $ python -m certifi
     /usr/local/lib/python3.7/site-packages/certifi/cacert.pem
 
 Enjoy!
 
-1024-bit Root Certificates
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Browsers and certificate authorities have concluded that 1024-bit keys are
-unacceptably weak for certificates, particularly root certificates. For this
-reason, Mozilla has removed any weak (i.e. 1024-bit key) certificate from its
-bundle, replacing it with an equivalent strong (i.e. 2048-bit or greater key)
-certificate from the same CA. Because Mozilla removed these certificates from
-its bundle, ``certifi`` removed them as well.
-
-In previous versions, ``certifi`` provided the ``certifi.old_where()`` function
-to intentionally re-add the 1024-bit roots back into your bundle. This was not
-recommended in production and therefore was removed at the end of 2018.
-
 .. _`Requests`: https://requests.readthedocs.io/en/master/
 
 Addition/Removal of Certificates
 --------------------------------
 
 Certifi does not support any addition/removal or other modification of the
 CA trust store content. This project is intended to provide a reliable and
```

### Comparing `certifi-2022.9.24/setup.py` & `certifi-2023.5.7/setup.py`

 * *Files identical despite different names*

