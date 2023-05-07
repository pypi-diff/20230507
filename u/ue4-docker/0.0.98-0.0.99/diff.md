# Comparing `tmp/ue4-docker-0.0.98.tar.gz` & `tmp/ue4-docker-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ue4-docker-0.0.98.tar", last modified: Wed Apr 27 12:07:58 2022, max compression
+gzip compressed data, was "ue4-docker-0.0.99.tar", last modified: Wed Jun  8 07:39:50 2022, max compression
```

## Comparing `ue4-docker-0.0.98.tar` & `ue4-docker-0.0.99.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4387 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4_docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4_docker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23509 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/build.py
--rw-r--r--   0 runner    (1001) docker     (121)     2988 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5626 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/diagnostics/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/diagnostics/diagnostic_20gig.py
--rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/diagnostics/diagnostic_8gig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/diagnostics/diagnostic_all.py
--rw-r--r--   0 runner    (1001) docker     (121)     3445 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/diagnostics/diagnostic_maxsize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3961 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/diagnostics/diagnostic_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     2568 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/diagnostics_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/20gig/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/20gig/windows/
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/20gig/windows/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/8gig/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/8gig/linux/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/8gig/linux/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/8gig/windows/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/8gig/windows/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/8gig/windows/test.ps1
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/network/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/network/linux/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/network/linux/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/network/windows/
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/network/windows/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/linux/
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/linux/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/windows/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/windows/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/windows/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/windows/buildtools-exitcode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6293 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/windows/install-prerequisites.bat
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/windows/remove-duplicate-dlls.ps1
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-engine/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-engine/linux/
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-engine/linux/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-engine/windows/
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-engine/windows/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-full/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-full/linux/
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-full/linux/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-full/linux/pulseaudio-client.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-full/windows/
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-full/windows/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)     5949 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/copy-toolchain.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/enable-opengl.py
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/fix-targets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/patch-build-graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/patch-filters-xml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/set-changelist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/split-components.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)     3438 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/fix-targets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/patch-build-graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/patch-filters-xml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/set-changelist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2071 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/split-components.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/git-credential-helper-endpoint.sh
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/git-credential-helper-secrets.sh
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/linker-fixup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/patch-broken-releases.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/patch-ubt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/git-credential-helper.bat
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/patch-broken-releases.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/patch-setup-win.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/patch-ubt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/export.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/exports/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2970 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/exports/export_installed.py
--rw-r--r--   0 runner    (1001) docker     (121)     6904 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/exports/export_packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (121)    29322 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/BuildConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3496 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/CredentialEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/DarwinUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7305 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/DockerUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/FilesystemUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/GlobalConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (121)     9298 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/ImageBuilder.py
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/ImageCleaner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/Logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/NetworkUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/PackageUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/PrettyPrinting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/ResourceMonitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/SubprocessUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4848 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/WindowsUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     5036 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/setup_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 12:07:58.000000 ue4-docker-0.0.98/ue4docker/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/tests/build-and-package.py
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/tests/consume-external-deps.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/version.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-27 12:07:54.000000 ue4-docker-0.0.98/ue4docker/version_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.259077 ue4-docker-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3588 2022-06-08 07:39:50.259077 ue4-docker-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-08 07:39:50.259077 ue4-docker-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3588 2022-06-08 07:39:50.000000 ue4-docker-0.0.99/ue4_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-06-08 07:39:50.000000 ue4-docker-0.0.99/ue4_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 07:39:50.000000 ue4-docker-0.0.99/ue4_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-08 07:39:50.000000 ue4-docker-0.0.99/ue4_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 07:39:50.000000 ue4-docker-0.0.99/ue4_docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-06-08 07:39:50.000000 ue4-docker-0.0.99/ue4_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-08 07:39:50.000000 ue4-docker-0.0.99/ue4_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24481 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2988 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5626 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/diagnostics/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/diagnostics/diagnostic_20gig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/diagnostics/diagnostic_8gig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/diagnostics/diagnostic_all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3961 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/diagnostics/diagnostic_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/diagnostics_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.247077 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.247077 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/20gig/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/20gig/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/20gig/windows/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.247077 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/8gig/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/8gig/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/8gig/linux/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/8gig/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/8gig/windows/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      691 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/8gig/windows/test.ps1
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/network/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/network/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/network/linux/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/network/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/network/windows/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/linux/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/windows/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/windows/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/windows/buildtools-exitcode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6432 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/windows/install-prerequisites.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/windows/remove-duplicate-dlls.ps1
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-engine/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-engine/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-engine/linux/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-engine/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-engine/windows/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-full/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-full/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-full/linux/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-full/linux/pulseaudio-client.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-full/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-full/windows/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)     5998 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/copy-toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/enable-opengl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/fix-targets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/patch-build-graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/patch-filters-xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/set-changelist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/split-components.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3471 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/fix-targets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/patch-build-graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/patch-filters-xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/set-changelist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2071 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/split-components.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.251077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/git-credential-helper-endpoint.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/git-credential-helper-secrets.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/linker-fixup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/patch-broken-releases.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/patch-ubt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/git-credential-helper.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/patch-broken-releases.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/patch-setup-win.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/patch-ubt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/export.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.255077 ue4-docker-0.0.99/ue4docker/exports/
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2970 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/exports/export_installed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6904 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/exports/export_packages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/info.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.259077 ue4-docker-0.0.99/ue4docker/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (121)    30938 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/BuildConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3496 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/CredentialEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/DarwinUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7368 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/DockerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/FilesystemUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/GlobalConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10811 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/ImageBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/ImageCleaner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/NetworkUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/PackageUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/PrettyPrinting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/ResourceMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/SubprocessUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4848 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/WindowsUtils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5036 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/setup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 07:39:50.259077 ue4-docker-0.0.99/ue4docker/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/tests/build-and-package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/tests/consume-external-deps.py
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-08 07:39:47.000000 ue4-docker-0.0.99/ue4docker/version_cmd.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ue4-docker-0.0.98/PKG-INFO` & `ue4-docker-0.0.99/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 Metadata-Version: 2.1
 Name: ue4-docker
-Version: 0.0.98
+Version: 0.0.99
 Summary: Windows and Linux containers for Unreal Engine 4
 Home-page: http://github.com/adamrehn/ue4-docker
 Author: Adam Rehn
 Author-email: adam@adamrehn.com
 License: MIT
-Description: <p align="center"><img src="https://raw.githubusercontent.com/adamrehn/ue4-docker/master/resources/images/banner.svg?sanitize=true" alt="Unreal Engine and Docker Logos" height="100"></p>
-        <h1 align="center"><strong>Unreal Engine 4 Docker Containers</strong></h1>
-        <h3 align="center"><a href="https://docs.adamrehn.com/ue4-docker/use-cases/continuous-integration">Continuous Integration</a> &bull; <a href="https://docs.adamrehn.com/ue4-docker/use-cases/cloud-rendering">Cloud Rendering</a> &bull; <a href="https://docs.adamrehn.com/ue4-docker/use-cases/microservices">UE4-Powered Microservices</a></h3>
-        <p>&nbsp;</p>
-        
-        **Looking for a place to start? Check out the [Unreal Containers community hub](https://unrealcontainers.com/) for implementation-agnostic information on using the Unreal Engine inside Docker containers, and then head to the [comprehensive ue4-docker documentation](https://docs.adamrehn.com/ue4-docker/) to view details specific to using the ue4-docker project.**
-        
-        The ue4-docker Python package contains a set of Dockerfiles and accompanying build infrastructure that allows you to build Docker images for Epic Games' [Unreal Engine 4](https://www.unrealengine.com/). The images also incorporate the infrastructure from [ue4cli](https://github.com/adamrehn/ue4cli), [conan-ue4cli](https://github.com/adamrehn/conan-ue4cli), and [ue4-ci-helpers](https://github.com/adamrehn/ue4-ci-helpers) to facilitate a wide variety of use cases.
-        
-        Key features include:
-        
-        - Unreal Engine 4.20.0 and newer is supported.
-        - Both Windows containers and Linux containers are supported.
-        - Building and packaging UE4 projects is supported.
-        - Running automation tests is supported.
-        - Running built UE4 projects with offscreen rendering is supported via NVIDIA Docker under Linux.
-        
-        Resources:
-        
-        - **Documentation:** <https://docs.adamrehn.com/ue4-docker/>
-        - **GitHub repository:** <https://github.com/adamrehn/ue4-docker>
-        - **Package on PyPI:** <https://pypi.org/project/ue4-docker/>
-        - **Related articles:** <https://adamrehn.com/articles/tag/Unreal%20Engine/>
-        - **Unreal Containers community hub:** <https://unrealcontainers.com/>
-        - **Development channel on the Unreal Containers Community Discord server**: <https://discord.gg/46CJg9fyJ9>
-        
-        
-        ## Contributing
-        
-        See the file [CONTRIBUTING.md](https://github.com/adamrehn/ue4-docker/blob/master/.github/CONTRIBUTING.md) for guidelines on how to contribute to the development of ue4-docker.
-        
-        
-        ## Legal
-        
-        Copyright &copy; 2018 - 2021, Adam Rehn. Licensed under the MIT License, see the file [LICENSE](https://github.com/adamrehn/ue4-docker/blob/master/LICENSE) for details.
-        
-        Unreal and its logo are Epic Games' trademarks or registered trademarks in the US and elsewhere.
-        
-        Docker and the Docker logo are trademarks or registered trademarks of Docker in the United States and other countries.
-        
 Keywords: epic unreal engine docker
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Console
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center"><img src="https://raw.githubusercontent.com/adamrehn/ue4-docker/master/resources/images/banner.svg?sanitize=true" alt="Unreal Engine and Docker Logos" height="100"></p>
+<h1 align="center"><strong>Unreal Engine 4 Docker Containers</strong></h1>
+<h3 align="center"><a href="https://docs.adamrehn.com/ue4-docker/use-cases/continuous-integration">Continuous Integration</a> &bull; <a href="https://docs.adamrehn.com/ue4-docker/use-cases/cloud-rendering">Cloud Rendering</a> &bull; <a href="https://docs.adamrehn.com/ue4-docker/use-cases/microservices">UE4-Powered Microservices</a></h3>
+<p>&nbsp;</p>
+
+**Looking for a place to start? Check out the [Unreal Containers community hub](https://unrealcontainers.com/) for implementation-agnostic information on using the Unreal Engine inside Docker containers, and then head to the [comprehensive ue4-docker documentation](https://docs.adamrehn.com/ue4-docker/) to view details specific to using the ue4-docker project.**
+
+The ue4-docker Python package contains a set of Dockerfiles and accompanying build infrastructure that allows you to build Docker images for Epic Games' [Unreal Engine 4](https://www.unrealengine.com/). The images also incorporate the infrastructure from [ue4cli](https://github.com/adamrehn/ue4cli), [conan-ue4cli](https://github.com/adamrehn/conan-ue4cli), and [ue4-ci-helpers](https://github.com/adamrehn/ue4-ci-helpers) to facilitate a wide variety of use cases.
+
+Key features include:
+
+- Unreal Engine 4.20.0 and newer is supported.
+- Both Windows containers and Linux containers are supported.
+- Building and packaging UE4 projects is supported.
+- Running automation tests is supported.
+- Running built UE4 projects with offscreen rendering is supported via NVIDIA Docker under Linux.
+
+Resources:
+
+- **Documentation:** <https://docs.adamrehn.com/ue4-docker/>
+- **GitHub repository:** <https://github.com/adamrehn/ue4-docker>
+- **Package on PyPI:** <https://pypi.org/project/ue4-docker/>
+- **Related articles:** <https://adamrehn.com/articles/tag/Unreal%20Engine/>
+- **Unreal Containers community hub:** <https://unrealcontainers.com/>
+- **Development channel on the Unreal Containers Community Discord server**: <https://discord.gg/46CJg9fyJ9>
+
+
+## Contributing
+
+See the file [CONTRIBUTING.md](https://github.com/adamrehn/ue4-docker/blob/master/.github/CONTRIBUTING.md) for guidelines on how to contribute to the development of ue4-docker.
+
+
+## Legal
+
+Copyright &copy; 2018 - 2021, Adam Rehn. Licensed under the MIT License, see the file [LICENSE](https://github.com/adamrehn/ue4-docker/blob/master/LICENSE) for details.
+
+Unreal and its logo are Epic Games' trademarks or registered trademarks in the US and elsewhere.
+
+Docker and the Docker logo are trademarks or registered trademarks of Docker in the United States and other countries.
+
+
```

#### html2text {}

```diff
@@ -1,11 +1,17 @@
-Metadata-Version: 2.1 Name: ue4-docker Version: 0.0.98 Summary: Windows and
+Metadata-Version: 2.1 Name: ue4-docker Version: 0.0.99 Summary: Windows and
 Linux containers for Unreal Engine 4 Home-page: http://github.com/adamrehn/ue4-
-docker Author: Adam Rehn Author-email: adam@adamrehn.com License: MIT
-Description:
+docker Author: Adam Rehn Author-email: adam@adamrehn.com License: MIT Keywords:
+epic unreal engine docker Platform: UNKNOWN Classifier: License :: OSI Approved
+:: MIT License Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Software
+Development :: Build Tools Classifier: Environment :: Console Requires-Python:
+>=3.6 Description-Content-Type: text/markdown License-File: LICENSE
                        [Unreal Engine and Docker Logos]
                 ****** Unreal Engine 4 Docker Containers ******
 **** Continuous_Integration • Cloud_Rendering • UE4-Powered_Microservices ****
  
 **Looking for a place to start? Check out the [Unreal Containers community hub]
 (https://unrealcontainers.com/) for implementation-agnostic information on
 using the Unreal Engine inside Docker containers, and then head to the
@@ -33,12 +39,7 @@
 github.com/adamrehn/ue4-docker/blob/master/.github/CONTRIBUTING.md) for
 guidelines on how to contribute to the development of ue4-docker. ## Legal
 Copyright © 2018 - 2021, Adam Rehn. Licensed under the MIT License, see the
 file [LICENSE](https://github.com/adamrehn/ue4-docker/blob/master/LICENSE) for
 details. Unreal and its logo are Epic Games' trademarks or registered
 trademarks in the US and elsewhere. Docker and the Docker logo are trademarks
 or registered trademarks of Docker in the United States and other countries.
-Keywords: epic unreal engine docker Platform: UNKNOWN Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Topic :: Software
-Development :: Build Tools Classifier: Environment :: Console Requires-Python:
->=3.6 Description-Content-Type: text/markdown
```

### Comparing `ue4-docker-0.0.98/README.md` & `ue4-docker-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/setup.py` & `ue4-docker-0.0.99/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     description="Windows and Linux containers for Unreal Engine 4",
     long_description=__readme__,
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Build Tools",
         "Environment :: Console",
     ],
     keywords="epic unreal engine docker",
     url="http://github.com/adamrehn/ue4-docker",
     author="Adam Rehn",
     author_email="adam@adamrehn.com",
@@ -43,15 +46,18 @@
         "docker>=3.0.0",
         "humanfriendly",
         "Jinja2>=2.11.3",
         "packaging>=19.1",
         "psutil",
         "requests",
         "semver>=2.7.9,<3.0.0",
-        "setuptools>=60.4.0",
+        # We want newer setuptools to avoid shim path bug on newer Pythons.
+        # See #231 and https://github.com/pypa/setuptools/issues/3001
+        # Unfortunately, that version of setuptools doesn't have Python 3.6 support
+        "setuptools>=60.4.0;python_version>='3.7.0'",
         "termcolor",
         "twine>=1.11.0",
         "wheel>=0.31.0",
     ],
     package_data={
         "ue4docker": [
             "dockerfiles/*/*/.dockerignore",
```

### Comparing `ue4-docker-0.0.98/ue4_docker.egg-info/PKG-INFO` & `ue4-docker-0.0.99/ue4_docker.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 Metadata-Version: 2.1
 Name: ue4-docker
-Version: 0.0.98
+Version: 0.0.99
 Summary: Windows and Linux containers for Unreal Engine 4
 Home-page: http://github.com/adamrehn/ue4-docker
 Author: Adam Rehn
 Author-email: adam@adamrehn.com
 License: MIT
-Description: <p align="center"><img src="https://raw.githubusercontent.com/adamrehn/ue4-docker/master/resources/images/banner.svg?sanitize=true" alt="Unreal Engine and Docker Logos" height="100"></p>
-        <h1 align="center"><strong>Unreal Engine 4 Docker Containers</strong></h1>
-        <h3 align="center"><a href="https://docs.adamrehn.com/ue4-docker/use-cases/continuous-integration">Continuous Integration</a> &bull; <a href="https://docs.adamrehn.com/ue4-docker/use-cases/cloud-rendering">Cloud Rendering</a> &bull; <a href="https://docs.adamrehn.com/ue4-docker/use-cases/microservices">UE4-Powered Microservices</a></h3>
-        <p>&nbsp;</p>
-        
-        **Looking for a place to start? Check out the [Unreal Containers community hub](https://unrealcontainers.com/) for implementation-agnostic information on using the Unreal Engine inside Docker containers, and then head to the [comprehensive ue4-docker documentation](https://docs.adamrehn.com/ue4-docker/) to view details specific to using the ue4-docker project.**
-        
-        The ue4-docker Python package contains a set of Dockerfiles and accompanying build infrastructure that allows you to build Docker images for Epic Games' [Unreal Engine 4](https://www.unrealengine.com/). The images also incorporate the infrastructure from [ue4cli](https://github.com/adamrehn/ue4cli), [conan-ue4cli](https://github.com/adamrehn/conan-ue4cli), and [ue4-ci-helpers](https://github.com/adamrehn/ue4-ci-helpers) to facilitate a wide variety of use cases.
-        
-        Key features include:
-        
-        - Unreal Engine 4.20.0 and newer is supported.
-        - Both Windows containers and Linux containers are supported.
-        - Building and packaging UE4 projects is supported.
-        - Running automation tests is supported.
-        - Running built UE4 projects with offscreen rendering is supported via NVIDIA Docker under Linux.
-        
-        Resources:
-        
-        - **Documentation:** <https://docs.adamrehn.com/ue4-docker/>
-        - **GitHub repository:** <https://github.com/adamrehn/ue4-docker>
-        - **Package on PyPI:** <https://pypi.org/project/ue4-docker/>
-        - **Related articles:** <https://adamrehn.com/articles/tag/Unreal%20Engine/>
-        - **Unreal Containers community hub:** <https://unrealcontainers.com/>
-        - **Development channel on the Unreal Containers Community Discord server**: <https://discord.gg/46CJg9fyJ9>
-        
-        
-        ## Contributing
-        
-        See the file [CONTRIBUTING.md](https://github.com/adamrehn/ue4-docker/blob/master/.github/CONTRIBUTING.md) for guidelines on how to contribute to the development of ue4-docker.
-        
-        
-        ## Legal
-        
-        Copyright &copy; 2018 - 2021, Adam Rehn. Licensed under the MIT License, see the file [LICENSE](https://github.com/adamrehn/ue4-docker/blob/master/LICENSE) for details.
-        
-        Unreal and its logo are Epic Games' trademarks or registered trademarks in the US and elsewhere.
-        
-        Docker and the Docker logo are trademarks or registered trademarks of Docker in the United States and other countries.
-        
 Keywords: epic unreal engine docker
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Console
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center"><img src="https://raw.githubusercontent.com/adamrehn/ue4-docker/master/resources/images/banner.svg?sanitize=true" alt="Unreal Engine and Docker Logos" height="100"></p>
+<h1 align="center"><strong>Unreal Engine 4 Docker Containers</strong></h1>
+<h3 align="center"><a href="https://docs.adamrehn.com/ue4-docker/use-cases/continuous-integration">Continuous Integration</a> &bull; <a href="https://docs.adamrehn.com/ue4-docker/use-cases/cloud-rendering">Cloud Rendering</a> &bull; <a href="https://docs.adamrehn.com/ue4-docker/use-cases/microservices">UE4-Powered Microservices</a></h3>
+<p>&nbsp;</p>
+
+**Looking for a place to start? Check out the [Unreal Containers community hub](https://unrealcontainers.com/) for implementation-agnostic information on using the Unreal Engine inside Docker containers, and then head to the [comprehensive ue4-docker documentation](https://docs.adamrehn.com/ue4-docker/) to view details specific to using the ue4-docker project.**
+
+The ue4-docker Python package contains a set of Dockerfiles and accompanying build infrastructure that allows you to build Docker images for Epic Games' [Unreal Engine 4](https://www.unrealengine.com/). The images also incorporate the infrastructure from [ue4cli](https://github.com/adamrehn/ue4cli), [conan-ue4cli](https://github.com/adamrehn/conan-ue4cli), and [ue4-ci-helpers](https://github.com/adamrehn/ue4-ci-helpers) to facilitate a wide variety of use cases.
+
+Key features include:
+
+- Unreal Engine 4.20.0 and newer is supported.
+- Both Windows containers and Linux containers are supported.
+- Building and packaging UE4 projects is supported.
+- Running automation tests is supported.
+- Running built UE4 projects with offscreen rendering is supported via NVIDIA Docker under Linux.
+
+Resources:
+
+- **Documentation:** <https://docs.adamrehn.com/ue4-docker/>
+- **GitHub repository:** <https://github.com/adamrehn/ue4-docker>
+- **Package on PyPI:** <https://pypi.org/project/ue4-docker/>
+- **Related articles:** <https://adamrehn.com/articles/tag/Unreal%20Engine/>
+- **Unreal Containers community hub:** <https://unrealcontainers.com/>
+- **Development channel on the Unreal Containers Community Discord server**: <https://discord.gg/46CJg9fyJ9>
+
+
+## Contributing
+
+See the file [CONTRIBUTING.md](https://github.com/adamrehn/ue4-docker/blob/master/.github/CONTRIBUTING.md) for guidelines on how to contribute to the development of ue4-docker.
+
+
+## Legal
+
+Copyright &copy; 2018 - 2021, Adam Rehn. Licensed under the MIT License, see the file [LICENSE](https://github.com/adamrehn/ue4-docker/blob/master/LICENSE) for details.
+
+Unreal and its logo are Epic Games' trademarks or registered trademarks in the US and elsewhere.
+
+Docker and the Docker logo are trademarks or registered trademarks of Docker in the United States and other countries.
+
+
```

#### html2text {}

```diff
@@ -1,11 +1,17 @@
-Metadata-Version: 2.1 Name: ue4-docker Version: 0.0.98 Summary: Windows and
+Metadata-Version: 2.1 Name: ue4-docker Version: 0.0.99 Summary: Windows and
 Linux containers for Unreal Engine 4 Home-page: http://github.com/adamrehn/ue4-
-docker Author: Adam Rehn Author-email: adam@adamrehn.com License: MIT
-Description:
+docker Author: Adam Rehn Author-email: adam@adamrehn.com License: MIT Keywords:
+epic unreal engine docker Platform: UNKNOWN Classifier: License :: OSI Approved
+:: MIT License Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Software
+Development :: Build Tools Classifier: Environment :: Console Requires-Python:
+>=3.6 Description-Content-Type: text/markdown License-File: LICENSE
                        [Unreal Engine and Docker Logos]
                 ****** Unreal Engine 4 Docker Containers ******
 **** Continuous_Integration • Cloud_Rendering • UE4-Powered_Microservices ****
  
 **Looking for a place to start? Check out the [Unreal Containers community hub]
 (https://unrealcontainers.com/) for implementation-agnostic information on
 using the Unreal Engine inside Docker containers, and then head to the
@@ -33,12 +39,7 @@
 github.com/adamrehn/ue4-docker/blob/master/.github/CONTRIBUTING.md) for
 guidelines on how to contribute to the development of ue4-docker. ## Legal
 Copyright © 2018 - 2021, Adam Rehn. Licensed under the MIT License, see the
 file [LICENSE](https://github.com/adamrehn/ue4-docker/blob/master/LICENSE) for
 details. Unreal and its logo are Epic Games' trademarks or registered
 trademarks in the US and elsewhere. Docker and the Docker logo are trademarks
 or registered trademarks of Docker in the United States and other countries.
-Keywords: epic unreal engine docker Platform: UNKNOWN Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Topic :: Software
-Development :: Build Tools Classifier: Environment :: Console Requires-Python:
->=3.6 Description-Content-Type: text/markdown
```

### Comparing `ue4-docker-0.0.98/ue4_docker.egg-info/SOURCES.txt` & `ue4-docker-0.0.99/ue4_docker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 ue4_docker.egg-info/PKG-INFO
 ue4_docker.egg-info/SOURCES.txt
 ue4_docker.egg-info/dependency_links.txt
 ue4_docker.egg-info/entry_points.txt
 ue4_docker.egg-info/not-zip-safe
@@ -20,15 +21,14 @@
 ue4docker/version.py
 ue4docker/version_cmd.py
 ue4docker/diagnostics/__init__.py
 ue4docker/diagnostics/base.py
 ue4docker/diagnostics/diagnostic_20gig.py
 ue4docker/diagnostics/diagnostic_8gig.py
 ue4docker/diagnostics/diagnostic_all.py
-ue4docker/diagnostics/diagnostic_maxsize.py
 ue4docker/diagnostics/diagnostic_network.py
 ue4docker/dockerfiles/diagnostics/20gig/windows/Dockerfile
 ue4docker/dockerfiles/diagnostics/8gig/linux/Dockerfile
 ue4docker/dockerfiles/diagnostics/8gig/windows/Dockerfile
 ue4docker/dockerfiles/diagnostics/8gig/windows/test.ps1
 ue4docker/dockerfiles/diagnostics/network/linux/Dockerfile
 ue4docker/dockerfiles/diagnostics/network/windows/Dockerfile
```

### Comparing `ue4-docker-0.0.98/ue4docker/build.py` & `ue4-docker-0.0.99/ue4docker/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,22 +84,19 @@
                 False,
             )
             sys.exit(1)
 
     # Create an auto-deleting temporary directory to hold our build context
     with tempfile.TemporaryDirectory() as tempDir:
 
-        # Copy our Dockerfiles to the temporary directory
         contextOrig = join(os.path.dirname(os.path.abspath(__file__)), "dockerfiles")
-        contextRoot = join(tempDir, "dockerfiles")
-        shutil.copytree(contextOrig, contextRoot)
 
         # Create the builder instance to build the Docker images
         builder = ImageBuilder(
-            contextRoot,
+            join(tempDir, "dockerfiles"),
             config.containerPlatform,
             logger,
             config.rebuild,
             config.dryRun,
             config.layoutDir,
             config.opts,
             config.combine,
@@ -233,15 +230,15 @@
             )
             if newer_check:
                 logger.error(
                     "Error: cannot build container images with a newer kernel version than that of the host OS!"
                 )
                 sys.exit(1)
             elif newer_check is None:
-                logger.info(
+                logger.warning(
                     "Warning: unable to determine whether host system is new enough to use specified base tag"
                 )
 
             # Ensure the Docker daemon is configured correctly
             requiredLimit = WindowsUtils.requiredSizeLimit()
             if DockerUtils.maxsize() < requiredLimit and config.buildTargets["source"]:
                 logger.error("SETUP REQUIRED:")
@@ -379,25 +376,45 @@
                     prereqsArgs = prereqsArgs + [
                         "--build-arg",
                         "DLLSRCIMAGE=" + config.dllSrcImage,
                         "--build-arg",
                         "VISUAL_STUDIO_BUILD_NUMBER=" + config.visualStudioBuildNumber,
                     ]
 
-                builder.build(
-                    "ue4-build-prerequisites",
-                    [config.prereqsTag],
-                    commonArgs + config.platformArgs + prereqsArgs,
-                )
-                builtImages.append("ue4-build-prerequisites")
+                custom_prerequisites_dockerfile = config.args.prerequisites_dockerfile
+                if custom_prerequisites_dockerfile is not None:
+                    builder.build_builtin_image(
+                        "ue4-base-build-prerequisites",
+                        [config.prereqsTag],
+                        commonArgs + config.platformArgs + prereqsArgs,
+                        builtin_name="ue4-build-prerequisites",
+                    )
+                    builtImages.append("ue4-base-build-prerequisites")
+                else:
+                    builder.build_builtin_image(
+                        "ue4-build-prerequisites",
+                        [config.prereqsTag],
+                        commonArgs + config.platformArgs + prereqsArgs,
+                    )
 
                 prereqConsumerArgs = [
                     "--build-arg",
                     "PREREQS_TAG={}".format(config.prereqsTag),
                 ]
+
+                if custom_prerequisites_dockerfile is not None:
+                    builder.build(
+                        "ue4-build-prerequisites",
+                        [config.prereqsTag],
+                        commonArgs + config.platformArgs + prereqConsumerArgs,
+                        dockerfile_template=custom_prerequisites_dockerfile,
+                        context_dir=os.path.dirname(custom_prerequisites_dockerfile),
+                    )
+
+                builtImages.append("ue4-build-prerequisites")
             else:
                 logger.info("Skipping ue4-build-prerequisities image build.")
 
             # Build the UE4 source image
             if config.buildTargets["source"]:
                 # Start the HTTP credential endpoint as a child process and wait for it to start
                 if config.opts.get("credential_mode", "endpoint") == "endpoint":
@@ -414,33 +431,33 @@
                     "--build-arg",
                     "GIT_REPO={}".format(config.repository),
                     "--build-arg",
                     "GIT_BRANCH={}".format(config.branch),
                     "--build-arg",
                     "VERBOSE_OUTPUT={}".format("1" if config.verbose == True else "0"),
                 ]
-                builder.build(
+                builder.build_builtin_image(
                     "ue4-source",
                     mainTags,
                     commonArgs + config.platformArgs + ue4SourceArgs + credentialArgs,
-                    secrets,
+                    secrets=secrets,
                 )
                 builtImages.append("ue4-source")
             else:
                 logger.info("Skipping ue4-source image build.")
 
             if config.buildTargets["engine"] or config.buildTargets["minimal"]:
                 ue4BuildArgs = prereqConsumerArgs + [
                     "--build-arg",
                     "TAG={}".format(mainTags[1]),
                 ]
 
             # Build the UE4 Engine source build image, unless requested otherwise by the user
             if config.buildTargets["engine"]:
-                builder.build(
+                builder.build_builtin_image(
                     "ue4-engine",
                     mainTags,
                     commonArgs + config.platformArgs + ue4BuildArgs,
                 )
                 builtImages.append("ue4-engine")
             else:
                 logger.info("Skipping ue4-engine image build.")
@@ -449,15 +466,15 @@
             if config.buildTargets["minimal"]:
                 minimalArgs = (
                     ["--build-arg", "CHANGELIST={}".format(config.changelist)]
                     if config.changelist is not None
                     else []
                 )
 
-                builder.build(
+                builder.build_builtin_image(
                     "ue4-minimal",
                     mainTags,
                     commonArgs + config.platformArgs + ue4BuildArgs + minimalArgs,
                 )
                 builtImages.append("ue4-minimal")
             else:
                 logger.info("Skipping ue4-minimal image build.")
@@ -479,15 +496,15 @@
                         [
                             "--build-arg",
                             "CONAN_UE4CLI_VERSION={}".format(config.conanUe4cliVersion),
                         ]
                     )
 
                 # Build the image
-                builder.build(
+                builder.build_builtin_image(
                     "ue4-full",
                     mainTags,
                     commonArgs
                     + config.platformArgs
                     + ue4BuildArgs
                     + infrastructureFlags,
                 )
```

### Comparing `ue4-docker-0.0.98/ue4docker/clean.py` & `ue4-docker-0.0.99/ue4docker/clean.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/diagnostics/base.py` & `ue4-docker-0.0.99/ue4docker/diagnostics/base.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/diagnostics/diagnostic_20gig.py` & `ue4-docker-0.0.99/ue4docker/diagnostics/diagnostic_20gig.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,17 +36,16 @@
     def getDescription(self):
         """
         Returns a description of what the diagnostic does
         """
         return "\n".join(
             [
                 "This diagnostic determines if the Docker daemon suffers from 20GiB COPY bug",
-                "reported at https://github.com/moby/moby/issues/37352 (affects Windows containers only)",
                 "",
-                "#37352 was fixed in https://github.com/moby/moby/pull/41636 but that fix was not released yet",
+                "See https://github.com/adamrehn/ue4-docker/issues/99#issuecomment-1079702817 for details and workarounds",
                 "",
                 self._parser.format_help(),
             ]
         )
 
     def getPrefix(self):
         """
```

### Comparing `ue4-docker-0.0.98/ue4docker/diagnostics/diagnostic_8gig.py` & `ue4-docker-0.0.99/ue4docker/diagnostics/diagnostic_8gig.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/diagnostics/diagnostic_all.py` & `ue4-docker-0.0.99/ue4docker/diagnostics/diagnostic_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from .base import DiagnosticBase
 from .diagnostic_8gig import diagnostic8Gig
 from .diagnostic_20gig import diagnostic20Gig
-from .diagnostic_maxsize import diagnosticMaxSize
 from .diagnostic_network import diagnosticNetwork
 
 
 class allDiagnostics(DiagnosticBase):
     def getName(self):
         """
         Returns the human-readable name of the diagnostic
@@ -24,15 +23,14 @@
         """
 
         # Run all available diagnostics in turn, storing the results
         results = []
         diagnostics = [
             diagnostic8Gig(),
             diagnostic20Gig(),
-            diagnosticMaxSize(),
             diagnosticNetwork(),
         ]
         for index, diagnostic in enumerate(diagnostics):
 
             # Run the diagnostic and report its result
             logger.info(
                 '[all] Running individual diagnostic: "{}"'.format(
```

### Comparing `ue4-docker-0.0.98/ue4docker/diagnostics/diagnostic_network.py` & `ue4-docker-0.0.99/ue4docker/diagnostics/diagnostic_network.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/diagnostics_cmd.py` & `ue4-docker-0.0.99/ue4docker/diagnostics_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 def diagnostics():
 
     # The diagnostics that can be run
     DIAGNOSTICS = {
         "all": allDiagnostics(),
         "8gig": diagnostic8Gig(),
         "20gig": diagnostic20Gig(),
-        "maxsize": diagnosticMaxSize(),
         "network": diagnosticNetwork(),
     }
 
     # Create our logger to generate coloured output on stderr
     logger = Logger(prefix="[{} diagnostics] ".format(sys.argv[0]))
 
     # Parse the supplied command-line arguments
```

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/20gig/windows/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/20gig/windows/Dockerfile`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/8gig/windows/test.ps1` & `ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/8gig/windows/test.ps1`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/diagnostics/network/windows/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/diagnostics/network/windows/Dockerfile`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/linux/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/linux/Dockerfile`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/windows/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/windows/Dockerfile`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-build-prerequisites/windows/install-prerequisites.bat` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-build-prerequisites/windows/install-prerequisites.bat`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 @rem Install the chocolatey packages we need
 choco install -y git --params "'/GitOnlyOnPath /NoAutoCrlf /WindowsTerminal /NoShellIntegration /NoCredentialManager'" || goto :error
 @rem pdbcopy.exe from Windows SDK is needed for creating an Installed Build of the Engine
-choco install -y choco-cleaner curl vcredist-all windows-sdk-10-version-1809-windbg || goto :error
-choco install -y python --version=3.7.5 || goto :error
+choco install -y choco-cleaner python vcredist-all windows-sdk-10-version-1809-windbg || goto :error
 
 @rem Reload our environment variables from the registry so the `git` command works
 call refreshenv
 @echo on
 
 @rem Forcibly disable the git credential manager
 git config --system credential.helper "" || goto :error
@@ -53,32 +52,33 @@
 if "%VISUAL_STUDIO_BUILD_NUMBER%" == "15" (
     set WINDOWS_SDK_VERSION=17763
 ) else (
     set WINDOWS_SDK_VERSION=20348
 )
 
 @rem Install the Visual Studio Build Tools workloads and components we need
-@rem NOTE: We use the Visual Studio 2019 installer even for Visual Studio 2017 here because the old installer now breaks
-@rem NOTE: VS2019 Build Tools doesn't have 4.6.2 .NET SDK and what actually gets installed is 4.8
-@rem NOTE: Microsoft.NetCore.Component.SDK only exists for VS2019. And it is actually *needed* only for UE5
-curl --progress-bar -L "https://aka.ms/vs/16/release/vs_buildtools.exe" --output %TEMP%\vs_buildtools.exe || goto :error
+@rem NOTE: We use the Visual Studio 2022 installer even for Visual Studio 2019 and 2017 here because the old (2017) installer now breaks
+@rem NOTE: Microsoft.NetCore.Component.SDK only exists for VS2019+. And it is actually *needed* only for UE5
+@rem NOTE: .NET 4.5 is required for some programs even in UE5, for example https://github.com/EpicGames/UnrealEngine/blob/5.0.1-release/Engine/Source/Programs/UnrealSwarm/SwarmCoordinator/SwarmCoordinator.csproj#L26
+curl --progress-bar -L "https://aka.ms/vs/17/release/vs_buildtools.exe" --output %TEMP%\vs_buildtools.exe || goto :error
 %TEMP%\vs_buildtools.exe --quiet --wait --norestart --nocache ^
 	--installPath C:\BuildTools ^
 	--channelUri "https://aka.ms/vs/%VISUAL_STUDIO_BUILD_NUMBER%/release/channel" ^
 	--installChannelUri "https://aka.ms/vs/%VISUAL_STUDIO_BUILD_NUMBER%/release/channel" ^
 	--channelId VisualStudio.%VISUAL_STUDIO_BUILD_NUMBER%.Release ^
 	--productId Microsoft.VisualStudio.Product.BuildTools ^
 	--locale en-US ^
 	--add Microsoft.VisualStudio.Workload.VCTools ^
 	--add Microsoft.VisualStudio.Workload.MSBuildTools ^
 	--add Microsoft.VisualStudio.Component.NuGet ^
 	--add Microsoft.VisualStudio.Component.VC.Tools.x86.x64 ^
 	--add Microsoft.VisualStudio.Component.Windows10SDK.%WINDOWS_SDK_VERSION% ^
 	--add Microsoft.Net.Component.4.5.TargetingPack ^
-	--add Microsoft.Net.ComponentGroup.4.6.2.DeveloperTools ^
+	--add Microsoft.Net.Component.4.6.2.TargetingPack ^
+	--add Microsoft.Net.ComponentGroup.DevelopmentPrerequisites ^
 	--add Microsoft.NetCore.Component.SDK
 
 python C:\buildtools-exitcode.py %ERRORLEVEL% || goto :error
 
 @rem Clean up any temp files generated during prerequisite installation
 rmdir /S /Q \\?\%TEMP%
 mkdir %TEMP%
```

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-full/linux/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-full/linux/Dockerfile`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-full/windows/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-full/windows/Dockerfile`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -27,24 +27,26 @@
 
 # Patch the default settings in InstalledEngineBuild.xml and increase the output verbosity of the DDC generation step
 COPY patch-build-graph.py /tmp/patch-build-graph.py
 RUN python3 /tmp/patch-build-graph.py /home/ue4/UnrealEngine/Engine/Build/InstalledEngineBuild.xml /home/ue4/UnrealEngine/Engine/Build/Build.version
 {% endif %}
 
 # Ensure UBT is built before we create the Installed Build, since Build.sh explicitly sets the
-# target .NET framework version, whereas InstalledEngineBuild.xml just uses the system default,
+# target .NET Framework version, whereas InstalledEngineBuild.xml just uses the system default,
 # which can result in errors when running the built UBT due to the wrong version being targeted
-RUN ./Engine/Build/BatchFiles/Linux/Build.sh UnrealHeaderTool Linux Development -SkipBuild
+RUN ./Engine/Build/BatchFiles/Linux/Build.sh UnrealHeaderTool Linux Development -SkipBuild -buildubt
 
 # Create an Installed Build of the Engine
 WORKDIR /home/ue4/UnrealEngine
 RUN ./Engine/Build/BatchFiles/RunUAT.sh BuildGraph \
     -target="Make Installed Build Linux" \
     -script=Engine/Build/InstalledEngineBuild.xml \
-    -set:WithDDC={% if excluded_components.ddc == true %}false{% else %}true{% endif %} {{ buildgraph_args }} && \
+    -set:HostPlatformOnly=true \
+    -set:WithDDC={% if excluded_components.ddc == true %}false{% else %}true{% endif %} \
+    {{ buildgraph_args }} && \
 	rm -R -f /home/ue4/UnrealEngine/LocalBuilds/InstalledDDC
 
 # Split out components (DDC, debug symbols, template projects) so they can be copied into the final container image as separate filesystem layers
 COPY split-components.py /tmp/split-components.py
 RUN python3 /tmp/split-components.py /home/ue4/UnrealEngine/LocalBuilds/Engine/Linux /home/ue4/UnrealEngine/Components
 
 {% if (not disable_all_patches) and (not disable_target_patches) %}
```

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/copy-toolchain.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/copy-toolchain.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/fix-targets.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/fix-targets.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/patch-build-graph.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/patch-build-graph.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/patch-filters-xml.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/patch-filters-xml.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/set-changelist.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/set-changelist.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/linux/split-components.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/linux/split-components.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 {% endif %}
 
 # Create an Installed Build of the Engine
 WORKDIR C:\UnrealEngine
 RUN .\Engine\Build\BatchFiles\RunUAT.bat BuildGraph `
     -target="Make Installed Build Win64" `
     -script=Engine/Build/InstalledEngineBuild.xml `
+    -set:HostPlatformOnly=true `
     -set:WithDDC={% if excluded_components.ddc == true %}false{% else %}true{% endif %} `
     {{ buildgraph_args }} && `
 	(if exist C:\UnrealEngine\LocalBuilds\InstalledDDC rmdir /s /q C:\UnrealEngine\LocalBuilds\InstalledDDC)
 
 # Split out components (DDC, debug symbols, template projects) so they can be copied into the final container image as separate filesystem layers
 COPY split-components.py C:\split-components.py
 RUN python C:\split-components.py C:\UnrealEngine\LocalBuilds\Engine\Windows C:\UnrealEngine\Components
```

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/fix-targets.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/fix-targets.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/patch-build-graph.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/patch-build-graph.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/patch-filters-xml.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/patch-filters-xml.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/set-changelist.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/set-changelist.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-minimal/windows/split-components.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-minimal/windows/split-components.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/Dockerfile`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/linker-fixup.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/linker-fixup.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/patch-broken-releases.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/patch-broken-releases.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/linux/patch-ubt.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/linux/patch-ubt.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/Dockerfile` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/Dockerfile`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/patch-broken-releases.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/patch-broken-releases.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/patch-setup-win.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/patch-setup-win.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/dockerfiles/ue4-source/windows/patch-ubt.py` & `ue4-docker-0.0.99/ue4docker/dockerfiles/ue4-source/windows/patch-ubt.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/export.py` & `ue4-docker-0.0.99/ue4docker/export.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/exports/export_installed.py` & `ue4-docker-0.0.99/ue4docker/exports/export_installed.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/exports/export_packages.py` & `ue4-docker-0.0.99/ue4docker/exports/export_packages.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/info.py` & `ue4-docker-0.0.99/ue4docker/info.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/BuildConfiguration.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/BuildConfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,33 +33,37 @@
     "4.21.0": 4541578,
     "4.22.0": 5660361,
     "4.23.0": 8386587,
     "4.24.0": 10570792,
     "4.25.0": 13144385,
     "4.26.0": 14830424,
     "4.27.0": 17155196,
+    "5.0.0": 19505902,
 }
 
 
 class VisualStudio(object):
     VS2017 = "2017"
     VS2019 = "2019"
+    VS2022 = "2022"
 
     BuildNumbers = {
         VS2017: "15",
         VS2019: "16",
+        VS2022: "17",
     }
 
     MinSupportedUnreal = {
         # Unreal Engine 4.23.1 is the first that successfully builds with Visual Studio v16.3
         # See https://github.com/EpicGames/UnrealEngine/commit/2510d4fd07a35ba5bff6ac2c7becaa6e8b7f11fa
         #
         # Unreal Engine 4.25 is the first that works with .NET SDK 4.7+
         # See https://github.com/EpicGames/UnrealEngine/commit/5256eedbdef30212ab69fdf4c09e898098959683
-        VS2019: semver.VersionInfo(4, 25)
+        VS2019: semver.VersionInfo(4, 25),
+        VS2022: semver.VersionInfo(4, 27),
     }
 
 
 class ExcludedComponent(object):
     """
     The different components that we support excluding from the built images
     """
@@ -256,14 +260,19 @@
         )
         parser.add_argument(
             "-changelist",
             type=int,
             default=None,
             help="Set a specific changelist number in the Unreal Engine's Build.version file",
         )
+        parser.add_argument(
+            "--prerequisites-dockerfile",
+            default=None,
+            help="Specifies path to custom ue4-build-prerequisites dockerfile",
+        )
 
     def __init__(self, parser, argv, logger):
         """
         Creates a new build configuration based on the supplied arguments object
         """
 
         # If the user has specified `--cuda` without a version value, treat the value as an empty string
@@ -466,15 +475,15 @@
         # If the user specified custom version strings for ue4cli and/or conan-ue4cli, process them
         self.ue4cliVersion = self._processPackageVersion("ue4cli", self.args.ue4cli)
         self.conanUe4cliVersion = self._processPackageVersion(
             "conan-ue4cli", self.args.conan_ue4cli
         )
 
         # Process any specified advanced configuration options (which we use directly as context values for the Jinja templating system)
-        self.opts = {"buildgraph_args": "-set:HostPlatformOnly=true"}
+        self.opts = {}
         for o in self.args.opt:
             if "=" in o:
                 key, value = o.split("=", 1)
                 self.opts[key.replace("-", "_")] = self._processTemplateValue(value)
             else:
                 self.opts[o.replace("-", "_")] = True
 
@@ -523,14 +532,41 @@
         # Generate Jinja context values for keeping or excluding components
         self.opts["excluded_components"] = {
             "ddc": ExcludedComponent.DDC in self.excludedComponents,
             "debug": ExcludedComponent.Debug in self.excludedComponents,
             "templates": ExcludedComponent.Templates in self.excludedComponents,
         }
 
+        # Warn user that they are in danger of Docker 20GB COPY bug
+        # Unfortunately, we don't have a cheap way to check whether user environment is affected
+        # See https://github.com/adamrehn/ue4-docker/issues/99
+        if self.containerPlatform == "windows":
+            warn20GiB = False
+            if ExcludedComponent.Debug not in self.excludedComponents:
+                logger.warning("Warning: You didn't pass --exclude debug", False)
+                warn20GiB = True
+            if (
+                self.release
+                and not self.custom
+                and semver.VersionInfo.parse(self.release) >= semver.VersionInfo(5, 0)
+            ):
+                logger.warning("Warning: You're building Unreal Engine 5", False)
+                warn20GiB = True
+
+            if warn20GiB:
+                logger.warning("Warning: You might hit Docker 20GiB COPY bug", False)
+                logger.warning(
+                    "Warning: Make sure that `ue4-docker diagnostics 20gig` passes",
+                    False,
+                )
+                logger.warning(
+                    "Warning: See https://github.com/adamrehn/ue4-docker/issues/99#issuecomment-1079702817 for details and workarounds",
+                    False,
+                )
+
         # If we're building Windows containers, generate our Windows-specific configuration settings
         if self.containerPlatform == "windows":
             self._generateWindowsConfig()
 
         # If we're building Linux containers, generate our Linux-specific configuration settings
         if self.containerPlatform == "linux":
             self._generateLinuxConfig()
@@ -568,15 +604,18 @@
                 )
 
         self.visualStudioBuildNumber = VisualStudio.BuildNumbers[self.visualStudio]
         # See https://github.com/EpicGames/UnrealEngine/commit/72585138472785e2ee58aab9950a7260275ee2ac
         # Note: We must not pass VS2019 arg for older UE4 versions that didn't have VS2019 variable in their build graph xml.
         # Otherwise, UAT errors out with "Unknown argument: VS2019".
         if self.visualStudio != VisualStudio.VS2017:
-            self.opts["buildgraph_args"] += f" -set:VS{self.visualStudio}=true"
+            self.opts["buildgraph_args"] = (
+                self.opts.get("buildgraph_args", "")
+                + f" -set:VS{self.visualStudio}=true"
+            )
 
         # Determine base tag for the Windows release of the host system
         self.hostBasetag = WindowsUtils.getHostBaseTag()
 
         # Store the tag for the base Windows Server Core image
         self.basetag = (
             self.args.basetag if self.args.basetag is not None else self.hostBasetag
```

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/CredentialEndpoint.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/CredentialEndpoint.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/DarwinUtils.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/DarwinUtils.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/DockerUtils.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/DockerUtils.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,28 +41,28 @@
         try:
             image = client.images.get(name)
             return True
         except:
             return False
 
     @staticmethod
-    def build(tags, context, args):
+    def build(tags: [str], context: str, args: [str]) -> [str]:
         """
         Returns the `docker build` command to build an image
         """
         tagArgs = [["-t", tag] for tag in tags]
         return (
             ["docker", "build"]
             + list(itertools.chain.from_iterable(tagArgs))
             + [context]
             + args
         )
 
     @staticmethod
-    def buildx(tags, context, args, secrets):
+    def buildx(tags: [str], context: str, args: [str], secrets: [str]) -> [str]:
         """
         Returns the `docker buildx` command to build an image with the BuildKit backend
         """
         tagArgs = [["-t", tag] for tag in tags]
         return (
             ["docker", "build"]
             + list(itertools.chain.from_iterable(tagArgs))
```

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/GlobalConfiguration.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/GlobalConfiguration.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/ImageBuilder.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/ImageBuilder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,104 @@
 from typing import Dict, Optional
 
 from .DockerUtils import DockerUtils
 from .FilesystemUtils import FilesystemUtils
 from .GlobalConfiguration import GlobalConfiguration
 import glob, humanfriendly, os, shutil, subprocess, tempfile, time
 from os.path import basename, exists, join
-from jinja2 import Environment, Template
+from jinja2 import Environment
+
+
+class ImageBuildParams(object):
+    def __init__(
+        self, dockerfile: str, context_dir: str, env: Optional[Dict[str, str]] = None
+    ):
+        self.dockerfile = dockerfile
+        self.context_dir = context_dir
+        self.env = env
 
 
 class ImageBuilder(object):
     def __init__(
         self,
-        root,
-        platform,
+        tempDir: str,
+        platform: str,
         logger,
-        rebuild=False,
-        dryRun=False,
-        layoutDir=None,
-        templateContext=None,
-        combine=False,
+        rebuild: bool = False,
+        dryRun: bool = False,
+        layoutDir: str = None,
+        templateContext: Dict[str, str] = None,
+        combine: bool = False,
     ):
         """
         Creates an ImageBuilder for the specified build parameters
         """
-        self.root = root
+        self.tempDir = tempDir
         self.platform = platform
         self.logger = logger
         self.rebuild = rebuild
         self.dryRun = dryRun
         self.layoutDir = layoutDir
         self.templateContext = templateContext if templateContext is not None else {}
         self.combine = combine
 
-    def build(self, name, tags, args, secrets=None):
+    def get_built_image_context(self, name):
+        """
+        Resolve the full path to the build context for the specified image
+        """
+        return os.path.normpath(
+            os.path.join(
+                os.path.dirname(os.path.abspath(__file__)),
+                "..",
+                "dockerfiles",
+                basename(name),
+                self.platform,
+            )
+        )
+
+    def build_builtin_image(
+        self,
+        name: str,
+        tags: [str],
+        args: [str],
+        builtin_name: str = None,
+        secrets: Dict[str, str] = None,
+    ):
+        context_dir = self.get_built_image_context(
+            name if builtin_name is None else builtin_name
+        )
+        return self.build(
+            name, tags, args, join(context_dir, "Dockerfile"), context_dir, secrets
+        )
+
+    def build(
+        self,
+        name: str,
+        tags: [str],
+        args: [str],
+        dockerfile_template: str,
+        context_dir: str,
+        secrets: Dict[str, str] = None,
+    ):
         """
         Builds the specified image if it doesn't exist or if we're forcing a rebuild
         """
 
+        workdir = join(self.tempDir, basename(name), self.platform)
+        os.makedirs(workdir, exist_ok=True)
+
         # Create a Jinja template environment and render the Dockerfile template
         environment = Environment(
             autoescape=False, trim_blocks=True, lstrip_blocks=True
         )
-        dockerfile = join(self.context(name), "Dockerfile")
-        templateInstance = environment.from_string(FilesystemUtils.readFile(dockerfile))
+        dockerfile = join(workdir, "Dockerfile")
+
+        templateInstance = environment.from_string(
+            FilesystemUtils.readFile(dockerfile_template)
+        )
         rendered = templateInstance.render(self.templateContext)
 
         # Compress excess whitespace introduced during Jinja rendering and save the contents back to disk
         # (Ensure that we still have a single trailing newline at the end of the Dockerfile)
         while "\n\n\n" in rendered:
             rendered = rendered.replace("\n\n\n", "\n\n")
         rendered = rendered.strip("\n") + "\n"
@@ -66,127 +118,122 @@
         )
 
         # Create a temporary directory to hold any files needed for the build
         with tempfile.TemporaryDirectory() as tempDir:
 
             # Determine whether we are building using `docker buildx` with build secrets
             imageTags = self._formatTags(name, tags)
-            command = DockerUtils.build(imageTags, self.context(name), args)
 
             if self.platform == "linux" and secrets is not None and len(secrets) > 0:
 
                 # Create temporary files to store the contents of each of our secrets
                 secretFlags = []
                 for secret, contents in secrets.items():
                     secretFile = join(tempDir, secret)
                     FilesystemUtils.writeFile(secretFile, contents)
                     secretFlags.append("id={},src={}".format(secret, secretFile))
 
                 # Generate the `docker buildx` command to use our build secrets
-                command = DockerUtils.buildx(
-                    imageTags, self.context(name), args, secretFlags
-                )
+                command = DockerUtils.buildx(imageTags, context_dir, args, secretFlags)
+            else:
+                command = DockerUtils.build(imageTags, context_dir, args)
+
+            command += ["--file", dockerfile]
 
             env = os.environ.copy()
             if self.platform == "linux":
                 env["DOCKER_BUILDKIT"] = "1"
 
             # Build the image if it doesn't already exist
             self._processImage(
                 imageTags[0],
                 name,
                 command,
                 "build",
                 "built",
-                env=env,
+                ImageBuildParams(dockerfile, context_dir, env),
             )
 
-    def context(self, name):
-        """
-        Resolve the full path to the build context for the specified image
-        """
-        return join(self.root, basename(name), self.platform)
-
-    def pull(self, image):
+    def pull(self, image: str) -> None:
         """
         Pulls the specified image if it doesn't exist or if we're forcing a pull of a newer version
         """
         self._processImage(image, None, DockerUtils.pull(image), "pull", "pulled")
 
-    def willBuild(self, name, tags):
+    def willBuild(self, name: str, tags: [str]) -> bool:
         """
         Determines if we will build the specified image, based on our build settings
         """
         imageTags = self._formatTags(name, tags)
         return self._willProcess(imageTags[0])
 
-    def _formatTags(self, name, tags):
+    def _formatTags(self, name: str, tags: [str]):
         """
         Generates the list of fully-qualified tags that we will use when building an image
         """
         return [
             "{}:{}".format(GlobalConfiguration.resolveTag(name), tag) for tag in tags
         ]
 
-    def _willProcess(self, image):
+    def _willProcess(self, image: [str]) -> bool:
         """
         Determines if we will build or pull the specified image, based on our build settings
         """
-        return self.rebuild == True or DockerUtils.exists(image) == False
+        return self.rebuild or not DockerUtils.exists(image)
 
     def _processImage(
         self,
         image: str,
         name: Optional[str],
         command: [str],
         actionPresentTense: str,
         actionPastTense: str,
-        env: Optional[Dict[str, str]] = None,
-    ):
+        build_params: Optional[ImageBuildParams] = None,
+    ) -> None:
         """
         Processes the specified image by running the supplied command if it doesn't exist (use rebuild=True to force processing)
         """
 
         # Determine if we are processing the image
-        if self._willProcess(image) == False:
+        if not self._willProcess(image):
             self.logger.info(
                 'Image "{}" exists and rebuild not requested, skipping {}.'.format(
                     image, actionPresentTense
                 )
             )
             return
 
         # Determine if we are running in "dry run" mode
         self.logger.action(
             '{}ing image "{}"...'.format(actionPresentTense.capitalize(), image)
         )
-        if self.dryRun == True:
+        if self.dryRun:
             print(command)
             self.logger.action(
                 'Completed dry run for image "{}".'.format(image), newline=False
             )
             return
 
         # Determine if we're just copying the Dockerfile to an output directory
         if self.layoutDir is not None:
 
             # Determine whether we're performing a simple copy or combining generated Dockerfiles
-            source = self.context(name)
-            if self.combine == True:
+            if self.combine:
 
                 # Ensure the destination directory exists
                 dest = join(self.layoutDir, "combined")
                 self.logger.action(
-                    'Merging "{}" into "{}"...'.format(source, dest), newline=False
+                    'Merging "{}" into "{}"...'.format(build_params.context_dir, dest),
+                    newline=False,
                 )
                 os.makedirs(dest, exist_ok=True)
 
                 # Merge the source Dockerfile with any existing Dockerfile contents in the destination directory
                 # (Insert a single newline between merged file contents and ensure we have a single trailing newline)
-                sourceDockerfile = join(source, "Dockerfile")
+                sourceDockerfile = build_params.dockerfile
                 destDockerfile = join(dest, "Dockerfile")
                 dockerfileContents = (
                     FilesystemUtils.readFile(destDockerfile)
                     if exists(destDockerfile)
                     else ""
                 )
                 dockerfileContents = (
@@ -195,40 +242,44 @@
                     + FilesystemUtils.readFile(sourceDockerfile)
                 )
                 dockerfileContents = dockerfileContents.strip("\n") + "\n"
                 FilesystemUtils.writeFile(destDockerfile, dockerfileContents)
 
                 # Copy any supplemental files from the source directory to the destination directory
                 # (Exclude any extraneous files which are not referenced in the Dockerfile contents)
-                for file in glob.glob(join(source, "*.*")):
+                for file in glob.glob(join(build_params.context_dir, "*.*")):
                     if basename(file) in dockerfileContents:
                         shutil.copy(file, join(dest, basename(file)))
 
                 # Report our success
                 self.logger.action(
                     'Merged Dockerfile for image "{}".'.format(image), newline=False
                 )
 
             else:
 
                 # Copy the source directory to the destination
                 dest = join(self.layoutDir, basename(name))
                 self.logger.action(
-                    'Copying "{}" to "{}"...'.format(source, dest), newline=False
+                    'Copying "{}" to "{}"...'.format(build_params.context_dir, dest),
+                    newline=False,
                 )
-                shutil.copytree(source, dest)
+                shutil.copytree(build_params.context_dir, dest)
+                shutil.copy(build_params.dockerfile, dest)
                 self.logger.action(
                     'Copied Dockerfile for image "{}".'.format(image), newline=False
                 )
 
             return
 
         # Attempt to process the image using the supplied command
         startTime = time.time()
-        exitCode = subprocess.call(command, env=env)
+        exitCode = subprocess.call(
+            command, env=build_params.env if build_params else None
+        )
         endTime = time.time()
 
         # Determine if processing succeeded
         if exitCode == 0:
             self.logger.action(
                 '{} image "{}" in {}'.format(
                     actionPastTense.capitalize(),
```

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/ImageCleaner.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/ImageCleaner.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/Logger.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/Logger.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/PackageUtils.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/PackageUtils.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/PrettyPrinting.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/PrettyPrinting.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/ResourceMonitor.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/ResourceMonitor.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/SubprocessUtils.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/SubprocessUtils.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/WindowsUtils.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/WindowsUtils.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/infrastructure/__init__.py` & `ue4-docker-0.0.99/ue4docker/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/main.py` & `ue4-docker-0.0.99/ue4docker/main.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/setup_cmd.py` & `ue4-docker-0.0.99/ue4docker/setup_cmd.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/test.py` & `ue4-docker-0.0.99/ue4docker/test.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/tests/build-and-package.py` & `ue4-docker-0.0.99/ue4docker/tests/build-and-package.py`

 * *Files identical despite different names*

### Comparing `ue4-docker-0.0.98/ue4docker/tests/consume-external-deps.py` & `ue4-docker-0.0.99/ue4docker/tests/consume-external-deps.py`

 * *Files identical despite different names*

