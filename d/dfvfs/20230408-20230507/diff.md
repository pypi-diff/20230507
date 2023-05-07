# Comparing `tmp/dfvfs-20230408.tar.gz` & `tmp/dfvfs-20230507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfvfs-20230408.tar", last modified: Sun Apr  9 13:43:04 2023, max compression
+gzip compressed data, was "dfvfs-20230507.tar", last modified: Sun May  7 16:50:11 2023, max compression
```

## Comparing `dfvfs-20230408.tar` & `dfvfs-20230507.tar`

### file list

```diff
@@ -1,686 +1,703 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.953698 dfvfs-20230408/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.457697 dfvfs-20230408/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.541697 dfvfs-20230408/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3491 2023-04-09 13:23:51.000000 dfvfs-20230408/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1857 2023-04-08 04:43:15.000000 dfvfs-20230408/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2158 2023-04-08 04:43:15.000000 dfvfs-20230408/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22087 2023-04-08 04:43:15.000000 dfvfs-20230408/.pylintrc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-12-29 15:59:10.000000 dfvfs-20230408/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1173 2022-11-21 19:14:36.000000 dfvfs-20230408/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      360 2022-11-21 19:18:17.000000 dfvfs-20230408/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2022-11-21 19:18:17.000000 dfvfs-20230408/LICENSE
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      632 2022-12-29 15:59:10.000000 dfvfs-20230408/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      552 2022-12-29 15:59:10.000000 dfvfs-20230408/MANIFEST.test_data.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      900 2023-04-09 13:43:04.953698 dfvfs-20230408/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      473 2022-11-21 19:14:36.000000 dfvfs-20230408/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2023-04-09 13:23:51.000000 dfvfs-20230408/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.458697 dfvfs-20230408/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.541697 dfvfs-20230408/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1008 2023-04-08 04:43:15.000000 dfvfs-20230408/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-04-08 04:43:15.000000 dfvfs-20230408/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-04-08 04:43:15.000000 dfvfs-20230408/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.542697 dfvfs-20230408/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      168 2023-04-09 13:23:51.000000 dfvfs-20230408/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       32 2022-11-21 19:18:17.000000 dfvfs-20230408/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-04-08 04:43:15.000000 dfvfs-20230408/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-04-08 04:43:15.000000 dfvfs-20230408/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      948 2022-11-21 19:18:17.000000 dfvfs-20230408/config/dpkg/copyright
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-04-08 04:43:15.000000 dfvfs-20230408/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.542697 dfvfs-20230408/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2022-11-21 19:18:17.000000 dfvfs-20230408/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.543697 dfvfs-20230408/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2022-11-21 19:18:17.000000 dfvfs-20230408/config/pylint/spelling-private-dict
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4978 2023-01-14 16:01:33.000000 dfvfs-20230408/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.543697 dfvfs-20230408/dfvfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      278 2023-04-09 13:23:51.000000 dfvfs-20230408/dfvfs/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.566697 dfvfs-20230408/dfvfs/analyzer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13902 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/apfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1010 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/apfs_container_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1120 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/bde_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/bzip2_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/cpio_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/cs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/ewf_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/ext_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/fat_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/gpt_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      964 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/gzip_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1370 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/hfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/luksde_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1174 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/lvm_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1168 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/modi_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/ntfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1003 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/phdi_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/qcow_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4938 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/specification.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1057 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/tar_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2266 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/analyzer/tsk_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1040 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/tsk_partition_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/vhdi_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/vmdk_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1071 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/vshadow_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      955 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/xfs_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      968 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/xz_analyzer_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      950 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/analyzer/zip_analyzer_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.568697 dfvfs-20230408/dfvfs/compression/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      247 2022-11-21 19:17:56.000000 dfvfs-20230408/dfvfs/compression/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/compression/bzip2_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/compression/decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2286 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/compression/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/compression/xz_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2118 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/compression/zlib_decompressor.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.570697 dfvfs-20230408/dfvfs/credentials/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      313 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/credentials/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/apfs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/bde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      544 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/credentials/cs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      497 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/encrypted_stream_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2696 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/credentials/keychain.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      498 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/credentials/luksde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/credentials/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.572697 dfvfs-20230408/dfvfs/encoding/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      191 2022-11-21 19:18:12.000000 dfvfs-20230408/dfvfs/encoding/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encoding/base16_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encoding/base32_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encoding/base64_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      392 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/encoding/decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encoding/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.574697 dfvfs-20230408/dfvfs/encryption/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      245 2022-11-25 17:21:27.000000 dfvfs-20230408/dfvfs/encryption/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1478 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/aes_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/blowfish_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3897 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/des3_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2274 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/encryption/rc4_decrypter.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.585697 dfvfs-20230408/dfvfs/file_io/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/file_io/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3960 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs/file_io/apfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/bde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9503 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/compressed_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4645 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/cpio_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4663 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/cs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5995 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/data_range_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9664 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/encoded_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10632 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/encrypted_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2710 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/ewf_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3948 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/ext_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/fake_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4398 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/fat_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4157 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/file_io/file_object_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5577 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/gpt_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2401 2023-01-14 16:01:33.000000 dfvfs-20230408/dfvfs/file_io/gzip_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4501 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/hfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1272 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/luksde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3978 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/lvm_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/modi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4540 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/ntfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6180 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/os_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4378 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/phdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4074 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/file_io/qcow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2733 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/raw_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/sqlite_blob_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4775 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/file_io/tar_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7991 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/tsk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/file_io/tsk_partition_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4313 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/vhdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/vmdk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4106 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/vshadow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/xfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9026 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/file_io/zip_file_io.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.587697 dfvfs-20230408/dfvfs/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29824 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/command_line.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/data_slice.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3992 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/fake_file_system_builder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22280 2023-04-07 07:26:35.000000 dfvfs-20230408/dfvfs/helpers/file_system_searcher.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30704 2023-04-07 04:40:26.000000 dfvfs-20230408/dfvfs/helpers/source_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6081 2022-12-23 11:41:15.000000 dfvfs-20230408/dfvfs/helpers/text_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28568 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/volume_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9518 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/helpers/windows_path_resolver.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.593697 dfvfs-20230408/dfvfs/lib/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1687 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/apfs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/bde_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10516 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/cpio.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4230 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/cpio.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/cs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/data_format.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/decorators.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4694 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1053 2022-11-21 19:18:10.000000 dfvfs-20230408/dfvfs/lib/errors.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3502 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/ewf_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/lib/glob2regex.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      723 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/gpt_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19596 2023-01-14 16:01:33.000000 dfvfs-20230408/dfvfs/lib/gzipfile.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/gzipfile.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1160 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/luksde_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/lvm_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12570 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/raw_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/sqlite_database.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/lib/tsk_image.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4930 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/tsk_partition.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      745 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/lib/vshadow_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.593697 dfvfs-20230408/dfvfs/mount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/mount/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/mount/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.602697 dfvfs-20230408/dfvfs/path/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1564 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/apfs_container_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/apfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1769 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/bde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1387 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/compressed_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/cpio_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2397 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/cs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/data_range_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/encoded_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/encrypted_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/ewf_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/ext_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3742 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      940 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/fake_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/fat_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/gpt_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      782 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/gzip_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/hfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      923 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/location_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1217 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/luksde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/lvm_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      798 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/modi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/mount_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/ntfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/os_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4043 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/phdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/qcow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      800 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/raw_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/sqlite_blob_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      947 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/tar_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/tsk_partition_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1943 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/tsk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      810 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/vhdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/vmdk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/vshadow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/path/xfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/path/zip_path_spec.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.602697 dfvfs-20230408/dfvfs/resolver/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:56.000000 dfvfs-20230408/dfvfs/resolver/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4365 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver/context.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6142 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver/resolver.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.609697 dfvfs-20230408/dfvfs/resolver_helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2723 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      904 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/apfs_container_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/apfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/bde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/cpio_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/cs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/data_range_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1296 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      824 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/ewf_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/ext_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/fake_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/fat_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/gpt_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1205 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/gzip_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/hfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/luksde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1209 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/lvm_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      846 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/modi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/ntfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/os_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/phdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/qcow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/raw_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/resolver_helpers/resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1300 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/tar_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1312 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/tsk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      830 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/vhdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/vmdk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/vshadow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/xfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/resolver_helpers/zip_resolver_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.610697 dfvfs-20230408/dfvfs/serializer/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:18:12.000000 dfvfs-20230408/dfvfs/serializer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5458 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/serializer/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/serializer/serializer.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.626697 dfvfs-20230408/dfvfs/vfs/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:59.000000 dfvfs-20230408/dfvfs/vfs/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3622 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_container_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4534 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_container_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4513 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_container_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8895 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/apfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2188 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/bde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2758 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/bde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/compressed_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2621 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/compressed_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cpio_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7019 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cpio_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cpio_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1112 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4353 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5012 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/cs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/data_range_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2781 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/data_range_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      859 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      961 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/encoded_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2534 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/encoded_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/encrypted_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2699 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/encrypted_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ext_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ext_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9823 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ext_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5159 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/ext_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      844 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/extent.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1212 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fake_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4684 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fake_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5004 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fake_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fat_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7675 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fat_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/fat_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11742 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7136 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/gpt_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3578 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/gpt_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4352 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/gpt_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1849 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/gzip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1019 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/gzip_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10348 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5316 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/hfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1944 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/luksde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/luksde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/lvm_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/lvm_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4750 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/lvm_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5041 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ntfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ntfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ntfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12181 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/ntfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5882 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/ntfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3067 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/os_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1662 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/os_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9286 2023-01-01 18:32:24.000000 dfvfs-20230408/dfvfs/vfs/os_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6345 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/os_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      665 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/root_only_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1699 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/root_only_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/sqlite_blob_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4202 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/sqlite_blob_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3520 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/sqlite_blob_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tar_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6442 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tar_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5180 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tar_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4281 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3018 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27588 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7175 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_partition_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4278 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_partition_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4196 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/tsk_partition_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1128 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/vshadow_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4224 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/vshadow_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4412 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/vshadow_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/xfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/xfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8567 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/xfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5313 2022-12-23 11:39:27.000000 dfvfs-20230408/dfvfs/vfs/xfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/zip_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6332 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/zip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/vfs/zip_file_system.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.628697 dfvfs-20230408/dfvfs/volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      332 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/volume/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2022-12-29 15:59:11.000000 dfvfs-20230408/dfvfs/volume/apfs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/cs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/gpt_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/lvm_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3054 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/tsk_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7299 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2022-12-29 15:59:12.000000 dfvfs-20230408/dfvfs/volume/vshadow_volume_system.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.556697 dfvfs-20230408/dfvfs.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      900 2023-04-09 13:43:01.000000 dfvfs-20230408/dfvfs.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20370 2023-04-09 13:43:04.000000 dfvfs-20230408/dfvfs.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-04-09 13:43:01.000000 dfvfs-20230408/dfvfs.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2022-11-21 19:14:18.000000 dfvfs-20230408/dfvfs.egg-info/not-zip-safe
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      729 2023-04-09 13:43:02.000000 dfvfs-20230408/dfvfs.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        6 2023-04-09 13:43:02.000000 dfvfs-20230408/dfvfs.egg-info/top_level.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2022-12-29 15:59:10.000000 dfvfs-20230408/dfvfs.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.649697 dfvfs-20230408/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2023-04-08 04:43:15.000000 dfvfs-20230408/docs/conf.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-04-08 04:43:23.000000 dfvfs-20230408/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.658697 dfvfs-20230408/docs/sources/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3182 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/Code-snippets.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14179 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/Path-specifications.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3922 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/Supported-formats.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.709698 dfvfs-20230408/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.analyzer.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1125 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.compression.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.credentials.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1032 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.encoding.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1264 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.encryption.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6140 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.file_io.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.helpers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.lib.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      325 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.mount.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6547 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.path.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      501 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.resolver.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8176 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.resolver_helpers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      461 2022-11-21 19:15:00.000000 dfvfs-20230408/docs/sources/api/dfvfs.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      551 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/api/dfvfs.serializer.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15405 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.vfs.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/api/dfvfs.volume.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       52 2022-11-21 19:15:00.000000 dfvfs-20230408/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.727697 dfvfs-20230408/docs/sources/developer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6837 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/developer/Adding-new-type.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5996 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/developer/Helpers.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3991 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/developer/Internals.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      447 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/developer/Testing.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      398 2022-12-23 11:39:27.000000 dfvfs-20230408/docs/sources/developer/index.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.728697 dfvfs-20230408/docs/sources/user/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1597 2022-12-29 15:59:12.000000 dfvfs-20230408/docs/sources/user/Installation-instructions.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      282 2022-11-21 19:15:01.000000 dfvfs-20230408/docs/sources/user/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      787 2023-04-09 13:23:51.000000 dfvfs-20230408/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-12-29 15:59:12.000000 dfvfs-20230408/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1314 2023-04-09 13:43:04.954698 dfvfs-20230408/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6873 2023-04-08 04:43:15.000000 dfvfs-20230408/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-29 15:59:13.000000 dfvfs-20230408/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-08 04:43:15.000000 dfvfs-20230408/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.729698 dfvfs-20230408/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:19.000000 dfvfs-20230408/tests/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.729698 dfvfs-20230408/tests/analyzer/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230408/tests/analyzer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18459 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/analyzer/analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      912 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/analyzer/specification.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.730697 dfvfs-20230408/tests/compression/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:19.000000 dfvfs-20230408/tests/compression/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1231 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/bzip2_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      224 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/xz_decompressor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/compression/zlib_decompressor.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.731697 dfvfs-20230408/tests/credentials/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:36.000000 dfvfs-20230408/tests/credentials/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      543 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/apfs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/bde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      475 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      521 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/credentials/cs_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/encrypted_stream_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/keychain.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/luksde_credentials.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/credentials/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.732698 dfvfs-20230408/tests/encoding/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230408/tests/encoding/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/base16_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/base32_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      801 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/base64_decoder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      214 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encoding/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.733698 dfvfs-20230408/tests/encryption/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:32.000000 dfvfs-20230408/tests/encryption/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3435 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/aes_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3643 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/blowfish_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3442 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/des3_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2302 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/encryption/rc4_decrypter.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/encryption/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.738697 dfvfs-20230408/tests/file_io/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:34.000000 dfvfs-20230408/tests/file_io/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4656 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/apfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/bde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9395 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/compressed_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6471 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/cpio_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/cs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2793 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/data_range_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6975 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/encoded_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14381 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/encrypted_stream_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3128 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/ewf_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4396 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/ext_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3463 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/fake_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3104 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/fat_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/gpt_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/gzip_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3512 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/hfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3659 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/luksde_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6235 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/lvm_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/modi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3082 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/ntfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5213 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/os_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/phdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/qcow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2868 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/raw_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3603 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/sqlite_blob_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1843 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/tar_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33122 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12616 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/tsk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1126 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/tsk_partition_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16839 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/vhdi_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/vmdk_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/file_io/vshadow_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4369 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/xfs_file_io.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1895 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/file_io/zip_file_io.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.739698 dfvfs-20230408/tests/helpers/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:25.000000 dfvfs-20230408/tests/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39320 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/helpers/command_line.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2714 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/helpers/data_slice.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2644 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/helpers/fake_file_system_builder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26712 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/helpers/file_system_searcher.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35980 2023-04-07 04:40:26.000000 dfvfs-20230408/tests/helpers/source_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8964 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/helpers/text_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38545 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/helpers/volume_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6744 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/helpers/windows_path_resolver.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.740697 dfvfs-20230408/tests/lib/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:27.000000 dfvfs-20230408/tests/lib/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5054 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/lib/apfs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/lib/cpio.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1756 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/lib/cs_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16350 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/lib/ewf_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1923 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/lib/glob2regex.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5410 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/lib/gzipfile.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/lib/lvm_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20600 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/lib/raw_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.741697 dfvfs-20230408/tests/mount/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:20.000000 dfvfs-20230408/tests/mount/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/mount/manager.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.745698 dfvfs-20230408/tests/path/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:26.000000 dfvfs-20230408/tests/path/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2784 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/apfs_container_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2372 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/apfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/bde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/compressed_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/cpio_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/cs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1752 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/data_range_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1538 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/encoded_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/encryption_stream_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/ewf_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/ext_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1580 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/fake_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/fat_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/gpt_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/gzip_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/hfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/luksde_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2463 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/lvm_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/modi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      945 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/mount_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3362 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/ntfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/os_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2585 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/phdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/qcow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/raw_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/sqlite_blob_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/tar_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      778 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/tsk_partition_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/tsk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1141 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/path/vhdi_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/vmdk_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/vshadow_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/xfs_path_spec.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/path/zip_path_spec.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.745698 dfvfs-20230408/tests/resolver/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5408 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver/context.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.750697 dfvfs-20230408/tests/resolver_helpers/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:30.000000 dfvfs-20230408/tests/resolver_helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/apfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/bde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/compressed_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/cpio_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/cs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1641 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/encoded_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/encrypted_stream_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/ewf_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/ext_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/fat_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/gpt_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/gzip_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/hfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/luksde_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/lvm_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/modi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/ntfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/os_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/phdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/qcow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/raw_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1617 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/sqlite_blob_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/tar_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2525 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1882 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/tsk_partition_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/tsk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/vhdi_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1442 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/vmdk_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/resolver_helpers/vshadow_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/xfs_resolver_helper.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/resolver_helpers/zip_resolver_helper.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.750697 dfvfs-20230408/tests/serializer/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230408/tests/serializer/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/serializer/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1996 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.763697 dfvfs-20230408/tests/vfs/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:21.000000 dfvfs-20230408/tests/vfs/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2458 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_container_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16546 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_container_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5723 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/apfs_container_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28404 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/apfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4316 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/apfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6755 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/bde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/bde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4742 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/compressed_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/compressed_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1790 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/cpio_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8419 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/cpio_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3366 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/cpio_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/cs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6279 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/cs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/data_range_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2658 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/data_range_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      883 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3796 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/encoded_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2771 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/encoded_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4144 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/encrypted_stream_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/encrypted_stream_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ext_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2113 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ext_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23810 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ext_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3983 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/ext_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      438 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/extent.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2323 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fake_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10644 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fake_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2904 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/fake_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fat_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13064 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fat_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4069 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/fat_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11194 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2749 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/gpt_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7790 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/gpt_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/gpt_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4674 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/gzip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2511 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/gzip_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/hfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4024 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/hfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/hfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17357 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/hfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4062 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/hfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4814 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/luksde_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2549 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/luksde_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/lvm_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8162 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/lvm_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6462 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/lvm_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9765 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_attibute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27468 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4115 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/ntfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/os_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9917 2023-01-01 18:32:24.000000 dfvfs-20230408/tests/vfs/os_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6171 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/os_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2628 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/sqlite_blob_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5588 2022-12-29 15:59:14.000000 dfvfs-20230408/tests/vfs/sqlite_blob_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/sqlite_blob_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1766 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tar_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8767 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tar_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5544 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/tar_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_data_stream.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1893 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    79436 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/tsk_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1904 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_partition_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14462 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/tsk_partition_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6657 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/tsk_partition_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/vshadow_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8488 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/vshadow_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6413 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/vshadow_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2228 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/xfs_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2112 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/xfs_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13190 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/xfs_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3985 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/xfs_file_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1763 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/zip_directory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13454 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/vfs/zip_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2022-12-23 11:39:29.000000 dfvfs-20230408/tests/vfs/zip_file_system.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.765698 dfvfs-20230408/tests/volume/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:18.000000 dfvfs-20230408/tests/volume/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2698 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/apfs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2088 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/cs_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/gpt_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3695 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/lvm_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8084 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/tsk_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3543 2022-12-29 15:59:15.000000 dfvfs-20230408/tests/volume/vshadow_volume_system.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1451 2023-04-08 04:43:15.000000 dfvfs-20230408/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-09 13:43:04.938698 dfvfs-20230408/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:55.000000 dfvfs-20230408/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-04-08 04:43:15.000000 dfvfs-20230408/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-04-08 04:43:15.000000 dfvfs-20230408/utils/dependencies.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    14019 2022-12-29 15:59:15.000000 dfvfs-20230408/utils/generate_test_data_linux.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4836 2022-12-29 15:59:15.000000 dfvfs-20230408/utils/generate_test_data_macos.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14212 2022-12-29 15:59:15.000000 dfvfs-20230408/utils/generate_test_data_windows.bat
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      815 2022-11-21 19:17:55.000000 dfvfs-20230408/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.401402 dfvfs-20230507/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.219402 dfvfs-20230507/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.269402 dfvfs-20230507/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3525 2023-05-07 07:19:13.000000 dfvfs-20230507/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1874 2023-05-07 07:19:13.000000 dfvfs-20230507/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5595 2023-05-07 07:19:13.000000 dfvfs-20230507/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22087 2023-05-06 09:14:08.000000 dfvfs-20230507/.pylintrc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-12-29 15:59:10.000000 dfvfs-20230507/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1173 2022-11-21 19:14:36.000000 dfvfs-20230507/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      360 2022-11-21 19:18:17.000000 dfvfs-20230507/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2022-11-21 19:18:17.000000 dfvfs-20230507/LICENSE
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      632 2022-12-29 15:59:10.000000 dfvfs-20230507/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      552 2022-12-29 15:59:10.000000 dfvfs-20230507/MANIFEST.test_data.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      900 2023-05-07 16:50:11.401402 dfvfs-20230507/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      473 2022-11-21 19:14:36.000000 dfvfs-20230507/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2023-05-06 09:14:08.000000 dfvfs-20230507/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.220402 dfvfs-20230507/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.270402 dfvfs-20230507/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2023-05-07 07:19:13.000000 dfvfs-20230507/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-06 09:14:08.000000 dfvfs-20230507/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-06 09:14:08.000000 dfvfs-20230507/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.271402 dfvfs-20230507/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      168 2023-05-07 16:07:46.000000 dfvfs-20230507/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       32 2022-11-21 19:18:17.000000 dfvfs-20230507/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-06 09:14:08.000000 dfvfs-20230507/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2023-05-07 07:19:13.000000 dfvfs-20230507/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      948 2022-11-21 19:18:17.000000 dfvfs-20230507/config/dpkg/copyright
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-06 09:14:08.000000 dfvfs-20230507/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.271402 dfvfs-20230507/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2022-11-21 19:18:17.000000 dfvfs-20230507/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.271402 dfvfs-20230507/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2022-11-21 19:18:17.000000 dfvfs-20230507/config/pylint/spelling-private-dict
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5156 2023-05-07 07:19:13.000000 dfvfs-20230507/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.271402 dfvfs-20230507/dfvfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      278 2023-05-07 16:07:46.000000 dfvfs-20230507/dfvfs/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.290402 dfvfs-20230507/dfvfs/analyzer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1488 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/analyzer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13902 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/analyzer/analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/analyzer/analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/apfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1010 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/apfs_container_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/analyzer/apm_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1120 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/bde_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/bzip2_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1404 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/cpio_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/analyzer/cs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/ewf_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1182 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/ext_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/analyzer/fat_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/gpt_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      964 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/gzip_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1370 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/analyzer/hfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/luksde_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1174 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/lvm_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1168 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/analyzer/modi_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/ntfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1003 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/analyzer/phdi_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/qcow_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4938 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/analyzer/specification.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1057 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/tar_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2266 2023-05-03 04:30:37.000000 dfvfs-20230507/dfvfs/analyzer/tsk_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1040 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/tsk_partition_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/vhdi_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/vmdk_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1071 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/vshadow_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      955 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/xfs_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      968 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/xz_analyzer_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      950 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/analyzer/zip_analyzer_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.290402 dfvfs-20230507/dfvfs/compression/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      247 2022-11-21 19:17:56.000000 dfvfs-20230507/dfvfs/compression/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/compression/bzip2_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/compression/decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2286 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/compression/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/compression/xz_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2118 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/compression/zlib_decompressor.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.292402 dfvfs-20230507/dfvfs/credentials/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      313 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/credentials/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/credentials/apfs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/credentials/bde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/credentials/credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      544 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/credentials/cs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      497 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/credentials/encrypted_stream_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2696 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/credentials/keychain.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      498 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/credentials/luksde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1902 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/credentials/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.292402 dfvfs-20230507/dfvfs/encoding/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      191 2022-11-21 19:18:12.000000 dfvfs-20230507/dfvfs/encoding/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encoding/base16_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encoding/base32_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encoding/base64_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      392 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/encoding/decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encoding/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.293402 dfvfs-20230507/dfvfs/encryption/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      245 2022-11-25 17:21:27.000000 dfvfs-20230507/dfvfs/encryption/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1478 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encryption/aes_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encryption/blowfish_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3897 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encryption/decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encryption/des3_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2274 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encryption/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/encryption/rc4_decrypter.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.298402 dfvfs-20230507/dfvfs/file_io/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/file_io/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3960 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs/file_io/apfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5561 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/file_io/apm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/bde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9503 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/compressed_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4645 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/cpio_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4663 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/cs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5995 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/data_range_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9664 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/encoded_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10632 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/encrypted_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2710 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/ewf_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3948 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/ext_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/fake_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4398 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/fat_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4157 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/file_io/file_object_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5577 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/gpt_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2401 2023-01-14 16:01:33.000000 dfvfs-20230507/dfvfs/file_io/gzip_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4501 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/hfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1272 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/luksde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3978 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/lvm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/modi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4540 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/ntfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6180 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/os_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4378 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/phdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4074 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/file_io/qcow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2733 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/raw_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/sqlite_blob_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4775 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/file_io/tar_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7991 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/tsk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2370 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/file_io/tsk_partition_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4313 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/vhdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/vmdk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4106 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/vshadow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/xfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9026 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/file_io/zip_file_io.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.300402 dfvfs-20230507/dfvfs/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29824 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/helpers/command_line.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/helpers/data_slice.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3992 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/helpers/fake_file_system_builder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22177 2023-04-29 09:33:20.000000 dfvfs-20230507/dfvfs/helpers/file_system_searcher.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30704 2023-04-07 04:40:26.000000 dfvfs-20230507/dfvfs/helpers/source_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6081 2022-12-23 11:41:15.000000 dfvfs-20230507/dfvfs/helpers/text_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28568 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/helpers/volume_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9517 2023-04-29 09:33:20.000000 dfvfs-20230507/dfvfs/helpers/windows_path_resolver.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.303402 dfvfs-20230507/dfvfs/lib/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1687 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/apfs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      722 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/lib/apm_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/bde_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10516 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/cpio.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4230 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/cpio.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/cs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3532 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/data_format.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/decorators.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4769 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/lib/definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1053 2022-11-21 19:18:10.000000 dfvfs-20230507/dfvfs/lib/errors.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3502 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/ewf_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/lib/glob2regex.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      723 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/gpt_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19596 2023-01-14 16:01:33.000000 dfvfs-20230507/dfvfs/lib/gzipfile.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/gzipfile.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1160 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/luksde_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      866 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/lvm_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12570 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/raw_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/sqlite_database.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/lib/tsk_image.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5460 2023-05-03 04:30:43.000000 dfvfs-20230507/dfvfs/lib/tsk_partition.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      745 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/lib/vshadow_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.303402 dfvfs-20230507/dfvfs/mount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/mount/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/mount/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.308402 dfvfs-20230507/dfvfs/path/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/path/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1564 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/apfs_container_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1547 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/apfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1473 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/path/apm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1769 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/bde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1387 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/compressed_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/path/cpio_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2397 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/cs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/data_range_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/encoded_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/encrypted_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/path/ewf_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/ext_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3742 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      940 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/path/fake_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/fat_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/gpt_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      782 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/path/gzip_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/hfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      923 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/location_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1217 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/luksde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1482 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/lvm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      798 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/modi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/mount_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2364 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/ntfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/os_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4043 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/phdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/path/qcow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      800 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/path/raw_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/sqlite_blob_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      947 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/path/tar_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/tsk_partition_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1943 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/tsk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      810 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/vhdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      784 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/path/vmdk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/vshadow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/path/xfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      978 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/path/zip_path_spec.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.308402 dfvfs-20230507/dfvfs/resolver/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:56.000000 dfvfs-20230507/dfvfs/resolver/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4365 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/resolver/context.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6142 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/resolver/resolver.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.313402 dfvfs-20230507/dfvfs/resolver_helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2813 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/resolver_helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      904 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/apfs_container_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/apfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1206 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/resolver_helpers/apm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/bde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/cpio_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1198 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/resolver_helpers/cs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/data_range_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1296 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1318 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      824 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/ewf_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/ext_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/fake_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/resolver_helpers/fat_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/gpt_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1205 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/gzip_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/hfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/luksde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1209 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/lvm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/resolver_helpers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      846 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/resolver_helpers/modi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1195 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/ntfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/os_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/resolver_helpers/phdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/qcow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/raw_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/resolver_helpers/resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1300 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/tar_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1312 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/tsk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      830 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/vhdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      832 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/vmdk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1246 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/vshadow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/xfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1184 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/resolver_helpers/zip_resolver_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.313402 dfvfs-20230507/dfvfs/serializer/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:18:12.000000 dfvfs-20230507/dfvfs/serializer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5458 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/serializer/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/serializer/serializer.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.325402 dfvfs-20230507/dfvfs/vfs/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:59.000000 dfvfs-20230507/dfvfs/vfs/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3622 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/apfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/apfs_container_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4534 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/apfs_container_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4513 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/apfs_container_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/apfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8895 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/apfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/apfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1101 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/vfs/apm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3577 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/vfs/apm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4352 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/vfs/apm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2188 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/bde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2758 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/bde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/compressed_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2621 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/compressed_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/cpio_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7019 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/cpio_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4635 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/cpio_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1112 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/cs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4353 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/cs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5012 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/cs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/data_range_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2781 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/data_range_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      859 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      961 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/encoded_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2534 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/encoded_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/encrypted_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2699 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/encrypted_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/ext_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/ext_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9823 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/ext_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5159 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/ext_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      844 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/extent.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1212 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/fake_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4684 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/fake_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5004 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/fake_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/fat_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7675 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/fat_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/fat_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11742 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7136 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/gpt_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3578 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/gpt_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4352 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/gpt_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1849 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/gzip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1019 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/gzip_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/hfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/hfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/hfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10348 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/hfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5316 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/hfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1944 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/luksde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/luksde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/lvm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/lvm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4750 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/lvm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5041 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/ntfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/ntfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1838 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/ntfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12181 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/ntfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5882 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/ntfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3067 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/os_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1662 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/os_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9286 2023-01-01 18:32:24.000000 dfvfs-20230507/dfvfs/vfs/os_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6345 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/os_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      665 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/root_only_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1699 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/root_only_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/sqlite_blob_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4202 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/sqlite_blob_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3520 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/sqlite_blob_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2093 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/tar_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6442 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/tar_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5180 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/tar_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4281 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/tsk_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3018 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/tsk_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/tsk_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27588 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/tsk_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7175 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/tsk_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2023-05-03 03:49:58.000000 dfvfs-20230507/dfvfs/vfs/tsk_partition_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4278 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/tsk_partition_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4196 2023-05-03 03:49:58.000000 dfvfs-20230507/dfvfs/vfs/tsk_partition_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1128 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/vshadow_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4224 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/vshadow_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4412 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/vshadow_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3601 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/xfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/xfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8567 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/xfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5313 2022-12-23 11:39:27.000000 dfvfs-20230507/dfvfs/vfs/xfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/zip_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6332 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/zip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/vfs/zip_file_system.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.326402 dfvfs-20230507/dfvfs/volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      375 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/volume/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2022-12-29 15:59:11.000000 dfvfs-20230507/dfvfs/volume/apfs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1421 2023-05-07 07:19:13.000000 dfvfs-20230507/dfvfs/volume/apm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1513 2022-12-29 15:59:12.000000 dfvfs-20230507/dfvfs/volume/cs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1710 2022-12-29 15:59:12.000000 dfvfs-20230507/dfvfs/volume/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2022-12-29 15:59:12.000000 dfvfs-20230507/dfvfs/volume/gpt_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2022-12-29 15:59:12.000000 dfvfs-20230507/dfvfs/volume/lvm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3054 2022-12-29 15:59:12.000000 dfvfs-20230507/dfvfs/volume/tsk_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7299 2022-12-29 15:59:12.000000 dfvfs-20230507/dfvfs/volume/volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2022-12-29 15:59:12.000000 dfvfs-20230507/dfvfs/volume/vshadow_volume_system.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.286402 dfvfs-20230507/dfvfs.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      900 2023-05-07 16:50:09.000000 dfvfs-20230507/dfvfs.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    20906 2023-05-07 16:50:11.000000 dfvfs-20230507/dfvfs.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-07 16:50:09.000000 dfvfs-20230507/dfvfs.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2022-11-21 19:14:18.000000 dfvfs-20230507/dfvfs.egg-info/not-zip-safe
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      755 2023-05-07 16:50:09.000000 dfvfs-20230507/dfvfs.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        6 2023-05-07 16:50:09.000000 dfvfs-20230507/dfvfs.egg-info/top_level.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2022-12-29 15:59:10.000000 dfvfs-20230507/dfvfs.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.326402 dfvfs-20230507/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2023-05-06 09:14:08.000000 dfvfs-20230507/docs/conf.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2022-12-29 15:59:12.000000 dfvfs-20230507/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-05-07 07:19:13.000000 dfvfs-20230507/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.327402 dfvfs-20230507/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3182 2022-12-29 15:59:12.000000 dfvfs-20230507/docs/sources/Code-snippets.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14179 2022-12-29 15:59:12.000000 dfvfs-20230507/docs/sources/Path-specifications.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4098 2023-05-07 07:19:13.000000 dfvfs-20230507/docs/sources/Supported-formats.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.329402 dfvfs-20230507/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6275 2023-05-07 16:07:46.000000 dfvfs-20230507/docs/sources/api/dfvfs.analyzer.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1125 2022-12-23 11:39:27.000000 dfvfs-20230507/docs/sources/api/dfvfs.compression.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2022-12-29 15:59:12.000000 dfvfs-20230507/docs/sources/api/dfvfs.credentials.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1032 2022-12-23 11:39:27.000000 dfvfs-20230507/docs/sources/api/dfvfs.encoding.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1264 2022-12-23 11:39:27.000000 dfvfs-20230507/docs/sources/api/dfvfs.encryption.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2023-05-07 16:07:46.000000 dfvfs-20230507/docs/sources/api/dfvfs.file_io.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2022-12-23 11:39:27.000000 dfvfs-20230507/docs/sources/api/dfvfs.helpers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3193 2023-05-07 16:07:46.000000 dfvfs-20230507/docs/sources/api/dfvfs.lib.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      325 2022-12-23 11:39:27.000000 dfvfs-20230507/docs/sources/api/dfvfs.mount.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6712 2023-05-07 16:07:46.000000 dfvfs-20230507/docs/sources/api/dfvfs.path.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      501 2022-12-29 15:59:12.000000 dfvfs-20230507/docs/sources/api/dfvfs.resolver.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8397 2023-05-07 16:07:46.000000 dfvfs-20230507/docs/sources/api/dfvfs.resolver_helpers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      461 2022-11-21 19:15:00.000000 dfvfs-20230507/docs/sources/api/dfvfs.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      551 2022-12-23 11:39:27.000000 dfvfs-20230507/docs/sources/api/dfvfs.serializer.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15898 2023-05-07 16:07:46.000000 dfvfs-20230507/docs/sources/api/dfvfs.vfs.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1793 2023-05-07 16:07:46.000000 dfvfs-20230507/docs/sources/api/dfvfs.volume.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       52 2022-11-21 19:15:00.000000 dfvfs-20230507/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.330402 dfvfs-20230507/docs/sources/developer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6837 2022-12-23 11:39:27.000000 dfvfs-20230507/docs/sources/developer/Adding-new-type.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5996 2022-12-23 11:39:27.000000 dfvfs-20230507/docs/sources/developer/Helpers.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3991 2022-12-29 15:59:12.000000 dfvfs-20230507/docs/sources/developer/Internals.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      447 2022-12-29 15:59:12.000000 dfvfs-20230507/docs/sources/developer/Testing.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      398 2022-12-23 11:39:27.000000 dfvfs-20230507/docs/sources/developer/index.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.330402 dfvfs-20230507/docs/sources/user/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1597 2022-12-29 15:59:12.000000 dfvfs-20230507/docs/sources/user/Installation-instructions.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      282 2022-11-21 19:15:01.000000 dfvfs-20230507/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      815 2023-05-07 07:19:13.000000 dfvfs-20230507/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-12-29 15:59:12.000000 dfvfs-20230507/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2023-05-07 16:50:11.402402 dfvfs-20230507/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6873 2023-05-06 09:14:08.000000 dfvfs-20230507/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-29 15:59:13.000000 dfvfs-20230507/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 09:14:08.000000 dfvfs-20230507/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.330402 dfvfs-20230507/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:19.000000 dfvfs-20230507/tests/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.331402 dfvfs-20230507/tests/analyzer/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230507/tests/analyzer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18459 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/analyzer/analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      912 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/analyzer/specification.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.332402 dfvfs-20230507/tests/compression/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:19.000000 dfvfs-20230507/tests/compression/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1231 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/compression/bzip2_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2083 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/compression/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      224 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/compression/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/compression/xz_decompressor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/compression/zlib_decompressor.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.333402 dfvfs-20230507/tests/credentials/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:36.000000 dfvfs-20230507/tests/credentials/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      543 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/credentials/apfs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/credentials/bde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      475 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/credentials/credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      521 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/credentials/cs_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      562 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/credentials/encrypted_stream_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/credentials/keychain.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/credentials/luksde_credentials.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/credentials/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.334402 dfvfs-20230507/tests/encoding/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230507/tests/encoding/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/encoding/base16_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/encoding/base32_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      801 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/encoding/base64_decoder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/encoding/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      214 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/encoding/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.335402 dfvfs-20230507/tests/encryption/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:32.000000 dfvfs-20230507/tests/encryption/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3435 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/encryption/aes_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3643 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/encryption/blowfish_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/encryption/decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3442 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/encryption/des3_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2302 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/encryption/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/encryption/rc4_decrypter.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/encryption/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.339402 dfvfs-20230507/tests/file_io/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:34.000000 dfvfs-20230507/tests/file_io/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4656 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/apfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3037 2023-05-07 07:19:13.000000 dfvfs-20230507/tests/file_io/apm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/bde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9395 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/compressed_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6471 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/cpio_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/cs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2793 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/data_range_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6975 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/encoded_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14381 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/encrypted_stream_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3128 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/ewf_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4396 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/ext_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3463 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/fake_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3104 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/fat_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/gpt_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/gzip_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3512 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/hfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3659 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/luksde_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6235 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/lvm_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/modi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3082 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/ntfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5213 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/os_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3042 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/phdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/qcow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2868 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/raw_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3603 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/sqlite_blob_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1843 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/tar_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33122 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12616 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/tsk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1126 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/tsk_partition_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16839 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/vhdi_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/vmdk_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5037 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/file_io/vshadow_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4369 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/xfs_file_io.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1895 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/file_io/zip_file_io.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.340402 dfvfs-20230507/tests/helpers/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:25.000000 dfvfs-20230507/tests/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39320 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/helpers/command_line.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2714 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/helpers/data_slice.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2644 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/helpers/fake_file_system_builder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26712 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/helpers/file_system_searcher.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35980 2023-04-07 04:40:26.000000 dfvfs-20230507/tests/helpers/source_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8964 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/helpers/text_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38545 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/helpers/volume_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6744 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/helpers/windows_path_resolver.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.341402 dfvfs-20230507/tests/lib/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:27.000000 dfvfs-20230507/tests/lib/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5054 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/lib/apfs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9118 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/lib/cpio.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1756 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/lib/cs_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16350 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/lib/ewf_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1923 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/lib/glob2regex.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5410 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/lib/gzipfile.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1806 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/lib/lvm_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20600 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/lib/raw_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.342402 dfvfs-20230507/tests/mount/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:20.000000 dfvfs-20230507/tests/mount/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/mount/manager.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.347402 dfvfs-20230507/tests/path/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:26.000000 dfvfs-20230507/tests/path/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2784 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/apfs_container_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2372 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/apfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2023-05-07 07:19:13.000000 dfvfs-20230507/tests/path/apm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/bde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/compressed_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/cpio_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/path/cs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1752 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/data_range_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1538 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/encoded_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/encryption_stream_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1102 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/ewf_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/ext_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1580 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/fake_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/path/fat_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2457 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/path/gpt_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/gzip_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/path/hfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/luksde_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2463 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/lvm_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/path/modi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      945 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/path/mount_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3362 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/ntfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/path/os_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2585 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/path/phdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/qcow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/raw_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/sqlite_blob_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/tar_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      778 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/tsk_partition_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/tsk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1141 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/path/vhdi_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1115 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/vmdk_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/vshadow_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/xfs_path_spec.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/path/zip_path_spec.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.347402 dfvfs-20230507/tests/resolver/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5408 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/resolver/context.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.351402 dfvfs-20230507/tests/resolver_helpers/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:30.000000 dfvfs-20230507/tests/resolver_helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/apfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2023-05-07 07:19:13.000000 dfvfs-20230507/tests/resolver_helpers/apm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/bde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/compressed_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/cpio_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/resolver_helpers/cs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1641 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/encoded_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/encrypted_stream_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/ewf_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/ext_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/resolver_helpers/fat_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/gpt_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/gzip_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/hfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/luksde_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/lvm_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1194 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/resolver_helpers/modi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/resolver_helpers/ntfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/os_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1466 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/resolver_helpers/phdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/qcow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/raw_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1617 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/sqlite_blob_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1413 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/tar_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2525 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1882 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/tsk_partition_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/tsk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/resolver_helpers/vhdi_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1442 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/vmdk_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/resolver_helpers/vshadow_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/xfs_resolver_helper.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/resolver_helpers/zip_resolver_helper.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.351402 dfvfs-20230507/tests/serializer/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:28.000000 dfvfs-20230507/tests/serializer/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/serializer/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1996 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.363402 dfvfs-20230507/tests/vfs/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:21.000000 dfvfs-20230507/tests/vfs/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2458 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/apfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/apfs_container_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16546 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/apfs_container_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5723 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/apfs_container_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/apfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28404 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/apfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4316 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/apfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1883 2023-05-07 07:19:13.000000 dfvfs-20230507/tests/vfs/apm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7699 2023-05-07 07:19:13.000000 dfvfs-20230507/tests/vfs/apm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5973 2023-05-07 07:19:13.000000 dfvfs-20230507/tests/vfs/apm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      545 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6755 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/bde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/bde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4742 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/compressed_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/compressed_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1790 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/cpio_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8419 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/cpio_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3366 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/cpio_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8349 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/cs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6279 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/cs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/data_range_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2658 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/data_range_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      883 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3796 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/encoded_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2771 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/encoded_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4144 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/encrypted_stream_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/encrypted_stream_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2226 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/ext_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2113 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/ext_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23810 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/ext_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3983 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/ext_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      438 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/extent.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2323 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/fake_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10644 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/fake_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2904 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/fake_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/fat_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13064 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/fat_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4069 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/fat_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11194 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2749 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/gpt_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7790 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/gpt_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/gpt_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4674 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/gzip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2511 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/gzip_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/hfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4024 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/hfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2116 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/hfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17357 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/hfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4062 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/hfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4814 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/luksde_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2549 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/luksde_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/lvm_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8162 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/lvm_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6462 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/lvm_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9765 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/ntfs_attibute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4168 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/ntfs_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/ntfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27468 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/ntfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4115 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/ntfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/os_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9917 2023-01-01 18:32:24.000000 dfvfs-20230507/tests/vfs/os_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6171 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/os_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2628 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/sqlite_blob_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5588 2022-12-29 15:59:14.000000 dfvfs-20230507/tests/vfs/sqlite_blob_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/sqlite_blob_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1766 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/tar_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8767 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/tar_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5544 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/tar_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/tsk_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/tsk_data_stream.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1893 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/tsk_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95551 2023-05-03 15:36:29.000000 dfvfs-20230507/tests/vfs/tsk_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3941 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/tsk_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1904 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/tsk_partition_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22354 2023-05-03 04:30:43.000000 dfvfs-20230507/tests/vfs/tsk_partition_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6657 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/tsk_partition_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/vshadow_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8488 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/vshadow_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6413 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/vshadow_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2228 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/xfs_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2112 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/xfs_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13190 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/xfs_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3985 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/xfs_file_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1763 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/zip_directory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13454 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/vfs/zip_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5641 2022-12-23 11:39:29.000000 dfvfs-20230507/tests/vfs/zip_file_system.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.364402 dfvfs-20230507/tests/volume/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:14:18.000000 dfvfs-20230507/tests/volume/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2698 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/volume/apfs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2023-05-07 07:19:13.000000 dfvfs-20230507/tests/volume/apm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2088 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/volume/cs_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/volume/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/volume/gpt_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3695 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/volume/lvm_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8084 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/volume/tsk_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3543 2022-12-29 15:59:15.000000 dfvfs-20230507/tests/volume/vshadow_volume_system.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-05-06 09:14:08.000000 dfvfs-20230507/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-07 16:50:11.401402 dfvfs-20230507/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-11-21 19:17:55.000000 dfvfs-20230507/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-06 09:14:08.000000 dfvfs-20230507/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-06 09:14:08.000000 dfvfs-20230507/utils/dependencies.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     2366 2023-05-01 03:33:58.000000 dfvfs-20230507/utils/generate_test_data_bsd.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    14027 2023-05-01 03:33:58.000000 dfvfs-20230507/utils/generate_test_data_linux.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4844 2023-05-01 03:33:58.000000 dfvfs-20230507/utils/generate_test_data_macos.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14212 2022-12-29 15:59:15.000000 dfvfs-20230507/utils/generate_test_data_windows.bat
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      815 2022-11-21 19:17:55.000000 dfvfs-20230507/utils/update_release.sh
```

### Comparing `dfvfs-20230408/.github/workflows/test_docker.yml` & `dfvfs-20230507/.github/workflows/test_docker.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 on: [push]
 permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['37']
+        version: ['38']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
-        dnf install -y @development-tools python3 python3-devel libbde-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi python3-cryptography python3-dfdatetime python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-pyyaml python3-setuptools
+        dnf install -y @development-tools python3 python3-devel libbde-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi python3-cryptography python3-dfdatetime python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-pyyaml python3-setuptools
     - name: Run tests
       env:
         LANG: C.utf8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       run: |
@@ -41,28 +41,28 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         version: ['22.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
         ln -f -s /usr/share/zoneinfo/UTC /etc/localtime
     - name: Install dependencies
       run: |
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential python3 python3-dev libbde-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi-backend python3-cryptography python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
+        apt-get install -y build-essential python3 python3-dev libbde-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi-backend python3-cryptography python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       env:
```

### Comparing `dfvfs-20230408/.github/workflows/test_docs.yml` & `dfvfs-20230507/.github/workflows/test_docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       matrix:
         include:
         - python-version: '3.8'
           toxenv: 'docs'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -32,15 +32,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi-backend python3-cryptography python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
+        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-cffi-backend python3-cryptography python3-dfdatetime python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `dfvfs-20230408/.pylintrc` & `dfvfs-20230507/.pylintrc`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/ACKNOWLEDGEMENTS` & `dfvfs-20230507/ACKNOWLEDGEMENTS`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/LICENSE` & `dfvfs-20230507/LICENSE`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/MANIFEST.in` & `dfvfs-20230507/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/MANIFEST.test_data.in` & `dfvfs-20230507/MANIFEST.test_data.in`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/PKG-INFO` & `dfvfs-20230507/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfvfs
-Version: 20230408
+Version: 20230507
 Summary: Digital Forensics Virtual File System (dfVFS).
 Home-page: https://github.com/log2timeline/dfvfs
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfvfs-20230408/appveyor.yml` & `dfvfs-20230507/appveyor.yml`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/config/appveyor/install.ps1` & `dfvfs-20230507/config/appveyor/install.ps1`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Script to set up tests on AppVeyor Windows.
 
-$Dependencies = "PyYAML cffi cryptography dfdatetime dtfabric idna libbde libewf libfsapfs libfsext libfsfat libfshfs libfsntfs libfsxfs libfvde libfwnt libluksde libmodi libphdi libqcow libsigscan libsmdev libsmraw libvhdi libvmdk libvsgpt libvshadow libvslvm pytsk3 xattr"
-$Dependencies = ${Dependencies} -split " "
+$Dependencies = "PyYAML cffi cryptography dfdatetime dtfabric idna libbde libewf libfsapfs libfsext libfsfat libfshfs libfsntfs libfsxfs libfvde libfwnt libluksde libmodi libphdi libqcow libsigscan libsmdev libsmraw libvhdi libvmdk libvsapm libvsgpt libvshadow libvslvm pytsk3 xattr"
 
-$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1"
-Write-Host (${Output} | Out-String)
-
-If ($env:APPVEYOR_REPO_BRANCH -eq "main")
-{
-	$Track = "stable"
-}
-Else
+If ($Dependencies.Length -gt 0)
 {
-	$Track = $env:APPVEYOR_REPO_BRANCH
-}
-New-Item -ItemType "directory" -Name "dependencies"
+	$Dependencies = ${Dependencies} -split " "
 
-$env:PYTHONPATH = "..\l2tdevtools"
+	$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
 
-$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1"
-Write-Host (${Output} | Out-String)
+	If ($env:APPVEYOR_REPO_BRANCH -eq "main")
+	{
+		$Track = "stable"
+	}
+	Else
+	{
+		$Track = $env:APPVEYOR_REPO_BRANCH
+	}
+	New-Item -ItemType "directory" -Name "dependencies"
+
+	$env:PYTHONPATH = "..\l2tdevtools"
+
+	$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
+}
```

### Comparing `dfvfs-20230408/config/appveyor/runtests.sh` & `dfvfs-20230507/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/config/dpkg/control` & `dfvfs-20230507/config/dpkg/control`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 Build-Depends: debhelper (>= 9), dh-python, python3-all (>= 3.6~), python3-setuptools
 Standards-Version: 4.1.4
 X-Python3-Version: >= 3.6
 Homepage: https://github.com/log2timeline/dfvfs
 
 Package: python3-dfvfs
 Architecture: all
-Depends: libbde-python3 (>= 20220121), libewf-python3 (>= 20131210), libfsapfs-python3 (>= 20220709), libfsext-python3 (>= 20220829), libfsfat-python3 (>= 20220925), libfshfs-python3 (>= 20220831), libfsntfs-python3 (>= 20211229), libfsxfs-python3 (>= 20220829), libfvde-python3 (>= 20220121), libfwnt-python3 (>= 20210717), libluksde-python3 (>= 20220121), libmodi-python3 (>= 20210405), libphdi-python3 (>= 20220228), libqcow-python3 (>= 20201213), libsigscan-python3 (>= 20191221), libsmdev-python3 (>= 20140529), libsmraw-python3 (>= 20140612), libvhdi-python3 (>= 20201014), libvmdk-python3 (>= 20140421), libvsgpt-python3 (>= 20211115), libvshadow-python3 (>= 20160109), libvslvm-python3 (>= 20160109), python3-cffi-backend (>= 1.9.1), python3-cryptography (>= 2.0.2), python3-dfdatetime (>= 20221112), python3-dtfabric (>= 20220219), python3-idna (>= 2.5), python3-pytsk3 (>= 20210419), python3-pyxattr (>= 0.7.2), python3-yaml (>= 3.10), ${misc:Depends}
+Depends: libbde-python3 (>= 20220121), libewf-python3 (>= 20131210), libfsapfs-python3 (>= 20220709), libfsext-python3 (>= 20220829), libfsfat-python3 (>= 20220925), libfshfs-python3 (>= 20220831), libfsntfs-python3 (>= 20211229), libfsxfs-python3 (>= 20220829), libfvde-python3 (>= 20220121), libfwnt-python3 (>= 20210717), libluksde-python3 (>= 20220121), libmodi-python3 (>= 20210405), libphdi-python3 (>= 20220228), libqcow-python3 (>= 20201213), libsigscan-python3 (>= 20191221), libsmdev-python3 (>= 20140529), libsmraw-python3 (>= 20140612), libvhdi-python3 (>= 20201014), libvmdk-python3 (>= 20140421), libvsapm-python3 (>= 20230506), libvsgpt-python3 (>= 20211115), libvshadow-python3 (>= 20160109), libvslvm-python3 (>= 20160109), python3-cffi-backend (>= 1.9.1), python3-cryptography (>= 2.0.2), python3-dfdatetime (>= 20221112), python3-dtfabric (>= 20220219), python3-idna (>= 2.5), python3-pytsk3 (>= 20210419), python3-pyxattr (>= 0.7.2), python3-yaml (>= 3.10), ${misc:Depends}
 Description: Python 3 module of dfVFS
  dfVFS, or Digital Forensics Virtual File System, provides read-only access to
  file-system objects from various storage media types and file formats. The goal
  of dfVFS is to provide a generic interface for accessing file-system objects,
  for which it uses several back-ends that provide the actual implementation of
  the various storage media types, volume systems and file systems.
```

### Comparing `dfvfs-20230408/config/dpkg/copyright` & `dfvfs-20230507/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/config/pylint/spelling-private-dict` & `dfvfs-20230507/config/pylint/spelling-private-dict`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dependencies.ini` & `dfvfs-20230507/dependencies.ini`

 * *Files 3% similar despite different names*

```diff
@@ -185,14 +185,22 @@
 dpkg_name: libvmdk-python3
 l2tbinaries_name: libvmdk
 minimum_version: 20140421
 pypi_name: libvmdk-python
 rpm_name: libvmdk-python3
 version_property: get_version()
 
+[pyvsapm]
+dpkg_name: libvsapm-python3
+l2tbinaries_name: libvsapm
+minimum_version: 20230506
+pypi_name: libvsapm-python
+rpm_name: libvsapm-python3
+version_property: get_version()
+
 [pyvsgpt]
 dpkg_name: libvsgpt-python3
 l2tbinaries_name: libvsgpt
 minimum_version: 20211115
 pypi_name: libvsgpt-python
 rpm_name: libvsgpt-python3
 version_property: get_version()
```

### Comparing `dfvfs-20230408/dfvfs/analyzer/__init__.py` & `dfvfs-20230507/dfvfs/analyzer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """Imports for the format analyzer."""
 
 from dfvfs.analyzer import apfs_analyzer_helper
 from dfvfs.analyzer import apfs_container_analyzer_helper
+from dfvfs.analyzer import apm_analyzer_helper
 from dfvfs.analyzer import bde_analyzer_helper
 from dfvfs.analyzer import bzip2_analyzer_helper
 from dfvfs.analyzer import cpio_analyzer_helper
 from dfvfs.analyzer import cs_analyzer_helper
 from dfvfs.analyzer import ewf_analyzer_helper
 from dfvfs.analyzer import ext_analyzer_helper
 from dfvfs.analyzer import fat_analyzer_helper
```

### Comparing `dfvfs-20230408/dfvfs/analyzer/analyzer.py` & `dfvfs-20230507/dfvfs/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/apfs_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/apfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/apfs_container_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/apfs_container_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/bde_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/bde_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/bzip2_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/bzip2_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/cpio_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/cpio_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/cs_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/cs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/ewf_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/ewf_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/ext_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/ext_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/fat_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/fat_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/gpt_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/gpt_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/gzip_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/gzip_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/hfs_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/hfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/luksde_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/luksde_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/lvm_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/lvm_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/modi_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/modi_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/ntfs_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/ntfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/phdi_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/phdi_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/qcow_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/qcow_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/specification.py` & `dfvfs-20230507/dfvfs/analyzer/specification.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/tar_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/tar_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/tsk_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/tsk_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/tsk_partition_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/tsk_partition_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/vhdi_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/vhdi_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/vmdk_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/vmdk_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/vshadow_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/vshadow_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/xfs_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/xfs_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/xz_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/xz_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/analyzer/zip_analyzer_helper.py` & `dfvfs-20230507/dfvfs/analyzer/zip_analyzer_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/compression/bzip2_decompressor.py` & `dfvfs-20230507/dfvfs/compression/bzip2_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/compression/manager.py` & `dfvfs-20230507/dfvfs/compression/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/compression/xz_decompressor.py` & `dfvfs-20230507/dfvfs/compression/xz_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/compression/zlib_decompressor.py` & `dfvfs-20230507/dfvfs/compression/zlib_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/credentials/apfs_credentials.py` & `dfvfs-20230507/dfvfs/credentials/apfs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/credentials/bde_credentials.py` & `dfvfs-20230507/dfvfs/credentials/bde_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/credentials/credentials.py` & `dfvfs-20230507/dfvfs/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/credentials/cs_credentials.py` & `dfvfs-20230507/dfvfs/credentials/cs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/credentials/keychain.py` & `dfvfs-20230507/dfvfs/credentials/keychain.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/credentials/manager.py` & `dfvfs-20230507/dfvfs/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encoding/base16_decoder.py` & `dfvfs-20230507/dfvfs/encoding/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encoding/base32_decoder.py` & `dfvfs-20230507/dfvfs/encoding/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encoding/base64_decoder.py` & `dfvfs-20230507/dfvfs/encoding/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encoding/manager.py` & `dfvfs-20230507/dfvfs/encoding/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encryption/aes_decrypter.py` & `dfvfs-20230507/dfvfs/encryption/aes_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encryption/blowfish_decrypter.py` & `dfvfs-20230507/dfvfs/encryption/blowfish_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encryption/decrypter.py` & `dfvfs-20230507/dfvfs/encryption/decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encryption/des3_decrypter.py` & `dfvfs-20230507/dfvfs/encryption/des3_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encryption/manager.py` & `dfvfs-20230507/dfvfs/encryption/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/encryption/rc4_decrypter.py` & `dfvfs-20230507/dfvfs/encryption/rc4_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/apfs_file_io.py` & `dfvfs-20230507/dfvfs/file_io/apfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/bde_file_io.py` & `dfvfs-20230507/dfvfs/file_io/bde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/compressed_stream_io.py` & `dfvfs-20230507/dfvfs/file_io/compressed_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/cpio_file_io.py` & `dfvfs-20230507/dfvfs/file_io/cpio_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/cs_file_io.py` & `dfvfs-20230507/dfvfs/file_io/cs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/data_range_io.py` & `dfvfs-20230507/dfvfs/file_io/data_range_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/encoded_stream_io.py` & `dfvfs-20230507/dfvfs/file_io/encoded_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/encrypted_stream_io.py` & `dfvfs-20230507/dfvfs/file_io/encrypted_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/ewf_file_io.py` & `dfvfs-20230507/dfvfs/file_io/ewf_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/ext_file_io.py` & `dfvfs-20230507/dfvfs/file_io/ext_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/fake_file_io.py` & `dfvfs-20230507/dfvfs/file_io/fake_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/fat_file_io.py` & `dfvfs-20230507/dfvfs/file_io/fat_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/file_io.py` & `dfvfs-20230507/dfvfs/file_io/file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/file_object_io.py` & `dfvfs-20230507/dfvfs/file_io/file_object_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/gpt_file_io.py` & `dfvfs-20230507/dfvfs/file_io/gpt_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/gzip_file_io.py` & `dfvfs-20230507/dfvfs/file_io/gzip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/hfs_file_io.py` & `dfvfs-20230507/dfvfs/file_io/hfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/luksde_file_io.py` & `dfvfs-20230507/dfvfs/file_io/luksde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/lvm_file_io.py` & `dfvfs-20230507/dfvfs/file_io/lvm_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/modi_file_io.py` & `dfvfs-20230507/dfvfs/file_io/modi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/ntfs_file_io.py` & `dfvfs-20230507/dfvfs/file_io/ntfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/os_file_io.py` & `dfvfs-20230507/dfvfs/file_io/os_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/phdi_file_io.py` & `dfvfs-20230507/dfvfs/file_io/phdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/qcow_file_io.py` & `dfvfs-20230507/dfvfs/file_io/qcow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/raw_file_io.py` & `dfvfs-20230507/dfvfs/file_io/raw_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/sqlite_blob_file_io.py` & `dfvfs-20230507/dfvfs/file_io/sqlite_blob_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/tar_file_io.py` & `dfvfs-20230507/dfvfs/file_io/tar_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/tsk_file_io.py` & `dfvfs-20230507/dfvfs/file_io/tsk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/tsk_partition_file_io.py` & `dfvfs-20230507/dfvfs/file_io/tsk_partition_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/vhdi_file_io.py` & `dfvfs-20230507/dfvfs/file_io/vhdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/vmdk_file_io.py` & `dfvfs-20230507/dfvfs/file_io/vmdk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/vshadow_file_io.py` & `dfvfs-20230507/dfvfs/file_io/vshadow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/xfs_file_io.py` & `dfvfs-20230507/dfvfs/file_io/xfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/file_io/zip_file_io.py` & `dfvfs-20230507/dfvfs/file_io/zip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/helpers/command_line.py` & `dfvfs-20230507/dfvfs/helpers/command_line.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/helpers/data_slice.py` & `dfvfs-20230507/dfvfs/helpers/data_slice.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/helpers/fake_file_system_builder.py` & `dfvfs-20230507/dfvfs/helpers/fake_file_system_builder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/helpers/file_system_searcher.py` & `dfvfs-20230507/dfvfs/helpers/file_system_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,26 +542,25 @@
       if (not has_location or location_match) and not at_last_location_segment:
         sub_find_specs.append(find_spec)
 
     if sub_find_specs:
       segment_index += 1
       try:
         for sub_file_entry in file_entry.sub_file_entries:
-          for matching_path_spec in self._FindInFileEntry(
-              sub_file_entry, sub_find_specs, segment_index):
-            yield matching_path_spec
+          yield from self._FindInFileEntry(
+              sub_file_entry, sub_find_specs, segment_index)
 
       except errors.AccessError:
         pass
 
   def Find(self, find_specs=None):
     """Searches for matching file entries within the file system.
 
     Args:
-      find_specs (list[FindSpec]): find specifications. where None
+      find_specs (Optional[list[FindSpec]]): find specifications, where None
           will return all allocated file entries.
 
     Yields:
       PathSpec: path specification of a matching file entry.
     """
     if not find_specs:
       find_specs.append(FindSpec())
@@ -570,17 +569,15 @@
         self._file_system.type_indicator):
       file_entry = self._file_system.GetFileEntryByPathSpec(self._mount_point)
     else:
       file_entry = self._file_system.GetRootFileEntry()
 
     # Note that APFS can have a volume without a root directory.
     if file_entry:
-      for matching_path_spec in self._FindInFileEntry(
-          file_entry, find_specs, 0):
-        yield matching_path_spec
+      yield from self._FindInFileEntry(file_entry, find_specs, 0)
 
   def GetFileEntryByPathSpec(self, path_spec):
     """Retrieves a file entry for a path specification.
 
     Args:
       path_spec (PathSpec): path specification.
```

### Comparing `dfvfs-20230408/dfvfs/helpers/source_scanner.py` & `dfvfs-20230507/dfvfs/helpers/source_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/helpers/text_file.py` & `dfvfs-20230507/dfvfs/helpers/text_file.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/helpers/volume_scanner.py` & `dfvfs-20230507/dfvfs/helpers/volume_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/helpers/windows_path_resolver.py` & `dfvfs-20230507/dfvfs/helpers/windows_path_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     if path_spec_factory.Factory.IsSystemLevelTypeIndicator(
         file_system.type_indicator):
       if not hasattr(mount_point, 'location'):
         raise errors.PathSpecError(
             'Mount point path specification missing location.')
 
     super(WindowsPathResolver, self).__init__()
-
     self._drive_letter = drive_letter
     self._environment_variables = {}
     self._file_system = file_system
     self._mount_point = mount_point
 
   # Windows paths:
   # Device path:                    \\.\PhysicalDrive0
```

### Comparing `dfvfs-20230408/dfvfs/lib/apfs_helper.py` & `dfvfs-20230507/dfvfs/lib/apfs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/bde_helper.py` & `dfvfs-20230507/dfvfs/lib/bde_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/cpio.py` & `dfvfs-20230507/dfvfs/lib/cpio.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/cpio.yaml` & `dfvfs-20230507/dfvfs/lib/cpio.yaml`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/cs_helper.py` & `dfvfs-20230507/dfvfs/lib/cs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/data_format.py` & `dfvfs-20230507/dfvfs/lib/data_format.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/decorators.py` & `dfvfs-20230507/dfvfs/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/definitions.py` & `dfvfs-20230507/dfvfs/lib/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # The extent types.
 EXTENT_TYPE_COMPRESSED = 'compressed'
 EXTENT_TYPE_DATA = 'data'
 EXTENT_TYPE_SPARSE = 'sparse'
 
 # The type indicator definitions.
 TYPE_INDICATOR_APFS = 'APFS'
+TYPE_INDICATOR_APM = 'APM'
 TYPE_INDICATOR_APFS_CONTAINER = 'APFS_CONTAINER'
 TYPE_INDICATOR_BDE = 'BDE'
 TYPE_INDICATOR_BZIP2 = 'BZIP2'
 TYPE_INDICATOR_COMPRESSED_STREAM = 'COMPRESSED_STREAM'
 TYPE_INDICATOR_CPIO = 'CPIO'
 TYPE_INDICATOR_CS = 'CS'
 TYPE_INDICATOR_DATA_RANGE = 'DATA_RANGE'
@@ -82,26 +83,28 @@
     TYPE_INDICATOR_FAT,
     TYPE_INDICATOR_HFS,
     TYPE_INDICATOR_NTFS,
     TYPE_INDICATOR_TSK,
     TYPE_INDICATOR_XFS])
 
 PARTITION_TABLE_TYPE_INDICATORS = frozenset([
+    TYPE_INDICATOR_APM,
     TYPE_INDICATOR_GPT,
     TYPE_INDICATOR_TSK_PARTITION])
 
 STORAGE_MEDIA_IMAGE_TYPE_INDICATORS = frozenset([
     TYPE_INDICATOR_EWF,
     TYPE_INDICATOR_QCOW,
     TYPE_INDICATOR_RAW,
     TYPE_INDICATOR_VHDI,
     TYPE_INDICATOR_VMDK])
 
 VOLUME_SYSTEM_TYPE_INDICATORS = frozenset([
     TYPE_INDICATOR_APFS_CONTAINER,
+    TYPE_INDICATOR_APM,
     TYPE_INDICATOR_CS,
     TYPE_INDICATOR_GPT,
     TYPE_INDICATOR_LVM,
     TYPE_INDICATOR_TSK_PARTITION,
     TYPE_INDICATOR_VSHADOW])
 
 # The preferred back-ends.
```

### Comparing `dfvfs-20230408/dfvfs/lib/errors.py` & `dfvfs-20230507/dfvfs/lib/errors.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/ewf_helper.py` & `dfvfs-20230507/dfvfs/lib/ewf_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/glob2regex.py` & `dfvfs-20230507/dfvfs/lib/glob2regex.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/gpt_helper.py` & `dfvfs-20230507/dfvfs/lib/gpt_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/gzipfile.py` & `dfvfs-20230507/dfvfs/lib/gzipfile.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/gzipfile.yaml` & `dfvfs-20230507/dfvfs/lib/gzipfile.yaml`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/luksde_helper.py` & `dfvfs-20230507/dfvfs/lib/luksde_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/lvm_helper.py` & `dfvfs-20230507/dfvfs/lib/lvm_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/raw_helper.py` & `dfvfs-20230507/dfvfs/lib/raw_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/sqlite_database.py` & `dfvfs-20230507/dfvfs/lib/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/tsk_image.py` & `dfvfs-20230507/dfvfs/lib/tsk_image.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/lib/tsk_partition.py` & `dfvfs-20230507/dfvfs/lib/tsk_partition.py`

 * *Files 10% similar despite different names*

```diff
@@ -141,14 +141,28 @@
     bool: True if the volume system part is allocated, False otherwise.
   """
   # Note that because pytsk3.TSK_VS_PART_INFO does not explicitly defines
   # flags need to check if the attribute exists.
   # The flags are an instance of TSK_VS_PART_FLAG_ENUM.
   tsk_vs_part_flags = getattr(tsk_vs_part, 'flags', None)
 
+  is_allocated = (tsk_vs_part_flags is not None and
+                  tsk_vs_part_flags == pytsk3.TSK_VS_PART_FLAG_ALLOC)
+
+  tsk_vs_vstype = getattr(tsk_vs_part.vs, 'vstype', pytsk3.TSK_VS_TYPE_UNSUPP)
+
+  # For BSD disklabel consider c and d partitions (slot 2 and 3) as metadata
+  # part of the disklabel volume itself and not a partition of the volume.
+  if tsk_vs_vstype == pytsk3.TSK_VS_TYPE_BSD:
+    tsk_vs_part_slot_num = getattr(tsk_vs_part, 'slot_num', None)
+    if tsk_vs_part_slot_num in (None, 2, 3):
+      is_allocated = False
+
   # For APM partition tables the description needs to be checked to determine
   # the usage of the part.
-  tsk_vs_part_desc = getattr(tsk_vs_part, 'desc', None)
+  elif tsk_vs_vstype == pytsk3.TSK_VS_TYPE_MAC:
+    tsk_vs_part_desc = getattr(tsk_vs_part, 'desc', None)
+
+    return is_allocated and tsk_vs_part_desc not in (
+        b'Apple_partition_map', b'Apple_Free')
 
-  return (tsk_vs_part_flags is not None and
-          tsk_vs_part_flags == pytsk3.TSK_VS_PART_FLAG_ALLOC and
-          tsk_vs_part_desc not in (b'Apple_partition_map', b'Apple_Free'))
+  return is_allocated
```

### Comparing `dfvfs-20230408/dfvfs/lib/vshadow_helper.py` & `dfvfs-20230507/dfvfs/lib/vshadow_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/mount/manager.py` & `dfvfs-20230507/dfvfs/mount/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/__init__.py` & `dfvfs-20230507/dfvfs/path/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """Imports for path specification factory."""
 
 from dfvfs.path import apfs_container_path_spec
 from dfvfs.path import apfs_path_spec
+from dfvfs.path import apm_path_spec
 from dfvfs.path import bde_path_spec
 from dfvfs.path import compressed_stream_path_spec
 from dfvfs.path import cpio_path_spec
 from dfvfs.path import cs_path_spec
 from dfvfs.path import data_range_path_spec
 from dfvfs.path import encoded_stream_path_spec
 from dfvfs.path import encrypted_stream_path_spec
```

### Comparing `dfvfs-20230408/dfvfs/path/apfs_container_path_spec.py` & `dfvfs-20230507/dfvfs/path/apfs_container_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/apfs_path_spec.py` & `dfvfs-20230507/dfvfs/path/apfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/bde_path_spec.py` & `dfvfs-20230507/dfvfs/path/bde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/compressed_stream_path_spec.py` & `dfvfs-20230507/dfvfs/path/compressed_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/cpio_path_spec.py` & `dfvfs-20230507/dfvfs/path/cpio_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/cs_path_spec.py` & `dfvfs-20230507/dfvfs/path/cs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/data_range_path_spec.py` & `dfvfs-20230507/dfvfs/path/data_range_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/encoded_stream_path_spec.py` & `dfvfs-20230507/dfvfs/path/encoded_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/encrypted_stream_path_spec.py` & `dfvfs-20230507/dfvfs/path/encrypted_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/ewf_path_spec.py` & `dfvfs-20230507/dfvfs/path/ewf_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/ext_path_spec.py` & `dfvfs-20230507/dfvfs/path/ext_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/factory.py` & `dfvfs-20230507/dfvfs/path/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/fake_path_spec.py` & `dfvfs-20230507/dfvfs/path/fake_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/fat_path_spec.py` & `dfvfs-20230507/dfvfs/path/fat_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/gpt_path_spec.py` & `dfvfs-20230507/dfvfs/path/gpt_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/gzip_path_spec.py` & `dfvfs-20230507/dfvfs/path/gzip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/hfs_path_spec.py` & `dfvfs-20230507/dfvfs/path/hfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/location_path_spec.py` & `dfvfs-20230507/dfvfs/path/location_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/luksde_path_spec.py` & `dfvfs-20230507/dfvfs/path/luksde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/lvm_path_spec.py` & `dfvfs-20230507/dfvfs/path/lvm_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/modi_path_spec.py` & `dfvfs-20230507/dfvfs/path/modi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/mount_path_spec.py` & `dfvfs-20230507/dfvfs/path/mount_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/ntfs_path_spec.py` & `dfvfs-20230507/dfvfs/path/ntfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/os_path_spec.py` & `dfvfs-20230507/dfvfs/path/os_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/path_spec.py` & `dfvfs-20230507/dfvfs/path/path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/phdi_path_spec.py` & `dfvfs-20230507/dfvfs/path/phdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/qcow_path_spec.py` & `dfvfs-20230507/dfvfs/path/qcow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/raw_path_spec.py` & `dfvfs-20230507/dfvfs/path/raw_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/sqlite_blob_path_spec.py` & `dfvfs-20230507/dfvfs/path/sqlite_blob_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/tar_path_spec.py` & `dfvfs-20230507/dfvfs/path/tar_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/tsk_partition_path_spec.py` & `dfvfs-20230507/dfvfs/path/tsk_partition_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/tsk_path_spec.py` & `dfvfs-20230507/dfvfs/path/tsk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/vhdi_path_spec.py` & `dfvfs-20230507/dfvfs/path/vhdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/vmdk_path_spec.py` & `dfvfs-20230507/dfvfs/path/vmdk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/vshadow_path_spec.py` & `dfvfs-20230507/dfvfs/path/vshadow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/xfs_path_spec.py` & `dfvfs-20230507/dfvfs/path/xfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/path/zip_path_spec.py` & `dfvfs-20230507/dfvfs/path/zip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver/context.py` & `dfvfs-20230507/dfvfs/resolver/context.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver/resolver.py` & `dfvfs-20230507/dfvfs/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/__init__.py` & `dfvfs-20230507/dfvfs/resolver_helpers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 try:
   from dfvfs.resolver_helpers import apfs_container_resolver_helper
   from dfvfs.resolver_helpers import apfs_resolver_helper
 except ImportError:
   pass
 
 try:
+  from dfvfs.resolver_helpers import apm_resolver_helper
+except ImportError:
+  pass
+
+try:
   from dfvfs.resolver_helpers import bde_resolver_helper
 except ImportError:
   pass
 
 from dfvfs.resolver_helpers import compressed_stream_resolver_helper
 from dfvfs.resolver_helpers import cpio_resolver_helper
```

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/apfs_container_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/apfs_container_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/apfs_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/apfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/bde_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/bde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/compressed_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/cpio_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/cpio_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/cs_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/cs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/data_range_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/data_range_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/encoded_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/ewf_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/ewf_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/ext_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/ext_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/fake_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/fake_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/fat_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/fat_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/gpt_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/gpt_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/gzip_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/gzip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/hfs_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/hfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/luksde_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/luksde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/lvm_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/lvm_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/manager.py` & `dfvfs-20230507/dfvfs/resolver_helpers/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/modi_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/modi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/ntfs_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/ntfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/os_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/os_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/phdi_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/phdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/qcow_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/qcow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/raw_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/raw_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/sqlite_blob_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/tar_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/tar_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/tsk_partition_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/tsk_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/tsk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/vhdi_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/vhdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/vmdk_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/vmdk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/vshadow_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/vshadow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/xfs_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/xfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/resolver_helpers/zip_resolver_helper.py` & `dfvfs-20230507/dfvfs/resolver_helpers/zip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/serializer/json_serializer.py` & `dfvfs-20230507/dfvfs/serializer/json_serializer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/serializer/serializer.py` & `dfvfs-20230507/dfvfs/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/apfs_attribute.py` & `dfvfs-20230507/dfvfs/vfs/apfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/apfs_container_directory.py` & `dfvfs-20230507/dfvfs/vfs/apfs_container_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/apfs_container_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/apfs_container_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/apfs_container_file_system.py` & `dfvfs-20230507/dfvfs/vfs/apfs_container_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/apfs_directory.py` & `dfvfs-20230507/dfvfs/vfs/apfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/apfs_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/apfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/apfs_file_system.py` & `dfvfs-20230507/dfvfs/vfs/apfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/attribute.py` & `dfvfs-20230507/dfvfs/vfs/attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/bde_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/bde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/bde_file_system.py` & `dfvfs-20230507/dfvfs/vfs/bde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/compressed_stream_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/compressed_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/compressed_stream_file_system.py` & `dfvfs-20230507/dfvfs/vfs/compressed_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/cpio_directory.py` & `dfvfs-20230507/dfvfs/vfs/cpio_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/cpio_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/cpio_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/cpio_file_system.py` & `dfvfs-20230507/dfvfs/vfs/cpio_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/cs_directory.py` & `dfvfs-20230507/dfvfs/vfs/cs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/cs_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/cs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/cs_file_system.py` & `dfvfs-20230507/dfvfs/vfs/cs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/data_range_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/data_range_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/data_range_file_system.py` & `dfvfs-20230507/dfvfs/vfs/data_range_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/data_stream.py` & `dfvfs-20230507/dfvfs/vfs/data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/directory.py` & `dfvfs-20230507/dfvfs/vfs/directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/encoded_stream_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/encoded_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/encoded_stream_file_system.py` & `dfvfs-20230507/dfvfs/vfs/encoded_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/encrypted_stream_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/encrypted_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/encrypted_stream_file_system.py` & `dfvfs-20230507/dfvfs/vfs/encrypted_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/ext_attribute.py` & `dfvfs-20230507/dfvfs/vfs/ext_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/ext_directory.py` & `dfvfs-20230507/dfvfs/vfs/ext_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/ext_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/ext_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/ext_file_system.py` & `dfvfs-20230507/dfvfs/vfs/ext_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/extent.py` & `dfvfs-20230507/dfvfs/vfs/extent.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/fake_directory.py` & `dfvfs-20230507/dfvfs/vfs/fake_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/fake_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/fake_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/fake_file_system.py` & `dfvfs-20230507/dfvfs/vfs/fake_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/fat_directory.py` & `dfvfs-20230507/dfvfs/vfs/fat_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/fat_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/fat_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/fat_file_system.py` & `dfvfs-20230507/dfvfs/vfs/fat_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/file_entry.py` & `dfvfs-20230507/dfvfs/vfs/file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/file_system.py` & `dfvfs-20230507/dfvfs/vfs/file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/gpt_directory.py` & `dfvfs-20230507/dfvfs/vfs/gpt_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/gpt_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/gpt_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/gpt_file_system.py` & `dfvfs-20230507/dfvfs/vfs/gpt_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/gzip_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/gzip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/gzip_file_system.py` & `dfvfs-20230507/dfvfs/vfs/gzip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/hfs_attribute.py` & `dfvfs-20230507/dfvfs/vfs/hfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/hfs_data_stream.py` & `dfvfs-20230507/dfvfs/vfs/hfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/hfs_directory.py` & `dfvfs-20230507/dfvfs/vfs/hfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/hfs_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/hfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/hfs_file_system.py` & `dfvfs-20230507/dfvfs/vfs/hfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/luksde_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/luksde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/luksde_file_system.py` & `dfvfs-20230507/dfvfs/vfs/luksde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/lvm_directory.py` & `dfvfs-20230507/dfvfs/vfs/lvm_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/lvm_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/lvm_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/lvm_file_system.py` & `dfvfs-20230507/dfvfs/vfs/lvm_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/ntfs_attribute.py` & `dfvfs-20230507/dfvfs/vfs/ntfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/ntfs_data_stream.py` & `dfvfs-20230507/dfvfs/vfs/ntfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/ntfs_directory.py` & `dfvfs-20230507/dfvfs/vfs/ntfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/ntfs_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/ntfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/ntfs_file_system.py` & `dfvfs-20230507/dfvfs/vfs/ntfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/os_attribute.py` & `dfvfs-20230507/dfvfs/vfs/os_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/os_directory.py` & `dfvfs-20230507/dfvfs/vfs/os_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/os_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/os_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/os_file_system.py` & `dfvfs-20230507/dfvfs/vfs/os_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/root_only_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/root_only_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/root_only_file_system.py` & `dfvfs-20230507/dfvfs/vfs/root_only_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/sqlite_blob_directory.py` & `dfvfs-20230507/dfvfs/vfs/sqlite_blob_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/sqlite_blob_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/sqlite_blob_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/sqlite_blob_file_system.py` & `dfvfs-20230507/dfvfs/vfs/sqlite_blob_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tar_directory.py` & `dfvfs-20230507/dfvfs/vfs/tar_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tar_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/tar_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tar_file_system.py` & `dfvfs-20230507/dfvfs/vfs/tar_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tsk_attribute.py` & `dfvfs-20230507/dfvfs/vfs/tsk_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tsk_data_stream.py` & `dfvfs-20230507/dfvfs/vfs/tsk_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tsk_directory.py` & `dfvfs-20230507/dfvfs/vfs/tsk_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tsk_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/tsk_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tsk_file_system.py` & `dfvfs-20230507/dfvfs/vfs/tsk_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tsk_partition_directory.py` & `dfvfs-20230507/dfvfs/vfs/tsk_partition_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tsk_partition_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/tsk_partition_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/tsk_partition_file_system.py` & `dfvfs-20230507/dfvfs/vfs/tsk_partition_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/vshadow_directory.py` & `dfvfs-20230507/dfvfs/vfs/vshadow_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/vshadow_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/vshadow_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/vshadow_file_system.py` & `dfvfs-20230507/dfvfs/vfs/vshadow_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/xfs_attribute.py` & `dfvfs-20230507/dfvfs/vfs/xfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/xfs_directory.py` & `dfvfs-20230507/dfvfs/vfs/xfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/xfs_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/xfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/xfs_file_system.py` & `dfvfs-20230507/dfvfs/vfs/xfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/zip_directory.py` & `dfvfs-20230507/dfvfs/vfs/zip_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/zip_file_entry.py` & `dfvfs-20230507/dfvfs/vfs/zip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/vfs/zip_file_system.py` & `dfvfs-20230507/dfvfs/vfs/zip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/volume/apfs_volume_system.py` & `dfvfs-20230507/dfvfs/volume/apfs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/volume/cs_volume_system.py` & `dfvfs-20230507/dfvfs/volume/cs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/volume/factory.py` & `dfvfs-20230507/dfvfs/volume/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/volume/gpt_volume_system.py` & `dfvfs-20230507/dfvfs/volume/gpt_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/volume/lvm_volume_system.py` & `dfvfs-20230507/dfvfs/volume/lvm_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/volume/tsk_volume_system.py` & `dfvfs-20230507/dfvfs/volume/tsk_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/volume/volume_system.py` & `dfvfs-20230507/dfvfs/volume/volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs/volume/vshadow_volume_system.py` & `dfvfs-20230507/dfvfs/volume/vshadow_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/dfvfs.egg-info/PKG-INFO` & `dfvfs-20230507/dfvfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfvfs
-Version: 20230408
+Version: 20230507
 Summary: Digital Forensics Virtual File System (dfVFS).
 Home-page: https://github.com/log2timeline/dfvfs
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfvfs-20230408/dfvfs.egg-info/SOURCES.txt` & `dfvfs-20230507/dfvfs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 dfvfs.egg-info/requires.txt
 dfvfs.egg-info/top_level.txt
 dfvfs/analyzer/__init__.py
 dfvfs/analyzer/analyzer.py
 dfvfs/analyzer/analyzer_helper.py
 dfvfs/analyzer/apfs_analyzer_helper.py
 dfvfs/analyzer/apfs_container_analyzer_helper.py
+dfvfs/analyzer/apm_analyzer_helper.py
 dfvfs/analyzer/bde_analyzer_helper.py
 dfvfs/analyzer/bzip2_analyzer_helper.py
 dfvfs/analyzer/cpio_analyzer_helper.py
 dfvfs/analyzer/cs_analyzer_helper.py
 dfvfs/analyzer/ewf_analyzer_helper.py
 dfvfs/analyzer/ext_analyzer_helper.py
 dfvfs/analyzer/fat_analyzer_helper.py
@@ -94,14 +95,15 @@
 dfvfs/encryption/blowfish_decrypter.py
 dfvfs/encryption/decrypter.py
 dfvfs/encryption/des3_decrypter.py
 dfvfs/encryption/manager.py
 dfvfs/encryption/rc4_decrypter.py
 dfvfs/file_io/__init__.py
 dfvfs/file_io/apfs_file_io.py
+dfvfs/file_io/apm_file_io.py
 dfvfs/file_io/bde_file_io.py
 dfvfs/file_io/compressed_stream_io.py
 dfvfs/file_io/cpio_file_io.py
 dfvfs/file_io/cs_file_io.py
 dfvfs/file_io/data_range_io.py
 dfvfs/file_io/encoded_stream_io.py
 dfvfs/file_io/encrypted_stream_io.py
@@ -138,14 +140,15 @@
 dfvfs/helpers/file_system_searcher.py
 dfvfs/helpers/source_scanner.py
 dfvfs/helpers/text_file.py
 dfvfs/helpers/volume_scanner.py
 dfvfs/helpers/windows_path_resolver.py
 dfvfs/lib/__init__.py
 dfvfs/lib/apfs_helper.py
+dfvfs/lib/apm_helper.py
 dfvfs/lib/bde_helper.py
 dfvfs/lib/cpio.py
 dfvfs/lib/cpio.yaml
 dfvfs/lib/cs_helper.py
 dfvfs/lib/data_format.py
 dfvfs/lib/decorators.py
 dfvfs/lib/definitions.py
@@ -163,14 +166,15 @@
 dfvfs/lib/tsk_partition.py
 dfvfs/lib/vshadow_helper.py
 dfvfs/mount/__init__.py
 dfvfs/mount/manager.py
 dfvfs/path/__init__.py
 dfvfs/path/apfs_container_path_spec.py
 dfvfs/path/apfs_path_spec.py
+dfvfs/path/apm_path_spec.py
 dfvfs/path/bde_path_spec.py
 dfvfs/path/compressed_stream_path_spec.py
 dfvfs/path/cpio_path_spec.py
 dfvfs/path/cs_path_spec.py
 dfvfs/path/data_range_path_spec.py
 dfvfs/path/encoded_stream_path_spec.py
 dfvfs/path/encrypted_stream_path_spec.py
@@ -204,14 +208,15 @@
 dfvfs/path/zip_path_spec.py
 dfvfs/resolver/__init__.py
 dfvfs/resolver/context.py
 dfvfs/resolver/resolver.py
 dfvfs/resolver_helpers/__init__.py
 dfvfs/resolver_helpers/apfs_container_resolver_helper.py
 dfvfs/resolver_helpers/apfs_resolver_helper.py
+dfvfs/resolver_helpers/apm_resolver_helper.py
 dfvfs/resolver_helpers/bde_resolver_helper.py
 dfvfs/resolver_helpers/compressed_stream_resolver_helper.py
 dfvfs/resolver_helpers/cpio_resolver_helper.py
 dfvfs/resolver_helpers/cs_resolver_helper.py
 dfvfs/resolver_helpers/data_range_resolver_helper.py
 dfvfs/resolver_helpers/encoded_stream_resolver_helper.py
 dfvfs/resolver_helpers/encrypted_stream_resolver_helper.py
@@ -248,14 +253,17 @@
 dfvfs/vfs/apfs_attribute.py
 dfvfs/vfs/apfs_container_directory.py
 dfvfs/vfs/apfs_container_file_entry.py
 dfvfs/vfs/apfs_container_file_system.py
 dfvfs/vfs/apfs_directory.py
 dfvfs/vfs/apfs_file_entry.py
 dfvfs/vfs/apfs_file_system.py
+dfvfs/vfs/apm_directory.py
+dfvfs/vfs/apm_file_entry.py
+dfvfs/vfs/apm_file_system.py
 dfvfs/vfs/attribute.py
 dfvfs/vfs/bde_file_entry.py
 dfvfs/vfs/bde_file_system.py
 dfvfs/vfs/compressed_stream_file_entry.py
 dfvfs/vfs/compressed_stream_file_system.py
 dfvfs/vfs/cpio_directory.py
 dfvfs/vfs/cpio_file_entry.py
@@ -332,14 +340,15 @@
 dfvfs/vfs/xfs_file_entry.py
 dfvfs/vfs/xfs_file_system.py
 dfvfs/vfs/zip_directory.py
 dfvfs/vfs/zip_file_entry.py
 dfvfs/vfs/zip_file_system.py
 dfvfs/volume/__init__.py
 dfvfs/volume/apfs_volume_system.py
+dfvfs/volume/apm_volume_system.py
 dfvfs/volume/cs_volume_system.py
 dfvfs/volume/factory.py
 dfvfs/volume/gpt_volume_system.py
 dfvfs/volume/lvm_volume_system.py
 dfvfs/volume/tsk_volume_system.py
 dfvfs/volume/volume_system.py
 dfvfs/volume/vshadow_volume_system.py
@@ -405,14 +414,15 @@
 tests/encryption/decrypter.py
 tests/encryption/des3_decrypter.py
 tests/encryption/manager.py
 tests/encryption/rc4_decrypter.py
 tests/encryption/test_lib.py
 tests/file_io/__init__.py
 tests/file_io/apfs_file_io.py
+tests/file_io/apm_file_io.py
 tests/file_io/bde_file_io.py
 tests/file_io/compressed_stream_io.py
 tests/file_io/cpio_file_io.py
 tests/file_io/cs_file_io.py
 tests/file_io/data_range_io.py
 tests/file_io/encoded_stream_io.py
 tests/file_io/encrypted_stream_io.py
@@ -460,14 +470,15 @@
 tests/lib/lvm_helper.py
 tests/lib/raw_helper.py
 tests/mount/__init__.py
 tests/mount/manager.py
 tests/path/__init__.py
 tests/path/apfs_container_path_spec.py
 tests/path/apfs_path_spec.py
+tests/path/apm_path_spec.py
 tests/path/bde_path_spec.py
 tests/path/compressed_stream_path_spec.py
 tests/path/cpio_path_spec.py
 tests/path/cs_path_spec.py
 tests/path/data_range_path_spec.py
 tests/path/encoded_stream_path_spec.py
 tests/path/encryption_stream_path_spec.py
@@ -498,14 +509,15 @@
 tests/path/vmdk_path_spec.py
 tests/path/vshadow_path_spec.py
 tests/path/xfs_path_spec.py
 tests/path/zip_path_spec.py
 tests/resolver/context.py
 tests/resolver_helpers/__init__.py
 tests/resolver_helpers/apfs_resolver_helper.py
+tests/resolver_helpers/apm_resolver_helper.py
 tests/resolver_helpers/bde_resolver_helper.py
 tests/resolver_helpers/compressed_stream_resolver_helper.py
 tests/resolver_helpers/cpio_resolver_helper.py
 tests/resolver_helpers/cs_resolver_helper.py
 tests/resolver_helpers/encoded_stream_resolver_helper.py
 tests/resolver_helpers/encrypted_stream_resolver_helper.py
 tests/resolver_helpers/ewf_resolver_helper.py
@@ -539,14 +551,17 @@
 tests/vfs/apfs_attribute.py
 tests/vfs/apfs_container_directory.py
 tests/vfs/apfs_container_file_entry.py
 tests/vfs/apfs_container_file_system.py
 tests/vfs/apfs_directory.py
 tests/vfs/apfs_file_entry.py
 tests/vfs/apfs_file_system.py
+tests/vfs/apm_directory.py
+tests/vfs/apm_file_entry.py
+tests/vfs/apm_file_system.py
 tests/vfs/attribute.py
 tests/vfs/bde_file_entry.py
 tests/vfs/bde_file_system.py
 tests/vfs/compressed_stream_file_entry.py
 tests/vfs/compressed_stream_file_system.py
 tests/vfs/cpio_directory.py
 tests/vfs/cpio_file_entry.py
@@ -619,20 +634,22 @@
 tests/vfs/xfs_file_entry.py
 tests/vfs/xfs_file_system.py
 tests/vfs/zip_directory.py
 tests/vfs/zip_file_entry.py
 tests/vfs/zip_file_system.py
 tests/volume/__init__.py
 tests/volume/apfs_volume_system.py
+tests/volume/apm_volume_system.py
 tests/volume/cs_volume_system.py
 tests/volume/factory.py
 tests/volume/gpt_volume_system.py
 tests/volume/lvm_volume_system.py
 tests/volume/tsk_volume_system.py
 tests/volume/vshadow_volume_system.py
 utils/__init__.py
 utils/check_dependencies.py
 utils/dependencies.py
+utils/generate_test_data_bsd.sh
 utils/generate_test_data_linux.sh
 utils/generate_test_data_macos.sh
 utils/generate_test_data_windows.bat
 utils/update_release.sh
```

### Comparing `dfvfs-20230408/dfvfs.egg-info/requires.txt` & `dfvfs-20230507/dfvfs.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 libphdi-python>=20220228
 libqcow-python>=20201213
 libsigscan-python>=20191221
 libsmdev-python>=20140529
 libsmraw-python>=20140612
 libvhdi-python>=20201014
 libvmdk-python>=20140421
+libvsapm-python>=20230506
 libvsgpt-python>=20211115
 libvshadow-python>=20160109
 libvslvm-python>=20160109
 pytsk3>=20210419
 
 [:platform_system != "Windows"]
 pyxattr>=0.7.2
```

### Comparing `dfvfs-20230408/dfvfs.ini` & `dfvfs-20230507/dfvfs.ini`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/conf.py` & `dfvfs-20230507/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/index.rst` & `dfvfs-20230507/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/Code-snippets.md` & `dfvfs-20230507/docs/sources/Code-snippets.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/Path-specifications.md` & `dfvfs-20230507/docs/sources/Path-specifications.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/Supported-formats.md` & `dfvfs-20230507/docs/sources/Supported-formats.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## Supported Formats
 
-The information below is based of version 20221207
+The information below is based of version 20230503
 
 ### Storage media types
 
 * EWF (EWF-E01, EWF-Ex01, EWF-S01) (Requires: [libewf/pyewf](https://github.com/libyal/libewf))
 * Mac OS disk image (Requires: [libmodi/pymodi](https://github.com/libyal/libmodi))
   * Sparse bundle disk image
   * Sparse disk image
@@ -16,17 +16,18 @@
 * (split) Storage Media RAW (Requires: [libsmraw/pysmraw](https://github.com/libyal/libsmraw))
 * VHD and VHDX (Requires: [libvhdi/pyvhdi](https://github.com/libyal/libvhdi))
 * VMDK (Requires: [libvmdk/pyvmdk](https://github.com/libyal/libvmdk))
   * currently no differential image support
 
 ### Volume systems
 
-* Apple Partition Map (APM) (Requires: [libtsk](https://github.com/sleuthkit/sleuthkit/)/[pytsk](https://github.com/py4n6/pytsk))
+* Apple Partition Map (APM) (Requires: [libtsk](https://github.com/sleuthkit/sleuthkit/)/[pytsk](https://github.com/py4n6/pytsk) or [libvsapm/pyvsapm](https://github.com/libyal/libvsapm))
 * Apple File System (APFS) container version 2 (Requires: [libfsapfs/pyfsapfs](https://github.com/libyal/libfsapfs))
 * BitLocker Disk Encryption (BDE) (Requires: [libbde/pybde](https://github.com/libyal/libbde))
+* BSD disklabel (Requires: [libtsk](https://github.com/sleuthkit/sleuthkit/)/[pytsk](https://github.com/py4n6/pytsk))
 * Core Storage (CS) including FileVault Disk Encryption (FVDE) (or FileVault 2) (Requires: [libfvde/pyfvde](https://github.com/libyal/libfvde))
 * GPT (Requires: [libvsgpt/pyvsgpt](https://github.com/libyal/libvsgpt) or [libtsk](https://github.com/sleuthkit/sleuthkit/)/[pytsk](https://github.com/py4n6/pytsk))
 * LVM (Requires: [libvslvm/pyvslvm](https://github.com/libyal/libvslvm))
   * At the moment only single physical volume LVM support
 * Linux Unified Key Setup (LUKS) (Requires: [libluksde/pyluksde](https://github.com/libyal/libluksde))
 * MBR (Requires: [libtsk](https://github.com/sleuthkit/sleuthkit/)/[pytsk](https://github.com/py4n6/pytsk))
 * Volume Shadow Snapshots (VSS) (Requires: [libvshadow/pyvshadow](https://github.com/libyal/libvshadow))
```

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.analyzer.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.analyzer.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 -------------------------------------------------------
 
 .. automodule:: dfvfs.analyzer.apfs_container_analyzer_helper
    :members:
    :undoc-members:
    :show-inheritance:
 
+dfvfs.analyzer.apm\_analyzer\_helper module
+-------------------------------------------
+
+.. automodule:: dfvfs.analyzer.apm_analyzer_helper
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 dfvfs.analyzer.bde\_analyzer\_helper module
 -------------------------------------------
 
 .. automodule:: dfvfs.analyzer.bde_analyzer_helper
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.compression.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.compression.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.credentials.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.credentials.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.encoding.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.encoding.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.encryption.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.encryption.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.file_io.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.file_io.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 ------------------------------------
 
 .. automodule:: dfvfs.file_io.apfs_file_io
    :members:
    :undoc-members:
    :show-inheritance:
 
+dfvfs.file\_io.apm\_file\_io module
+-----------------------------------
+
+.. automodule:: dfvfs.file_io.apm_file_io
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 dfvfs.file\_io.bde\_file\_io module
 -----------------------------------
 
 .. automodule:: dfvfs.file_io.bde_file_io
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.helpers.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.helpers.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.lib.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.lib.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 -----------------------------
 
 .. automodule:: dfvfs.lib.apfs_helper
    :members:
    :undoc-members:
    :show-inheritance:
 
+dfvfs.lib.apm\_helper module
+----------------------------
+
+.. automodule:: dfvfs.lib.apm_helper
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 dfvfs.lib.bde\_helper module
 ----------------------------
 
 .. automodule:: dfvfs.lib.bde_helper
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.path.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.path.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 ----------------------------------
 
 .. automodule:: dfvfs.path.apfs_path_spec
    :members:
    :undoc-members:
    :show-inheritance:
 
+dfvfs.path.apm\_path\_spec module
+---------------------------------
+
+.. automodule:: dfvfs.path.apm_path_spec
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 dfvfs.path.bde\_path\_spec module
 ---------------------------------
 
 .. automodule:: dfvfs.path.bde_path_spec
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.resolver_helpers.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.resolver_helpers.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 -----------------------------------------------------
 
 .. automodule:: dfvfs.resolver_helpers.apfs_resolver_helper
    :members:
    :undoc-members:
    :show-inheritance:
 
+dfvfs.resolver\_helpers.apm\_resolver\_helper module
+----------------------------------------------------
+
+.. automodule:: dfvfs.resolver_helpers.apm_resolver_helper
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 dfvfs.resolver\_helpers.bde\_resolver\_helper module
 ----------------------------------------------------
 
 .. automodule:: dfvfs.resolver_helpers.bde_resolver_helper
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.serializer.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.serializer.rst`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.vfs.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.vfs.rst`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,38 @@
 -----------------------------------
 
 .. automodule:: dfvfs.vfs.apfs_file_system
    :members:
    :undoc-members:
    :show-inheritance:
 
+dfvfs.vfs.apm\_directory module
+-------------------------------
+
+.. automodule:: dfvfs.vfs.apm_directory
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+dfvfs.vfs.apm\_file\_entry module
+---------------------------------
+
+.. automodule:: dfvfs.vfs.apm_file_entry
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+dfvfs.vfs.apm\_file\_system module
+----------------------------------
+
+.. automodule:: dfvfs.vfs.apm_file_system
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 dfvfs.vfs.attribute module
 --------------------------
 
 .. automodule:: dfvfs.vfs.attribute
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `dfvfs-20230408/docs/sources/api/dfvfs.volume.rst` & `dfvfs-20230507/docs/sources/api/dfvfs.volume.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 ----------------------------------------
 
 .. automodule:: dfvfs.volume.apfs_volume_system
    :members:
    :undoc-members:
    :show-inheritance:
 
+dfvfs.volume.apm\_volume\_system module
+---------------------------------------
+
+.. automodule:: dfvfs.volume.apm_volume_system
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 dfvfs.volume.cs\_volume\_system module
 --------------------------------------
 
 .. automodule:: dfvfs.volume.cs_volume_system
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `dfvfs-20230408/docs/sources/developer/Adding-new-type.md` & `dfvfs-20230507/docs/sources/developer/Adding-new-type.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/developer/Helpers.md` & `dfvfs-20230507/docs/sources/developer/Helpers.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/developer/Internals.md` & `dfvfs-20230507/docs/sources/developer/Internals.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/docs/sources/user/Installation-instructions.md` & `dfvfs-20230507/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/requirements.txt` & `dfvfs-20230507/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 libphdi-python >= 20220228
 libqcow-python >= 20201213
 libsigscan-python >= 20191221
 libsmdev-python >= 20140529
 libsmraw-python >= 20140612
 libvhdi-python >= 20201014
 libvmdk-python >= 20140421
+libvsapm-python >= 20230506
 libvsgpt-python >= 20211115
 libvshadow-python >= 20160109
 libvslvm-python >= 20160109
 pytsk3 >= 20210419
 pyxattr >= 0.7.2 ; platform_system != "Windows"
```

### Comparing `dfvfs-20230408/run_tests.py` & `dfvfs-20230507/run_tests.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/setup.cfg` & `dfvfs-20230507/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 	libphdi-python3 >= 20220228
 	libqcow-python3 >= 20201213
 	libsigscan-python3 >= 20191221
 	libsmdev-python3 >= 20140529
 	libsmraw-python3 >= 20140612
 	libvhdi-python3 >= 20201014
 	libvmdk-python3 >= 20140421
+	libvsapm-python3 >= 20230506
 	libvsgpt-python3 >= 20211115
 	libvshadow-python3 >= 20160109
 	libvslvm-python3 >= 20160109
 	python3-cffi >= 1.9.1
 	python3-cryptography >= 2.0.2
 	python3-dfdatetime >= 20221112
 	python3-dtfabric >= 20220219
```

### Comparing `dfvfs-20230408/setup.py` & `dfvfs-20230507/setup.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/analyzer/analyzer.py` & `dfvfs-20230507/tests/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/analyzer/specification.py` & `dfvfs-20230507/tests/analyzer/specification.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/compression/bzip2_decompressor.py` & `dfvfs-20230507/tests/compression/bzip2_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/compression/manager.py` & `dfvfs-20230507/tests/compression/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/compression/xz_decompressor.py` & `dfvfs-20230507/tests/compression/xz_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/compression/zlib_decompressor.py` & `dfvfs-20230507/tests/compression/zlib_decompressor.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/credentials/apfs_credentials.py` & `dfvfs-20230507/tests/credentials/apfs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/credentials/bde_credentials.py` & `dfvfs-20230507/tests/credentials/bde_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/credentials/cs_credentials.py` & `dfvfs-20230507/tests/credentials/cs_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/credentials/encrypted_stream_credentials.py` & `dfvfs-20230507/tests/credentials/encrypted_stream_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/credentials/keychain.py` & `dfvfs-20230507/tests/credentials/keychain.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/credentials/luksde_credentials.py` & `dfvfs-20230507/tests/credentials/luksde_credentials.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/credentials/manager.py` & `dfvfs-20230507/tests/credentials/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encoding/base16_decoder.py` & `dfvfs-20230507/tests/encoding/base16_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encoding/base32_decoder.py` & `dfvfs-20230507/tests/encoding/base32_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encoding/base64_decoder.py` & `dfvfs-20230507/tests/encoding/base64_decoder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encoding/manager.py` & `dfvfs-20230507/tests/encoding/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encryption/aes_decrypter.py` & `dfvfs-20230507/tests/encryption/aes_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encryption/blowfish_decrypter.py` & `dfvfs-20230507/tests/encryption/blowfish_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encryption/decrypter.py` & `dfvfs-20230507/tests/encryption/decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encryption/des3_decrypter.py` & `dfvfs-20230507/tests/encryption/des3_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encryption/manager.py` & `dfvfs-20230507/tests/encryption/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/encryption/rc4_decrypter.py` & `dfvfs-20230507/tests/encryption/rc4_decrypter.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/apfs_file_io.py` & `dfvfs-20230507/tests/file_io/apfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/bde_file_io.py` & `dfvfs-20230507/tests/file_io/bde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/compressed_stream_io.py` & `dfvfs-20230507/tests/file_io/compressed_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/cpio_file_io.py` & `dfvfs-20230507/tests/file_io/cpio_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/cs_file_io.py` & `dfvfs-20230507/tests/file_io/cs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/data_range_io.py` & `dfvfs-20230507/tests/file_io/data_range_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/encoded_stream_io.py` & `dfvfs-20230507/tests/file_io/encoded_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/encrypted_stream_io.py` & `dfvfs-20230507/tests/file_io/encrypted_stream_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/ewf_file_io.py` & `dfvfs-20230507/tests/file_io/ewf_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/ext_file_io.py` & `dfvfs-20230507/tests/file_io/ext_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/fake_file_io.py` & `dfvfs-20230507/tests/file_io/fake_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/fat_file_io.py` & `dfvfs-20230507/tests/file_io/fat_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/gpt_file_io.py` & `dfvfs-20230507/tests/file_io/gpt_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/gzip_file_io.py` & `dfvfs-20230507/tests/file_io/gzip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/hfs_file_io.py` & `dfvfs-20230507/tests/file_io/hfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/luksde_file_io.py` & `dfvfs-20230507/tests/file_io/luksde_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/lvm_file_io.py` & `dfvfs-20230507/tests/file_io/lvm_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/modi_file_io.py` & `dfvfs-20230507/tests/file_io/modi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/ntfs_file_io.py` & `dfvfs-20230507/tests/file_io/ntfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/os_file_io.py` & `dfvfs-20230507/tests/file_io/os_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/phdi_file_io.py` & `dfvfs-20230507/tests/file_io/phdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/qcow_file_io.py` & `dfvfs-20230507/tests/file_io/qcow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/raw_file_io.py` & `dfvfs-20230507/tests/file_io/raw_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/sqlite_blob_file_io.py` & `dfvfs-20230507/tests/file_io/sqlite_blob_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/tar_file_io.py` & `dfvfs-20230507/tests/file_io/tar_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/test_lib.py` & `dfvfs-20230507/tests/file_io/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/tsk_file_io.py` & `dfvfs-20230507/tests/file_io/tsk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/tsk_partition_file_io.py` & `dfvfs-20230507/tests/file_io/tsk_partition_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/vhdi_file_io.py` & `dfvfs-20230507/tests/file_io/vhdi_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/vmdk_file_io.py` & `dfvfs-20230507/tests/file_io/vmdk_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/vshadow_file_io.py` & `dfvfs-20230507/tests/file_io/vshadow_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/xfs_file_io.py` & `dfvfs-20230507/tests/file_io/xfs_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/file_io/zip_file_io.py` & `dfvfs-20230507/tests/file_io/zip_file_io.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/helpers/command_line.py` & `dfvfs-20230507/tests/helpers/command_line.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/helpers/data_slice.py` & `dfvfs-20230507/tests/helpers/data_slice.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/helpers/fake_file_system_builder.py` & `dfvfs-20230507/tests/helpers/fake_file_system_builder.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/helpers/file_system_searcher.py` & `dfvfs-20230507/tests/helpers/file_system_searcher.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/helpers/source_scanner.py` & `dfvfs-20230507/tests/helpers/source_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/helpers/text_file.py` & `dfvfs-20230507/tests/helpers/text_file.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/helpers/volume_scanner.py` & `dfvfs-20230507/tests/helpers/volume_scanner.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/helpers/windows_path_resolver.py` & `dfvfs-20230507/tests/helpers/windows_path_resolver.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/lib/apfs_helper.py` & `dfvfs-20230507/tests/lib/apfs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/lib/cpio.py` & `dfvfs-20230507/tests/lib/cpio.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/lib/cs_helper.py` & `dfvfs-20230507/tests/lib/cs_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/lib/ewf_helper.py` & `dfvfs-20230507/tests/lib/ewf_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/lib/glob2regex.py` & `dfvfs-20230507/tests/lib/glob2regex.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/lib/gzipfile.py` & `dfvfs-20230507/tests/lib/gzipfile.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/lib/lvm_helper.py` & `dfvfs-20230507/tests/lib/lvm_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/lib/raw_helper.py` & `dfvfs-20230507/tests/lib/raw_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/mount/manager.py` & `dfvfs-20230507/tests/mount/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/apfs_container_path_spec.py` & `dfvfs-20230507/tests/path/apfs_container_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/apfs_path_spec.py` & `dfvfs-20230507/tests/path/apfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/bde_path_spec.py` & `dfvfs-20230507/tests/path/bde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/compressed_stream_path_spec.py` & `dfvfs-20230507/tests/path/compressed_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/cpio_path_spec.py` & `dfvfs-20230507/tests/path/cpio_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/cs_path_spec.py` & `dfvfs-20230507/tests/path/cs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/data_range_path_spec.py` & `dfvfs-20230507/tests/path/data_range_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/encoded_stream_path_spec.py` & `dfvfs-20230507/tests/path/encoded_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/encryption_stream_path_spec.py` & `dfvfs-20230507/tests/path/encryption_stream_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/ewf_path_spec.py` & `dfvfs-20230507/tests/path/ewf_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/ext_path_spec.py` & `dfvfs-20230507/tests/path/ext_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/factory.py` & `dfvfs-20230507/tests/path/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/fake_path_spec.py` & `dfvfs-20230507/tests/path/fake_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/fat_path_spec.py` & `dfvfs-20230507/tests/path/fat_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/gpt_path_spec.py` & `dfvfs-20230507/tests/path/gpt_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/gzip_path_spec.py` & `dfvfs-20230507/tests/path/gzip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/hfs_path_spec.py` & `dfvfs-20230507/tests/path/hfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/luksde_path_spec.py` & `dfvfs-20230507/tests/path/luksde_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/lvm_path_spec.py` & `dfvfs-20230507/tests/path/lvm_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/modi_path_spec.py` & `dfvfs-20230507/tests/path/modi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/mount_path_spec.py` & `dfvfs-20230507/tests/path/mount_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/ntfs_path_spec.py` & `dfvfs-20230507/tests/path/ntfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/os_path_spec.py` & `dfvfs-20230507/tests/path/os_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/path_spec.py` & `dfvfs-20230507/tests/path/path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/phdi_path_spec.py` & `dfvfs-20230507/tests/path/phdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/qcow_path_spec.py` & `dfvfs-20230507/tests/path/qcow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/raw_path_spec.py` & `dfvfs-20230507/tests/path/raw_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/sqlite_blob_path_spec.py` & `dfvfs-20230507/tests/path/sqlite_blob_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/tar_path_spec.py` & `dfvfs-20230507/tests/path/tar_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/test_lib.py` & `dfvfs-20230507/tests/path/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/tsk_partition_path_spec.py` & `dfvfs-20230507/tests/path/tsk_partition_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/tsk_path_spec.py` & `dfvfs-20230507/tests/path/tsk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/vhdi_path_spec.py` & `dfvfs-20230507/tests/path/vhdi_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/vmdk_path_spec.py` & `dfvfs-20230507/tests/path/vmdk_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/vshadow_path_spec.py` & `dfvfs-20230507/tests/path/vshadow_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/xfs_path_spec.py` & `dfvfs-20230507/tests/path/xfs_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/path/zip_path_spec.py` & `dfvfs-20230507/tests/path/zip_path_spec.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver/context.py` & `dfvfs-20230507/tests/resolver/context.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/apfs_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/apfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/bde_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/bde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/compressed_stream_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/compressed_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/cpio_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/cpio_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/cs_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/cs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/encoded_stream_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/encoded_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/encrypted_stream_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/encrypted_stream_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/ewf_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/ewf_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/ext_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/ext_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/fat_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/fat_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/gpt_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/gpt_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/gzip_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/gzip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/hfs_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/hfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/luksde_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/luksde_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/lvm_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/lvm_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/manager.py` & `dfvfs-20230507/tests/resolver_helpers/manager.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/modi_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/modi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/ntfs_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/ntfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/os_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/os_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/phdi_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/phdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/qcow_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/qcow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/raw_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/raw_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/sqlite_blob_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/sqlite_blob_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/tar_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/tar_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/test_lib.py` & `dfvfs-20230507/tests/resolver_helpers/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/tsk_partition_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/tsk_partition_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/tsk_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/tsk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/vhdi_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/vhdi_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/vmdk_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/vmdk_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/vshadow_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/vshadow_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/xfs_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/xfs_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/resolver_helpers/zip_resolver_helper.py` & `dfvfs-20230507/tests/resolver_helpers/zip_resolver_helper.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/serializer/json_serializer.py` & `dfvfs-20230507/tests/serializer/json_serializer.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/test_lib.py` & `dfvfs-20230507/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/apfs_attribute.py` & `dfvfs-20230507/tests/vfs/apfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/apfs_container_directory.py` & `dfvfs-20230507/tests/vfs/apfs_container_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/apfs_container_file_entry.py` & `dfvfs-20230507/tests/vfs/apfs_container_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/apfs_container_file_system.py` & `dfvfs-20230507/tests/vfs/apfs_container_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/apfs_directory.py` & `dfvfs-20230507/tests/vfs/apfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/apfs_file_entry.py` & `dfvfs-20230507/tests/vfs/apfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/apfs_file_system.py` & `dfvfs-20230507/tests/vfs/apfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/attribute.py` & `dfvfs-20230507/tests/vfs/attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/bde_file_entry.py` & `dfvfs-20230507/tests/vfs/bde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/bde_file_system.py` & `dfvfs-20230507/tests/vfs/bde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/compressed_stream_file_entry.py` & `dfvfs-20230507/tests/vfs/compressed_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/compressed_stream_file_system.py` & `dfvfs-20230507/tests/vfs/compressed_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/cpio_directory.py` & `dfvfs-20230507/tests/vfs/cpio_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/cpio_file_entry.py` & `dfvfs-20230507/tests/vfs/cpio_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/cpio_file_system.py` & `dfvfs-20230507/tests/vfs/cpio_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/cs_file_entry.py` & `dfvfs-20230507/tests/vfs/cs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/cs_file_system.py` & `dfvfs-20230507/tests/vfs/cs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/data_range_file_entry.py` & `dfvfs-20230507/tests/vfs/data_range_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/data_range_file_system.py` & `dfvfs-20230507/tests/vfs/data_range_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/data_stream.py` & `dfvfs-20230507/tests/vfs/data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/directory.py` & `dfvfs-20230507/tests/vfs/directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/encoded_stream_file_entry.py` & `dfvfs-20230507/tests/vfs/encoded_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/encoded_stream_file_system.py` & `dfvfs-20230507/tests/vfs/encoded_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/encrypted_stream_file_entry.py` & `dfvfs-20230507/tests/vfs/encrypted_stream_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/encrypted_stream_file_system.py` & `dfvfs-20230507/tests/vfs/encrypted_stream_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/ext_attribute.py` & `dfvfs-20230507/tests/vfs/ext_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/ext_directory.py` & `dfvfs-20230507/tests/vfs/ext_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/ext_file_entry.py` & `dfvfs-20230507/tests/vfs/ext_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/ext_file_system.py` & `dfvfs-20230507/tests/vfs/ext_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/fake_directory.py` & `dfvfs-20230507/tests/vfs/fake_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/fake_file_entry.py` & `dfvfs-20230507/tests/vfs/fake_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/fake_file_system.py` & `dfvfs-20230507/tests/vfs/fake_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/fat_directory.py` & `dfvfs-20230507/tests/vfs/fat_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/fat_file_entry.py` & `dfvfs-20230507/tests/vfs/fat_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/fat_file_system.py` & `dfvfs-20230507/tests/vfs/fat_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/file_entry.py` & `dfvfs-20230507/tests/vfs/file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/file_system.py` & `dfvfs-20230507/tests/vfs/file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/gpt_directory.py` & `dfvfs-20230507/tests/vfs/gpt_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/gpt_file_entry.py` & `dfvfs-20230507/tests/vfs/gpt_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/gpt_file_system.py` & `dfvfs-20230507/tests/vfs/gpt_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/gzip_file_entry.py` & `dfvfs-20230507/tests/vfs/gzip_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/gzip_file_system.py` & `dfvfs-20230507/tests/vfs/gzip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/hfs_attribute.py` & `dfvfs-20230507/tests/vfs/hfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/hfs_data_stream.py` & `dfvfs-20230507/tests/vfs/hfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/hfs_directory.py` & `dfvfs-20230507/tests/vfs/hfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/hfs_file_entry.py` & `dfvfs-20230507/tests/vfs/hfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/hfs_file_system.py` & `dfvfs-20230507/tests/vfs/hfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/luksde_file_entry.py` & `dfvfs-20230507/tests/vfs/luksde_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/luksde_file_system.py` & `dfvfs-20230507/tests/vfs/luksde_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/lvm_directory.py` & `dfvfs-20230507/tests/vfs/lvm_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/lvm_file_entry.py` & `dfvfs-20230507/tests/vfs/lvm_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/lvm_file_system.py` & `dfvfs-20230507/tests/vfs/lvm_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/ntfs_attibute.py` & `dfvfs-20230507/tests/vfs/ntfs_attibute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/ntfs_data_stream.py` & `dfvfs-20230507/tests/vfs/ntfs_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/ntfs_directory.py` & `dfvfs-20230507/tests/vfs/ntfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/ntfs_file_entry.py` & `dfvfs-20230507/tests/vfs/ntfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/ntfs_file_system.py` & `dfvfs-20230507/tests/vfs/ntfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/os_directory.py` & `dfvfs-20230507/tests/vfs/os_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/os_file_entry.py` & `dfvfs-20230507/tests/vfs/os_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/os_file_system.py` & `dfvfs-20230507/tests/vfs/os_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/sqlite_blob_directory.py` & `dfvfs-20230507/tests/vfs/sqlite_blob_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/sqlite_blob_file_entry.py` & `dfvfs-20230507/tests/vfs/sqlite_blob_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/sqlite_blob_file_system.py` & `dfvfs-20230507/tests/vfs/sqlite_blob_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/tar_directory.py` & `dfvfs-20230507/tests/vfs/tar_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/tar_file_entry.py` & `dfvfs-20230507/tests/vfs/tar_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/tar_file_system.py` & `dfvfs-20230507/tests/vfs/tar_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/tsk_attribute.py` & `dfvfs-20230507/tests/vfs/tsk_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/tsk_data_stream.py` & `dfvfs-20230507/tests/vfs/tsk_data_stream.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/tsk_directory.py` & `dfvfs-20230507/tests/vfs/tsk_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/tsk_file_entry.py` & `dfvfs-20230507/tests/vfs/tsk_file_entry.py`

 * *Files 8% similar despite different names*

```diff
@@ -2014,9 +2014,420 @@
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     with self.assertRaises(errors.BackEndError):
       file_entry.GetFileObject()
 
 
+class TSKFileEntryTestUfs1(shared_test_lib.BaseTestCase):
+  """Tests the SleuthKit (TSK) file entry on ufs1."""
+
+  # pylint: disable=protected-access
+
+  _INODE_A_DIRECTORY = 256
+  _INODE_A_FILE = 257
+  _INODE_A_LINK = 5
+  _INODE_ANOTHER_FILE = 258
+
+  def setUp(self):
+    """Sets up the needed objects used throughout the test."""
+    self._resolver_context = context.Context()
+    test_path = self._GetTestFilePath(['ufs1.raw'])
+    self._SkipIfPathNotExists(test_path)
+
+    test_os_path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_OS, location=test_path)
+    raw_path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_RAW, parent=test_os_path_spec)
+    self._tsk_partition_path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK_PARTITION, location='/p1',
+        parent=raw_path_spec)
+    self._tsk_path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, location='/',
+        parent=self._tsk_partition_path_spec)
+
+    self._file_system = tsk_file_system.TSKFileSystem(
+        self._resolver_context, self._tsk_path_spec)
+    self._file_system.Open()
+
+  def tearDown(self):
+    """Cleans up the needed objects used throughout the test."""
+    self._resolver_context.Empty()
+
+  def testInitialize(self):
+    """Tests the __init__ function."""
+    file_entry = tsk_file_entry.TSKFileEntry(
+        self._resolver_context, self._file_system, self._tsk_path_spec)
+
+    self.assertIsNotNone(file_entry)
+
+  def testGetAttributes(self):
+    """Tests the _GetAttributes function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_A_FILE,
+        location='/a_directory/a_file', parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    self.assertIsNone(file_entry._attributes)
+
+    file_entry._GetAttributes()
+    self.assertIsNotNone(file_entry._attributes)
+    self.assertEqual(len(file_entry._attributes), 0)
+
+    # No extended attributes are returned.
+    # Also see: https://github.com/py4n6/pytsk/issues/79.
+
+  def testGetDataStreams(self):
+    """Tests the _GetDataStreams function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    data_streams = file_entry._GetDataStreams()
+    self.assertEqual(len(data_streams), 1)
+
+  # TODO: add tests for _GetDirectory
+  # TODO: add tests for _GetLink
+
+  def testGetStatAttribute(self):
+    """Tests the _GetStatAttribute function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    stat_attribute = file_entry._GetStatAttribute()
+
+    self.assertIsNotNone(stat_attribute)
+    self.assertEqual(stat_attribute.group_identifier, 0)
+    self.assertEqual(stat_attribute.inode_number, 258)
+    self.assertEqual(stat_attribute.mode, 0o644)
+    self.assertEqual(stat_attribute.number_of_links, 1)
+    self.assertEqual(stat_attribute.owner_identifier, 0)
+    self.assertEqual(stat_attribute.size, 22)
+    self.assertEqual(stat_attribute.type, stat_attribute.TYPE_FILE)
+
+  # TODO: add tests for _GetSubFileEntries
+  # TODO: add tests for _GetTimeValue
+
+  def testAccessTime(self):
+    """Test the access_time property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+    self.assertIsNotNone(file_entry.access_time)
+
+  def testBackupTime(self):
+    """Test the backup_time property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+    self.assertIsNone(file_entry.backup_time)
+
+  def testChangeTime(self):
+    """Test the change_time property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+    self.assertIsNotNone(file_entry.change_time)
+
+  def testCreationTime(self):
+    """Test the creation_time property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+    self.assertIsNone(file_entry.creation_time)
+
+  def testDeletionTime(self):
+    """Test the deletion_time property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+    self.assertIsNone(file_entry.deletion_time)
+
+  def testModificationTime(self):
+    """Test the modification_time property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+    self.assertIsNotNone(file_entry.modification_time)
+
+  def testName(self):
+    """Test the name property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+    self.assertEqual(file_entry.name, 'another_file')
+
+  def testSize(self):
+    """Test the size property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+    self.assertEqual(file_entry.size, 22)
+
+  def testGetExtents(self):
+    """Tests the GetExtents function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_EXT, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    extents = file_entry.GetExtents()
+    self.assertEqual(len(extents), 1)
+
+    self.assertEqual(extents[0].extent_type, definitions.EXTENT_TYPE_DATA)
+    self.assertEqual(extents[0].offset, 4169728)
+    self.assertEqual(extents[0].size, 4096)
+
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_EXT, inode=self._INODE_A_DIRECTORY,
+        location='/a_directory', parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    extents = file_entry.GetExtents()
+    self.assertEqual(len(extents), 0)
+
+  def testGetFileEntryByPathSpec(self):
+    """Tests the GetFileEntryByPathSpec function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+
+  def testGetFileObject(self):
+    """Tests the GetFileObject function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    file_object = file_entry.GetFileObject()
+    self.assertIsNotNone(file_object)
+
+    self.assertEqual(file_object.get_size(), 22)
+
+    file_object = file_entry.GetFileObject(data_stream_name='bogus')
+    self.assertIsNone(file_object)
+
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_A_DIRECTORY,
+        location='/a_directory', parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    with self.assertRaises(errors.BackEndError):
+      file_entry.GetFileObject()
+
+  def testGetLinkedFileEntry(self):
+    """Tests the GetLinkedFileEntry function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_A_LINK,
+        location='/a_link', parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    linked_file_entry = file_entry.GetLinkedFileEntry()
+
+    self.assertIsNotNone(linked_file_entry)
+
+    self.assertEqual(linked_file_entry.name, 'another_file')
+
+  def testGetParentFileEntry(self):
+    """Tests the GetParentFileEntry function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    parent_file_entry = file_entry.GetParentFileEntry()
+
+    self.assertIsNotNone(parent_file_entry)
+
+    self.assertEqual(parent_file_entry.name, 'a_directory')
+
+  # TODO: add tests for GetTSKFile
+
+  def testIsFunctions(self):
+    """Tests the Is? functions."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    self.assertFalse(file_entry.IsRoot())
+    self.assertFalse(file_entry.IsVirtual())
+    self.assertTrue(file_entry.IsAllocated())
+
+    self.assertFalse(file_entry.IsDevice())
+    self.assertFalse(file_entry.IsDirectory())
+    self.assertTrue(file_entry.IsFile())
+    self.assertFalse(file_entry.IsLink())
+    self.assertFalse(file_entry.IsPipe())
+    self.assertFalse(file_entry.IsSocket())
+
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_A_DIRECTORY,
+        location='/a_directory', parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    self.assertFalse(file_entry.IsRoot())
+    self.assertFalse(file_entry.IsVirtual())
+    self.assertTrue(file_entry.IsAllocated())
+
+    self.assertFalse(file_entry.IsDevice())
+    self.assertTrue(file_entry.IsDirectory())
+    self.assertFalse(file_entry.IsFile())
+    self.assertFalse(file_entry.IsLink())
+    self.assertFalse(file_entry.IsPipe())
+    self.assertFalse(file_entry.IsSocket())
+
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, location='/',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    self.assertTrue(file_entry.IsRoot())
+    self.assertFalse(file_entry.IsVirtual())
+    self.assertTrue(file_entry.IsAllocated())
+
+    self.assertFalse(file_entry.IsDevice())
+    self.assertTrue(file_entry.IsDirectory())
+    self.assertFalse(file_entry.IsFile())
+    self.assertFalse(file_entry.IsLink())
+    self.assertFalse(file_entry.IsPipe())
+    self.assertFalse(file_entry.IsSocket())
+
+  def testSubFileEntries(self):
+    """Tests the number_of_sub_file_entries and sub_file_entries properties."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, location='/',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    self.assertEqual(file_entry.number_of_sub_file_entries, 5)
+
+    # Note that passwords.txt~ is currently ignored by dfVFS, since
+    # its directory entry has no pytsk3.TSK_FS_META object.
+    expected_sub_file_entry_names = [
+        '.snap',
+        'a_directory',
+        'a_link',
+        'passwords.txt',
+        '$OrphanFiles']
+
+    sub_file_entry_names = []
+    for sub_file_entry in file_entry.sub_file_entries:
+      sub_file_entry_names.append(sub_file_entry.name)
+
+    self.assertEqual(
+        len(sub_file_entry_names), len(expected_sub_file_entry_names))
+    self.assertEqual(
+        sorted(sub_file_entry_names), sorted(expected_sub_file_entry_names))
+
+    # Test a path specification without a location.
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_A_DIRECTORY,
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    self.assertEqual(file_entry.number_of_sub_file_entries, 2)
+
+  def testDataStreams(self):
+    """Tests the data streams functionality."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    self.assertEqual(file_entry.number_of_data_streams, 1)
+
+    data_stream_names = []
+    for data_stream in file_entry.data_streams:
+      data_stream_names.append(data_stream.name)
+
+    self.assertEqual(data_stream_names, [''])
+
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_A_DIRECTORY,
+        location='/a_directory', parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    self.assertEqual(file_entry.number_of_data_streams, 0)
+
+    data_stream_names = []
+    for data_stream in file_entry.data_streams:
+      data_stream_names.append(data_stream.name)
+
+    self.assertEqual(data_stream_names, [])
+
+  def testGetDataStream(self):
+    """Tests the GetDataStream function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_TSK, inode=self._INODE_ANOTHER_FILE,
+        location='/a_directory/another_file',
+        parent=self._tsk_partition_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    data_stream = file_entry.GetDataStream('')
+    self.assertIsNotNone(data_stream)
+
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `dfvfs-20230408/tests/vfs/tsk_file_system.py` & `dfvfs-20230507/tests/vfs/tsk_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/tsk_partition_directory.py` & `dfvfs-20230507/tests/vfs/tsk_partition_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/tsk_partition_file_entry.py` & `dfvfs-20230507/tests/vfs/zip_file_entry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,386 +1,365 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-"""Tests for the partition file entry implementation using pytsk3."""
+"""Tests for the file entry implementation using the zipfile."""
 
 import unittest
 
 from dfvfs.lib import definitions
 from dfvfs.path import factory as path_spec_factory
 from dfvfs.resolver import context
-from dfvfs.vfs import tsk_partition_file_entry
-from dfvfs.vfs import tsk_partition_file_system
+from dfvfs.vfs import zip_file_entry
+from dfvfs.vfs import zip_file_system
 
 from tests import test_lib as shared_test_lib
 
 
-class TSKPartitionFileEntryTestAPM(shared_test_lib.BaseTestCase):
-  """TSK partition file entry tests on APM."""
+class ZIPFileEntryTest(shared_test_lib.BaseTestCase):
+  """Tests the ZIP extracted file entry."""
+
+  # pylint: disable=protected-access
 
   def setUp(self):
     """Sets up the needed objects used throughout the test."""
     self._resolver_context = context.Context()
-    test_path = self._GetTestFilePath(['apm.dmg'])
+    test_path = self._GetTestFilePath(['syslog.zip'])
     self._SkipIfPathNotExists(test_path)
 
     self._os_path_spec = path_spec_factory.Factory.NewPathSpec(
         definitions.TYPE_INDICATOR_OS, location=test_path)
-    self._tsk_partition_path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, location='/',
-        parent=self._os_path_spec)
+    self._zip_path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
 
-    self._file_system = tsk_partition_file_system.TSKPartitionFileSystem(
-        self._resolver_context, self._tsk_partition_path_spec)
+    self._file_system = zip_file_system.ZipFileSystem(
+        self._resolver_context, self._zip_path_spec)
     self._file_system.Open()
 
   def tearDown(self):
     """Cleans up the needed objects used throughout the test."""
     self._resolver_context.Empty()
 
-  # mmls test_data/apm.dmg
-  # MAC Partition Map
-  # Offset Sector: 0
-  # Units are in 512-byte sectors
-  #
-  #       Slot      Start        End          Length       Description
-  # 000:  -------   0000000000   0000000000   0000000001   Unallocated
-  # 001:  000       0000000001   0000000063   0000000063   Apple_partition_map
-  # 002:  Meta      0000000001   0000000003   0000000003   Table
-  # 003:  001       0000000064   0000008175   0000008112   Apple_HFS
-  # 004:  002       0000008176   0000008191   0000000016   Apple_Free
-
   def testIntialize(self):
     """Test the __init__ function."""
-    file_entry = tsk_partition_file_entry.TSKPartitionFileEntry(
-        self._resolver_context, self._file_system,
-        self._tsk_partition_path_spec, is_virtual=True)
+    file_entry = zip_file_entry.ZipFileEntry(
+        self._resolver_context, self._file_system, self._zip_path_spec,
+        is_virtual=True)
 
     self.assertIsNotNone(file_entry)
 
-  # TODO: add tests for _GetDirectory
+  # TODO: add tests for _GetDirectory function.
   # TODO: add tests for _GetSubFileEntries
 
-  def testName(self):
-    """Test the name property."""
+  def testAccessTime(self):
+    """Test the access_time property."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=3,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
-    self.assertEqual(file_entry.name, 'p1')
+    self.assertIsNone(file_entry.access_time)
 
-  def testSize(self):
-    """Test the size property."""
+  def testChangeTime(self):
+    """Test the change_time property."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=3,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
-    self.assertEqual(file_entry.size, 8112 * 512)
+    self.assertIsNone(file_entry.change_time)
 
-  def testGetParentFileEntry(self):
-    """Tests the GetParentFileEntry function."""
+  def testCreationTime(self):
+    """Test the creation_time property."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=0,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
-    parent_file_entry = file_entry.GetParentFileEntry()
-    self.assertIsNone(parent_file_entry)
+    self.assertIsNone(file_entry.creation_time)
 
-  # TODO: add tests for GetTSKVsPart
-
-  def testIsFunctions(self):
-    """Test the Is? functions."""
+  def testDataStreams(self):
+    """Test the data_streams property."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=0,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
-    self.assertFalse(file_entry.IsRoot())
-    self.assertFalse(file_entry.IsVirtual())
-    self.assertFalse(file_entry.IsAllocated())
+    self.assertEqual(file_entry.number_of_data_streams, 1)
 
-    self.assertFalse(file_entry.IsDevice())
-    self.assertFalse(file_entry.IsDirectory())
-    self.assertTrue(file_entry.IsFile())
-    self.assertFalse(file_entry.IsLink())
-    self.assertFalse(file_entry.IsPipe())
-    self.assertFalse(file_entry.IsSocket())
+    data_stream_names = []
+    for data_stream in file_entry.data_streams:
+      data_stream_names.append(data_stream.name)
+
+    self.assertEqual(data_stream_names, [''])
 
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, location='/',
-        parent=self._os_path_spec)
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
-    self.assertTrue(file_entry.IsRoot())
-    self.assertTrue(file_entry.IsVirtual())
-    self.assertTrue(file_entry.IsAllocated())
+    self.assertEqual(file_entry.number_of_data_streams, 0)
 
-    self.assertFalse(file_entry.IsDevice())
-    self.assertTrue(file_entry.IsDirectory())
-    self.assertFalse(file_entry.IsFile())
-    self.assertFalse(file_entry.IsLink())
-    self.assertFalse(file_entry.IsPipe())
-    self.assertFalse(file_entry.IsSocket())
+    data_stream_names = []
+    for data_stream in file_entry.data_streams:
+      data_stream_names.append(data_stream.name)
 
-  def testSubFileEntries(self):
-    """Test the sub file entries iteration functionality."""
+    self.assertEqual(data_stream_names, [])
+
+  def testModificationTime(self):
+    """Test the modification_time property."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, location='/',
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
-    self.assertIsNotNone(file_entry)
 
-    self.assertEqual(file_entry.number_of_sub_file_entries, 5)
+    self.assertIsNotNone(file_entry.modification_time)
 
-    expected_sub_file_entry_names = ['', '', '', '', 'p1']
-
-    sub_file_entry_names = []
-    for sub_file_entry in file_entry.sub_file_entries:
-      sub_file_entry_names.append(sub_file_entry.name)
+  def testName(self):
+    """Test the name property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
+        parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
-    self.assertEqual(
-        len(sub_file_entry_names), len(expected_sub_file_entry_names))
-    self.assertEqual(
-        sorted(sub_file_entry_names), sorted(expected_sub_file_entry_names))
+    self.assertIsNotNone(file_entry)
+    self.assertEqual(file_entry.name, 'syslog')
 
-  def testDataStreams(self):
-    """Test the data streams functionality."""
+  def testSize(self):
+    """Test the size property."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=0,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
     self.assertIsNotNone(file_entry)
+    self.assertEqual(file_entry.size, 1247)
 
-    self.assertEqual(file_entry.number_of_data_streams, 1)
+  def testSubFileEntries(self):
+    """Test the sub_file_entries property."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
-    data_stream_names = []
-    for data_stream in file_entry.data_streams:
-      data_stream_names.append(data_stream.name)
+    self.assertIsNotNone(file_entry)
+    self.assertEqual(file_entry.number_of_sub_file_entries, 2)
 
-    self.assertEqual(data_stream_names, [''])
+    self._assertSubFileEntries(file_entry, ['syslog', 'wtmp.1'])
+
+    # Test on a zip file that has missing directory entries.
+    test_path = self._GetTestFilePath(['missing_directory_entries.zip'])
+    self._SkipIfPathNotExists(test_path)
 
+    test_os_path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_OS, location=test_path)
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, location='/',
-        parent=self._os_path_spec)
-    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
-    self.assertIsNotNone(file_entry)
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=test_os_path_spec)
 
-    self.assertEqual(file_entry.number_of_data_streams, 0)
+    file_system = zip_file_system.ZipFileSystem(
+        self._resolver_context, path_spec)
+    self.assertIsNotNone(file_system)
 
-    data_stream_names = []
-    for data_stream in file_entry.data_streams:
-      data_stream_names.append(data_stream.name)
+    file_system.Open()
 
-    self.assertEqual(data_stream_names, [])
+    file_entry = file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
+
+    self._assertSubFileEntries(file_entry, ['folder'])
+
+    # The "folder" folder is a missing directory entry but should still
+    # be found due to the files found inside the directory.
+    sub_file_entry = next(file_entry.sub_file_entries)
+    self.assertTrue(sub_file_entry.IsVirtual())
+    self._assertSubFileEntries(sub_file_entry, ['syslog', 'wtmp.1'])
 
   def testGetDataStream(self):
     """Tests the GetDataStream function."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=0,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
     self.assertIsNotNone(file_entry)
 
     data_stream_name = ''
     data_stream = file_entry.GetDataStream(data_stream_name)
     self.assertIsNotNone(data_stream)
     self.assertEqual(data_stream.name, data_stream_name)
 
     data_stream = file_entry.GetDataStream('bogus')
     self.assertIsNone(data_stream)
 
+  def testGetParentFileEntry(self):
+    """Tests the GetParentFileEntry function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
+        parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+    self.assertIsNotNone(file_entry)
 
-class TSKPartitionFileEntryTestMBR(shared_test_lib.BaseTestCase):
-  """TSK partition file entry tests on MBR."""
+    parent_file_entry = file_entry.GetParentFileEntry()
 
-  def setUp(self):
-    """Sets up the needed objects used throughout the test."""
-    self._resolver_context = context.Context()
-    test_path = self._GetTestFilePath(['mbr.raw'])
-    self._SkipIfPathNotExists(test_path)
+    self.assertIsNotNone(parent_file_entry)
 
-    self._os_path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_OS, location=test_path)
-    self._tsk_partition_path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, location='/',
-        parent=self._os_path_spec)
+    self.assertEqual(parent_file_entry.name, '')
 
-    self._file_system = tsk_partition_file_system.TSKPartitionFileSystem(
-        self._resolver_context, self._tsk_partition_path_spec)
-    self._file_system.Open()
+  # TODO: add tests for GetZipInfo function.
 
-  def tearDown(self):
-    """Cleans up the needed objects used throughout the test."""
-    self._resolver_context.Empty()
+  def testIsAllocated(self):
+    """Test the IsAllocated function."""
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
+        parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
-  # mmls test_data/mbr.raw
-  # DOS Partition Table
-  # Offset Sector: 0
-  # Units are in 512-byte sectors
-  #
-  #       Slot      Start        End          Length       Description
-  # 000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
-  # 001:  -------   0000000000   0000000000   0000000001   Unallocated
-  # 002:  000:000   0000000001   0000000129   0000000129   Linux (0x83)
-  # 003:  Meta      0000000130   0000008191   0000008062   DOS Extended (0x05)
-  # 004:  Meta      0000000130   0000000130   0000000001   Extended Table (#1)
-  # 005:  -------   0000000130   0000000130   0000000001   Unallocated
-  # 006:  001:000   0000000131   0000000259   0000000129   Linux (0x83)
-  # 007:  -------   0000000260   0000008191   0000007932   Unallocated
+    self.assertIsNotNone(file_entry)
+    self.assertTrue(file_entry.IsAllocated())
 
-  def testIntialize(self):
-    """Test the __init__ function."""
-    file_entry = tsk_partition_file_entry.TSKPartitionFileEntry(
-        self._resolver_context, self._file_system,
-        self._tsk_partition_path_spec, is_virtual=True)
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
+    self.assertTrue(file_entry.IsAllocated())
 
-  # TODO: add tests for _GetDirectory
-  # TODO: add tests for _GetSubFileEntries
-
-  def testName(self):
-    """Test the name property."""
+  def testIsDevice(self):
+    """Test the IsDevice function."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=2,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
-    self.assertEqual(file_entry.name, 'p1')
+    self.assertFalse(file_entry.IsDevice())
 
-  def testSize(self):
-    """Test the size property."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=2,
-        parent=self._os_path_spec)
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
-    self.assertEqual(file_entry.size, 129 * 512)
+    self.assertFalse(file_entry.IsDevice())
 
-  def testGetParentFileEntry(self):
-    """Tests the GetParentFileEntry function."""
+  def testIsDirectory(self):
+    """Test the IsDirectory function."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=1,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
     self.assertIsNotNone(file_entry)
-    parent_file_entry = file_entry.GetParentFileEntry()
-    self.assertIsNone(parent_file_entry)
+    self.assertFalse(file_entry.IsDirectory())
 
-  # TODO: add tests for GetTSKVsPart
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
+    self.assertIsNotNone(file_entry)
+    self.assertTrue(file_entry.IsDirectory())
 
-  def testIsFunctions(self):
-    """Test the Is? functions."""
+  def testIsFile(self):
+    """Test the IsFile function."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=1,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
     self.assertIsNotNone(file_entry)
+    self.assertTrue(file_entry.IsFile())
 
-    self.assertFalse(file_entry.IsRoot())
-    self.assertFalse(file_entry.IsVirtual())
-    self.assertFalse(file_entry.IsAllocated())
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
-    self.assertFalse(file_entry.IsDevice())
-    self.assertFalse(file_entry.IsDirectory())
-    self.assertTrue(file_entry.IsFile())
-    self.assertFalse(file_entry.IsLink())
-    self.assertFalse(file_entry.IsPipe())
-    self.assertFalse(file_entry.IsSocket())
+    self.assertIsNotNone(file_entry)
+    self.assertFalse(file_entry.IsFile())
 
+  def testIsLink(self):
+    """Test the IsLink function."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, location='/',
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
     self.assertIsNotNone(file_entry)
+    self.assertFalse(file_entry.IsLink())
 
-    self.assertTrue(file_entry.IsRoot())
-    self.assertTrue(file_entry.IsVirtual())
-    self.assertTrue(file_entry.IsAllocated())
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
-    self.assertFalse(file_entry.IsDevice())
-    self.assertTrue(file_entry.IsDirectory())
-    self.assertFalse(file_entry.IsFile())
+    self.assertIsNotNone(file_entry)
     self.assertFalse(file_entry.IsLink())
-    self.assertFalse(file_entry.IsPipe())
-    self.assertFalse(file_entry.IsSocket())
 
-  def testSubFileEntries(self):
-    """Test the sub file entries iteration functionality."""
+  def testIsPipe(self):
+    """Test the IsPipe function."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, location='/',
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
-    self.assertIsNotNone(file_entry)
-
-    self.assertEqual(file_entry.number_of_sub_file_entries, 8)
 
-    expected_sub_file_entry_names = ['', '', '', '', '', '', 'p1', 'p2']
+    self.assertIsNotNone(file_entry)
+    self.assertFalse(file_entry.IsPipe())
 
-    sub_file_entry_names = []
-    for sub_file_entry in file_entry.sub_file_entries:
-      sub_file_entry_names.append(sub_file_entry.name)
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
-    self.assertEqual(
-        len(sub_file_entry_names), len(expected_sub_file_entry_names))
-    self.assertEqual(
-        sorted(sub_file_entry_names), sorted(expected_sub_file_entry_names))
+    self.assertIsNotNone(file_entry)
+    self.assertFalse(file_entry.IsPipe())
 
-  def testDataStreams(self):
-    """Test the data streams functionality."""
+  def testIsRoot(self):
+    """Test the IsRoot function."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=1,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
-    self.assertIsNotNone(file_entry)
 
-    self.assertEqual(file_entry.number_of_data_streams, 1)
+    self.assertIsNotNone(file_entry)
+    self.assertFalse(file_entry.IsRoot())
 
-    data_stream_names = []
-    for data_stream in file_entry.data_streams:
-      data_stream_names.append(data_stream.name)
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
-    self.assertEqual(data_stream_names, [''])
+    self.assertIsNotNone(file_entry)
+    self.assertTrue(file_entry.IsRoot())
 
+  def testIsSocket(self):
+    """Test the IsSocket function."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, location='/',
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
-    self.assertIsNotNone(file_entry)
 
-    self.assertEqual(file_entry.number_of_data_streams, 0)
+    self.assertIsNotNone(file_entry)
+    self.assertFalse(file_entry.IsSocket())
 
-    data_stream_names = []
-    for data_stream in file_entry.data_streams:
-      data_stream_names.append(data_stream.name)
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
-    self.assertEqual(data_stream_names, [])
+    self.assertIsNotNone(file_entry)
+    self.assertFalse(file_entry.IsSocket())
 
-  def testGetDataStream(self):
-    """Tests the GetDataStream function."""
+  def testIsVirtual(self):
+    """Test the IsVirtual function."""
     path_spec = path_spec_factory.Factory.NewPathSpec(
-        definitions.TYPE_INDICATOR_TSK_PARTITION, part_index=1,
+        definitions.TYPE_INDICATOR_ZIP, location='/syslog',
         parent=self._os_path_spec)
     file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
+
     self.assertIsNotNone(file_entry)
+    self.assertFalse(file_entry.IsVirtual())
 
-    data_stream_name = ''
-    data_stream = file_entry.GetDataStream(data_stream_name)
-    self.assertIsNotNone(data_stream)
-    self.assertEqual(data_stream.name, data_stream_name)
+    path_spec = path_spec_factory.Factory.NewPathSpec(
+        definitions.TYPE_INDICATOR_ZIP, location='/', parent=self._os_path_spec)
+    file_entry = self._file_system.GetFileEntryByPathSpec(path_spec)
 
-    data_stream = file_entry.GetDataStream('bogus')
-    self.assertIsNone(data_stream)
+    self.assertIsNotNone(file_entry)
+    self.assertTrue(file_entry.IsVirtual())
+
+  # TODO: add tests for GetZipInfo function.
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `dfvfs-20230408/tests/vfs/tsk_partition_file_system.py` & `dfvfs-20230507/tests/vfs/tsk_partition_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/vshadow_directory.py` & `dfvfs-20230507/tests/vfs/vshadow_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/vshadow_file_entry.py` & `dfvfs-20230507/tests/vfs/vshadow_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/vshadow_file_system.py` & `dfvfs-20230507/tests/vfs/vshadow_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/xfs_attribute.py` & `dfvfs-20230507/tests/vfs/xfs_attribute.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/xfs_directory.py` & `dfvfs-20230507/tests/vfs/xfs_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/xfs_file_entry.py` & `dfvfs-20230507/tests/vfs/xfs_file_entry.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/xfs_file_system.py` & `dfvfs-20230507/tests/vfs/xfs_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/zip_directory.py` & `dfvfs-20230507/tests/vfs/zip_directory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/vfs/zip_file_system.py` & `dfvfs-20230507/tests/vfs/zip_file_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/volume/apfs_volume_system.py` & `dfvfs-20230507/tests/volume/apfs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/volume/cs_volume_system.py` & `dfvfs-20230507/tests/volume/cs_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/volume/factory.py` & `dfvfs-20230507/tests/volume/factory.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/volume/gpt_volume_system.py` & `dfvfs-20230507/tests/volume/gpt_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/volume/lvm_volume_system.py` & `dfvfs-20230507/tests/volume/lvm_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/volume/tsk_volume_system.py` & `dfvfs-20230507/tests/volume/tsk_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tests/volume/vshadow_volume_system.py` & `dfvfs-20230507/tests/volume/vshadow_volume_system.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/tox.ini` & `dfvfs-20230507/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -14,31 +14,15 @@
     -rrequirements.txt
     -rtest_requirements.txt
     coverage: coverage
 commands =
     py3{7,8,9,10,11}: ./run_tests.py
     coverage: coverage erase
     coverage: coverage run --source=dfvfs --omit="*_test*,*__init__*,*test_lib*" run_tests.py
-
-[testenv:codecov]
-skip_install = True
-passenv =
-    CFLAGS
-    CPPFLAGS
-    GITHUB_ACTION
-    GITHUB_HEAD_REF
-    GITHUB_REF
-    GITHUB_REPOSITORY
-    GITHUB_RUN_ID
-    GITHUB_SHA
-    LDFLAGS
-deps =
-    codecov < 2.1.10
-commands =
-    codecov
+    coverage: coverage xml
 
 [testenv:docs]
 usedevelop = True
 deps =
     -rdocs/requirements.txt
 commands =
     sphinx-build -b html -d build/doctrees docs dist/docs
```

### Comparing `dfvfs-20230408/utils/dependencies.py` & `dfvfs-20230507/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/utils/generate_test_data_linux.sh` & `dfvfs-20230507/utils/generate_test_data_linux.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/bin/bash
+#!/usr/bin/env bash
 #
 # Script to generate dfVFS test files on Linux.
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 
 # Checks the availability of a binary and exits if not available.
```

### Comparing `dfvfs-20230408/utils/generate_test_data_macos.sh` & `dfvfs-20230507/utils/generate_test_data_macos.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/bin/bash
+#!/usr/bin/env bash
 #
 # Script to generate dfVFS test files on Mac OS.
 #
 # Requires:
 # * diskutil
 # * hdiutil
```

### Comparing `dfvfs-20230408/utils/generate_test_data_windows.bat` & `dfvfs-20230507/utils/generate_test_data_windows.bat`

 * *Files identical despite different names*

### Comparing `dfvfs-20230408/utils/update_release.sh` & `dfvfs-20230507/utils/update_release.sh`

 * *Files identical despite different names*

