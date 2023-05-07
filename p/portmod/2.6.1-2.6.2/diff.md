# Comparing `tmp/portmod-2.6.1.tar.gz` & `tmp/portmod-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/portmod-2.6.1.tar", last modified: Mon Apr 17 22:30:25 2023, max compression
+gzip compressed data, was "dist/portmod-2.6.2.tar", last modified: Sun May  7 01:16:10 2023, max compression
```

## Comparing `portmod-2.6.1.tar` & `portmod-2.6.2.tar`

### file list

```diff
@@ -1,418 +1,419 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/
--rw-rw-rw-   0 root         (0) root         (0)     3059 2023-04-17 22:18:49.000000 portmod-2.6.1/.appveyor.yml
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-17 22:18:49.000000 portmod-2.6.1/.bandit.yaml
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-04-17 22:18:49.000000 portmod-2.6.1/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-17 22:18:49.000000 portmod-2.6.1/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-17 22:18:49.000000 portmod-2.6.1/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/.gitlab/issue_templates/
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-04-17 22:18:49.000000 portmod-2.6.1/.gitlab/issue_templates/Bug.md
--rw-rw-rw-   0 root         (0) root         (0)     4807 2023-04-17 22:18:49.000000 portmod-2.6.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/.portmod_not_installed
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-04-17 22:18:49.000000 portmod-2.6.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      871 2023-04-17 22:18:49.000000 portmod-2.6.1/.pre-commit-hooks.yaml
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-17 22:18:49.000000 portmod-2.6.1/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-17 22:18:49.000000 portmod-2.6.1/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-17 22:18:49.000000 portmod-2.6.1/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    79947 2023-04-17 22:18:49.000000 portmod-2.6.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-17 22:18:49.000000 portmod-2.6.1/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    53303 2023-04-17 22:18:49.000000 portmod-2.6.1/Cargo.lock
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-17 22:18:49.000000 portmod-2.6.1/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-04-17 22:18:49.000000 portmod-2.6.1/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    35141 2023-04-17 22:18:49.000000 portmod-2.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7248 2023-04-17 22:30:25.000000 portmod-2.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5880 2023-04-17 22:18:49.000000 portmod-2.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/bin/
--rwxrwxrwx   0 root         (0) root         (0)      467 2023-04-17 22:18:49.000000 portmod-2.6.1/bin/inquisitor
--rwxrwxrwx   0 root         (0) root         (0)      485 2023-04-17 22:18:49.000000 portmod-2.6.1/bin/portmod
--rwxrwxrwx   0 root         (0) root         (0)      480 2023-04-17 22:18:49.000000 portmod-2.6.1/bin/portmod-gui
--rw-rw-rw-   0 root         (0) root         (0)     5729 2023-04-17 22:18:49.000000 portmod-2.6.1/code_of_conduct.md
--rw-rw-rw-   0 root         (0) root         (0)     3174 2023-04-17 22:18:49.000000 portmod-2.6.1/default.nix
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      650 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_build/man/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_build/man/man1/
--rw-r--r--   0 root         (0) root         (0)     3445 2023-04-17 22:28:37.000000 portmod-2.6.1/doc/_build/man/man1/inquisitor.1
--rw-r--r--   0 root         (0) root         (0)    17408 2023-04-17 22:28:37.000000 portmod-2.6.1/doc/_build/man/man1/portmod.1
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_build/man/man3/
--rw-r--r--   0 root         (0) root         (0)    49702 2023-04-17 22:28:38.000000 portmod-2.6.1/doc/_build/man/man3/pybuild.3
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_build/man/man5/
--rw-r--r--   0 root         (0) root         (0)    14769 2023-04-17 22:28:37.000000 portmod-2.6.1/doc/_build/man/man5/portmod.5
--rw-r--r--   0 root         (0) root         (0)    16480 2023-04-17 22:28:38.000000 portmod-2.6.1/doc/_build/man/man5/pybuild.5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_build/man/man7/
--rw-r--r--   0 root         (0) root         (0)    16228 2023-04-17 22:28:38.000000 portmod-2.6.1/doc/_build/man/man7/portmod.7
--rw-r--r--   0 root         (0) root         (0)    83378 2023-04-17 22:28:38.000000 portmod-2.6.1/doc/_build/man/man7/pybuild.7
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_ext/
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/_ext/summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_static/css/
--rw-rw-rw-   0 root         (0) root         (0)     1830 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/_static/css/custom.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/_templates/
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/_templates/package.rst_t
--rw-rw-rw-   0 root         (0) root         (0)     2560 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/basic-usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/cli/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/cli/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/cli/inquisitor.rst
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/cli/portmod.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/concepts/
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/concepts/cfg-protect.rst
--rw-rw-rw-   0 root         (0) root         (0)      741 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/concepts/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2694 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/concepts/keywords.rst
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/concepts/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/concepts/profiles.rst
--rw-rw-rw-   0 root         (0) root         (0)     4681 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/concepts/sandbox.rst
--rw-rw-rw-   0 root         (0) root         (0)     1682 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/concepts/sets.rst
--rw-rw-rw-   0 root         (0) root         (0)     2323 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/concepts/use-flags.rst
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/config/
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/config/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/config/package.accept_keywords.rst
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/config/package.accept_license.rst
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/config/package.mask.rst
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/config/package.use.rst
--rw-rw-rw-   0 root         (0) root         (0)     4779 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/config/portmod.conf.rst
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/config/profile.user.rst
--rw-rw-rw-   0 root         (0) root         (0)     1825 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/config/repos.cfg.rst
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/config/sets.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/dev/
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/arch_version.rst
--rw-rw-rw-   0 root         (0) root         (0)     1301 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/archives.rst
--rw-rw-rw-   0 root         (0) root         (0)     3644 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/common.rst
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/dependencies.rst
--rw-rw-rw-   0 root         (0) root         (0)     2249 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/l10n.rst
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/manifest.rst
--rw-rw-rw-   0 root         (0) root         (0)     6953 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)     7053 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/naming.rst
--rw-rw-rw-   0 root         (0) root         (0)     2194 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/packages.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/dev/repo/
--rw-rw-rw-   0 root         (0) root         (0)     4927 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/repo/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1362 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/repo/layout.conf.rst
--rw-rw-rw-   0 root         (0) root         (0)     7043 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/repo/metadata.yaml.rst
--rw-rw-rw-   0 root         (0) root         (0)    11849 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/repo/profiles.rst
--rw-rw-rw-   0 root         (0) root         (0)     3886 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/setup.rst
--rw-rw-rw-   0 root         (0) root         (0)     7322 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/dev/use-flags.rst
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/doc/install/
--rw-rw-rw-   0 root         (0) root         (0)     5227 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/install/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/install/linux.rst
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/install/macos.rst
--rw-rw-rw-   0 root         (0) root         (0)     4707 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/install/windows.rst
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4427 2023-04-17 22:18:49.000000 portmod-2.6.1/doc/setup.rst
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-04-17 22:18:49.000000 portmod-2.6.1/header.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/l10n/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/l10n/en-GB/
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-04-17 22:18:49.000000 portmod-2.6.1/l10n/en-GB/gui.ftl
--rw-rw-rw-   0 root         (0) root         (0)    37168 2023-04-17 22:18:49.000000 portmod-2.6.1/l10n/en-GB/main.ftl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/l10n/en-US/
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-17 22:18:49.000000 portmod-2.6.1/l10n/en-US/main.ftl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/l10n/fr/
--rw-rw-rw-   0 root         (0) root         (0)     2919 2023-04-17 22:18:49.000000 portmod-2.6.1/l10n/fr/main.ftl
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-17 22:18:49.000000 portmod-2.6.1/l10n/l10n.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/l10n/sv-SE/
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-04-17 22:18:49.000000 portmod-2.6.1/l10n/sv-SE/main.ftl
--rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-17 22:18:49.000000 portmod-2.6.1/mkdoc.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/_cli/
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6053 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/cfg_update.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/destroy.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/error.py
--rw-rw-rw-   0 root         (0) root         (0)     4508 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/init.py
--rw-rw-rw-   0 root         (0) root         (0)    23482 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/inquisitor.py
--rw-rw-rw-   0 root         (0) root         (0)    12729 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/main.py
--rw-rw-rw-   0 root         (0) root         (0)    19368 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/merge.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/mirror.py
--rw-rw-rw-   0 root         (0) root         (0)     3665 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/pybuild.py
--rw-rw-rw-   0 root         (0) root         (0)    13952 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/query.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/run.py
--rw-rw-rw-   0 root         (0) root         (0)     1582 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/search.py
--rw-rw-rw-   0 root         (0) root         (0)     7471 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/select.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/sync.py
--rw-rw-rw-   0 root         (0) root         (0)     2055 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/use.py
--rw-rw-rw-   0 root         (0) root         (0)     1663 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_cli/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/_deprecated/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_deprecated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_deprecated/rebuild.py
--rw-rw-rw-   0 root         (0) root         (0)     8784 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_deprecated/vfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/_deps/
--rw-rw-rw-   0 root         (0) root         (0)    21789 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_deps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28291 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_deps/formula.py
--rw-rw-rw-   0 root         (0) root         (0)     3262 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_deps/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)    17697 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_deps/weights.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/_gui/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/_gui/Manage/
--rw-rw-rw-   0 root         (0) root         (0)      476 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Manage/DetailsLabel.qml
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Manage/FlagListModel.py
--rw-rw-rw-   0 root         (0) root         (0)     6572 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Manage/InstalledPackagesModel.py
--rw-rw-rw-   0 root         (0) root         (0)     2393 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Manage/InstalledPackagesPanel.qml
--rw-rw-rw-   0 root         (0) root         (0)     4145 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Manage/ManageTab.qml
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Manage/PackageDetailsPanel.qml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Manage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/_gui/Search/
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Search/SearchPackagesModel.py
--rw-rw-rw-   0 root         (0) root         (0)     2472 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Search/SearchTab.qml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/Search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2252 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/human_bytes.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/l10n.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/main.qml
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/_gui/packages.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6082 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5831 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/cfg_protect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/config/
--rw-rw-rw-   0 root         (0) root         (0)     7241 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3148 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/config/license.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/config/mask.py
--rw-rw-rw-   0 root         (0) root         (0)     3587 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/config/profiles.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/config/pyconf.py
--rw-rw-rw-   0 root         (0) root         (0)     5648 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/config/sets.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/config/textures.py
--rw-rw-rw-   0 root         (0) root         (0)    13619 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/config/use.py
--rw-rw-rw-   0 root         (0) root         (0)    14477 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/download.py
--rw-rw-rw-   0 root         (0) root         (0)    14699 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/execute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/fs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/fs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2680 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/functools.py
--rw-rw-rw-   0 root         (0) root         (0)     5402 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/globals.py
--rw-rw-rw-   0 root         (0) root         (0)     9858 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/io.py
--rw-rw-rw-   0 root         (0) root         (0)    20297 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     6219 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/lock.py
--rw-rw-rw-   0 root         (0) root         (0)    21551 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/merge.py
--rw-rw-rw-   0 root         (0) root         (0)     5004 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/modules.py
--rw-rw-rw-   0 root         (0) root         (0)    12126 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/news.py
--rw-rw-rw-   0 root         (0) root         (0)    18772 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4735 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/parsers/flags.py
--rw-rw-rw-   0 root         (0) root         (0)     6334 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/parsers/manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/parsers/userconf.py
--rw-rw-rw-   0 root         (0) root         (0)     1356 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/perms.py
--rw-rw-rw-   0 root         (0) root         (0)     6911 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/prefix.py
--rw-rw-rw-   0 root         (0) root         (0)     7092 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/prompt.py
--rw-rw-rw-   0 root         (0) root         (0)    23081 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/pybuild.py
--rw-rw-rw-   0 root         (0) root         (0)    26890 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod/repo/
--rw-rw-rw-   0 root         (0) root         (0)     3971 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/repo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12708 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/repo/keywords.py
--rw-rw-rw-   0 root         (0) root         (0)    16589 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/repo/loader.py
--rw-rw-rw-   0 root         (0) root         (0)    10106 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/repo/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1552 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/repo/updates.py
--rw-rw-rw-   0 root         (0) root         (0)     5929 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/repos.py
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/source.py
--rw-rw-rw-   0 root         (0) root         (0)     5232 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/sync.py
--rw-rw-rw-   0 root         (0) root         (0)    14068 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/transactions.py
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/tsort.py
--rw-rw-rw-   0 root         (0) root         (0)     4726 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/util.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/vdb.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-17 22:18:49.000000 portmod-2.6.1/portmod/win32.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7248 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8744 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      140 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 22:20:11.000000 portmod-2.6.1/portmod.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      675 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-17 22:30:24.000000 portmod-2.6.1/portmod.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmodlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmodlib/_deprecated/
--rw-rw-rw-   0 root         (0) root         (0)    11502 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/_deprecated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4875 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/_deprecated/vfs.py
--rw-rw-rw-   0 root         (0) root         (0)    10669 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/_phase.py
--rw-rw-rw-   0 root         (0) root         (0)     7758 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     3196 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/archives.py
--rw-rw-rw-   0 root         (0) root         (0)    11301 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/atom.py
--rw-rw-rw-   0 root         (0) root         (0)     1159 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/colour.py
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     9613 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/fs.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/functools.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/globals.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/l10n.py
--rw-rw-rw-   0 root         (0) root         (0)     1703 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/log.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/masters.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/module_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/portmodlib/parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1738 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/parsers/list.py
--rw-rw-rw-   0 root         (0) root         (0)     4212 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/portmod.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9627 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/pybuild.py
--rw-rw-rw-   0 root         (0) root         (0)     1660 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/source.py
--rw-rw-rw-   0 root         (0) root         (0)    21357 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/usestr.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/util.py
--rw-rw-rw-   0 root         (0) root         (0)    13354 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-04-17 22:18:49.000000 portmod-2.6.1/portmodlib/winreg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/pybuild/
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-04-17 22:18:49.000000 portmod-2.6.1/pybuild/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33866 2023-04-17 22:18:49.000000 portmod-2.6.1/pybuild/_pybuild.py
--rw-rw-rw-   0 root         (0) root         (0)     1551 2023-04-17 22:18:49.000000 portmod-2.6.1/pybuild/info.py
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-04-17 22:18:49.000000 portmod-2.6.1/pybuild/winreg.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-04-17 22:18:49.000000 portmod-2.6.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-04-17 22:18:49.000000 portmod-2.6.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-04-17 22:30:25.000000 portmod-2.6.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4920 2023-04-17 22:18:49.000000 portmod-2.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/src/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-04-17 22:18:49.000000 portmod-2.6.1/src/dds.rs
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-04-17 22:18:49.000000 portmod-2.6.1/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)     9538 2023-04-17 22:18:49.000000 portmod-2.6.1/src/index.rs
--rw-rw-rw-   0 root         (0) root         (0)    11290 2023-04-17 22:18:49.000000 portmod-2.6.1/src/lib.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/src/metadata/
--rw-rw-rw-   0 root         (0) root         (0)     4787 2023-04-17 22:18:49.000000 portmod-2.6.1/src/metadata/mod.rs
--rw-rw-rw-   0 root         (0) root         (0)     2904 2023-04-17 22:18:49.000000 portmod-2.6.1/src/metadata/person.rs
--rw-rw-rw-   0 root         (0) root         (0)     1864 2023-04-17 22:18:49.000000 portmod-2.6.1/src/news.rs
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-04-17 22:18:49.000000 portmod-2.6.1/src/yaml.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/_benchmarks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/test/_benchmarks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-04-17 22:18:49.000000 portmod-2.6.1/test/_benchmarks/atom.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-04-17 22:18:49.000000 portmod-2.6.1/test/_benchmarks/hash.py
--rw-rw-rw-   0 root         (0) root         (0)     4128 2023-04-17 22:18:49.000000 portmod-2.6.1/test/_benchmarks/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     4448 2023-04-17 22:18:49.000000 portmod-2.6.1/test/env.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-17 22:18:49.000000 portmod-2.6.1/test/merge.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_alias.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_atom.py
--rw-rw-rw-   0 root         (0) root         (0)     6464 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_cfg_protect.py
--rw-rw-rw-   0 root         (0) root         (0)     1435 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_clean.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_common.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_deps.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_download.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2434 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_existing.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2799 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_fs.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_gui_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3564 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_gui_installed_packages_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_gui_packages.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_init.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_inquisitor.py
--rw-rw-rw-   0 root         (0) root         (0)     7428 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_keywords.py
--rw-rw-rw-   0 root         (0) root         (0)    24407 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_log.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_mask.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_masters.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_news.py
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_obscure.py
--rw-rw-rw-   0 root         (0) root         (0)     1884 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_portmod_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_prefix_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_query.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_resolve.py
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_select.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_unpack.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_updates.py
--rw-rw-rw-   0 root         (0) root         (0)     4235 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_use.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_vdb.py
--rw-rw-rw-   0 root         (0) root         (0)     6518 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7996 2023-04-17 22:18:49.000000 portmod-2.6.1/test/test_vfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/common/masked/
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/common/masked/masked-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/common/superclass/
--rw-rw-rw-   0 root         (0) root         (0)      472 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/common/superclass/superclass-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/licenses/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/licenses/CC-BY-SA-4.0
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/licenses/eula
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/licenses/free-use
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/licenses/test
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/metadata/news/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/metadata/news/2020-04-12-installed/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/metadata/news/2020-04-12-installed/2020-04-12-installed.en.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/metadata/news/2020-04-12-keyword/
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/metadata/news/2020-04-12-keyword/2020-04-12-keyword.en.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/metadata/news/2020-04-12-profile/
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/metadata/news/2020-04-12-profile/2020-04-12-profile.en.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/metadata/news/2020-04-12-test/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/metadata/news/2020-04-12-test/2020-04-12-test.en.yaml
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/metadata/repos.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/profiles/
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/arch.list
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/profiles/base/
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/base/defaults.conf
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/categories
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/profiles/desc/
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/desc/screen_aspect.yaml
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/license_groups.yaml
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/package.mask
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/profiles.yaml
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/repo_name
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/profiles/test/
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/test/packages
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/test/parent
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/profiles/test-config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/test-config/defaults.conf
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/test-config/parent
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/profiles/test-unstable/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/test-unstable/defaults.conf
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/test-unstable/parent
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/profiles/updates/
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/updates/2Q-2020
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/use.alias.yaml
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/profiles/use.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/test/masked/
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/masked/masked-1.0.pybuild
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/masked/masked-1.1.pybuild
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/metadata.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/test/quill-of-feyfolken/
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/quill-of-feyfolken/Manifest
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/quill-of-feyfolken/metadata.yaml
--rw-rw-rw-   0 root         (0) root         (0)      723 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/quill-of-feyfolken/quill-of-feyfolken-2.0.2-r1.pybuild
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/quill-of-feyfolken/quill-of-feyfolken-2.0.2.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/test/test/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test/metadata.yaml
--rw-rw-rw-   0 root         (0) root         (0)      736 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test/test-1.0-r1.pybuild
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test/test-1.0-r2.pybuild
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test/test-1.0.pybuild
--rw-rw-rw-   0 root         (0) root         (0)     1094 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test/test-2.0.pybuild
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test/test-2.0_rc1.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/test/test-eula/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test-eula/test-eula-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/test/test-install/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test-install/Manifest
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/test/test-install/files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test-install/files/file
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test-install/test-install-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/test/test-module/
--rw-rw-rw-   0 root         (0) root         (0)     1666 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test-module/test-module-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:24.000000 portmod-2.6.1/test/testrepo/test/test-new/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test-new/test-new-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/test/testrepo/test/test-nofetch/
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test-nofetch/Manifest
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test-nofetch/test-nofetch-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/test/testrepo/test/test-useless/
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test-useless/test-useless-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/test/testrepo/test/test0/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test0/test0-1.0_rc1.pybuild
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test0/test0-2.0_alpha.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/test/testrepo/test/test2/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test2/test2-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/test/testrepo/test/test3/
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test3/test3-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/test/testrepo/test/test4/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test4/metadata.yaml
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test4/test4-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/test/testrepo/test/test5/
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test5/test5-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/test/testrepo/test/test6/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test6/test6-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/test/testrepo/test/test7/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test7/test7-0.1.pybuild
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-04-17 22:18:49.000000 portmod-2.6.1/test/testrepo/test/test7/test7-1.0.pybuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:30:25.000000 portmod-2.6.1/tools/
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-04-17 22:18:49.000000 portmod-2.6.1/tools/update_header.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)     3059 2023-05-07 01:04:18.000000 portmod-2.6.2/.appveyor.yml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-07 01:04:18.000000 portmod-2.6.2/.bandit.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-05-07 01:04:18.000000 portmod-2.6.2/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-07 01:04:18.000000 portmod-2.6.2/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-07 01:04:18.000000 portmod-2.6.2/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-05-07 01:04:18.000000 portmod-2.6.2/.gitlab/issue_templates/Bug.md
+-rw-rw-rw-   0 root         (0) root         (0)     4823 2023-05-07 01:04:18.000000 portmod-2.6.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/.portmod_not_installed
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-05-07 01:04:18.000000 portmod-2.6.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      871 2023-05-07 01:04:18.000000 portmod-2.6.2/.pre-commit-hooks.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-05-07 01:04:18.000000 portmod-2.6.2/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-05-07 01:04:18.000000 portmod-2.6.2/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-07 01:04:18.000000 portmod-2.6.2/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    80254 2023-05-07 01:04:18.000000 portmod-2.6.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-07 01:04:18.000000 portmod-2.6.2/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    53303 2023-05-07 01:04:18.000000 portmod-2.6.2/Cargo.lock
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-05-07 01:04:18.000000 portmod-2.6.2/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-05-07 01:04:18.000000 portmod-2.6.2/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    35141 2023-05-07 01:04:18.000000 portmod-2.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7248 2023-05-07 01:16:10.000000 portmod-2.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5880 2023-05-07 01:04:18.000000 portmod-2.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/bin/
+-rwxrwxrwx   0 root         (0) root         (0)      467 2023-05-07 01:04:18.000000 portmod-2.6.2/bin/inquisitor
+-rwxrwxrwx   0 root         (0) root         (0)      485 2023-05-07 01:04:18.000000 portmod-2.6.2/bin/portmod
+-rwxrwxrwx   0 root         (0) root         (0)      480 2023-05-07 01:04:18.000000 portmod-2.6.2/bin/portmod-gui
+-rw-rw-rw-   0 root         (0) root         (0)     5729 2023-05-07 01:04:18.000000 portmod-2.6.2/code_of_conduct.md
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2023-05-07 01:04:18.000000 portmod-2.6.2/default.nix
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      650 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_build/man/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_build/man/man1/
+-rw-r--r--   0 root         (0) root         (0)     3445 2023-05-07 01:14:32.000000 portmod-2.6.2/doc/_build/man/man1/inquisitor.1
+-rw-r--r--   0 root         (0) root         (0)    17408 2023-05-07 01:14:32.000000 portmod-2.6.2/doc/_build/man/man1/portmod.1
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_build/man/man3/
+-rw-r--r--   0 root         (0) root         (0)    49702 2023-05-07 01:14:33.000000 portmod-2.6.2/doc/_build/man/man3/pybuild.3
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_build/man/man5/
+-rw-r--r--   0 root         (0) root         (0)    14769 2023-05-07 01:14:32.000000 portmod-2.6.2/doc/_build/man/man5/portmod.5
+-rw-r--r--   0 root         (0) root         (0)    20743 2023-05-07 01:14:33.000000 portmod-2.6.2/doc/_build/man/man5/pybuild.5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_build/man/man7/
+-rw-r--r--   0 root         (0) root         (0)    16313 2023-05-07 01:14:32.000000 portmod-2.6.2/doc/_build/man/man7/portmod.7
+-rw-r--r--   0 root         (0) root         (0)    84696 2023-05-07 01:14:33.000000 portmod-2.6.2/doc/_build/man/man7/pybuild.7
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_ext/
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/_ext/summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_static/css/
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/_static/css/custom.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/_templates/package.rst_t
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/basic-usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/cli/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/cli/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/cli/inquisitor.rst
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/cli/portmod.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/concepts/
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/concepts/cfg-protect.rst
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/concepts/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/concepts/keywords.rst
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/concepts/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/concepts/profiles.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4681 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/concepts/sandbox.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1768 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/concepts/sets.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2323 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/concepts/use-flags.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/config/
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/config/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/config/package.accept_keywords.rst
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/config/package.accept_license.rst
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/config/package.mask.rst
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/config/package.use.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4779 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/config/portmod.conf.rst
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/config/profile.user.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1825 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/config/repos.cfg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/config/sets.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/dev/
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/arch_version.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/archives.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/common.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/dependencies.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2249 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/l10n.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/manifest.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7072 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/naming.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/packages.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/dev/repo/
+-rw-rw-rw-   0 root         (0) root         (0)     5920 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/repo/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/repo/layout.conf.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7043 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/repo/metadata.yaml.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/repo/package-files.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11849 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/repo/profiles.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3886 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/setup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7322 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/dev/use-flags.rst
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/doc/install/
+-rw-rw-rw-   0 root         (0) root         (0)     5227 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/install/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/install/linux.rst
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/install/macos.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/install/windows.rst
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4427 2023-05-07 01:04:18.000000 portmod-2.6.2/doc/setup.rst
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-07 01:04:18.000000 portmod-2.6.2/header.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/l10n/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/l10n/en-GB/
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-07 01:04:18.000000 portmod-2.6.2/l10n/en-GB/gui.ftl
+-rw-rw-rw-   0 root         (0) root         (0)    37168 2023-05-07 01:04:18.000000 portmod-2.6.2/l10n/en-GB/main.ftl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/l10n/en-US/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-07 01:04:18.000000 portmod-2.6.2/l10n/en-US/main.ftl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/l10n/fr/
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2023-05-07 01:04:18.000000 portmod-2.6.2/l10n/fr/main.ftl
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-07 01:04:18.000000 portmod-2.6.2/l10n/l10n.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/l10n/sv-SE/
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-05-07 01:04:18.000000 portmod-2.6.2/l10n/sv-SE/main.ftl
+-rwxrwxrwx   0 root         (0) root         (0)      475 2023-05-07 01:04:18.000000 portmod-2.6.2/mkdoc.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/_cli/
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6053 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/cfg_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/destroy.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     4508 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/init.py
+-rw-rw-rw-   0 root         (0) root         (0)    23482 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/inquisitor.py
+-rw-rw-rw-   0 root         (0) root         (0)    12729 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    19368 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/mirror.py
+-rw-rw-rw-   0 root         (0) root         (0)     3665 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/pybuild.py
+-rw-rw-rw-   0 root         (0) root         (0)    13952 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1582 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7471 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/select.py
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/sync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/use.py
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_cli/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/_deprecated/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_deprecated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_deprecated/rebuild.py
+-rw-rw-rw-   0 root         (0) root         (0)     8784 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_deprecated/vfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/_deps/
+-rw-rw-rw-   0 root         (0) root         (0)    21789 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_deps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28291 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_deps/formula.py
+-rw-rw-rw-   0 root         (0) root         (0)     3262 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_deps/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)    17697 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_deps/weights.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/_gui/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/_gui/Manage/
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Manage/DetailsLabel.qml
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Manage/FlagListModel.py
+-rw-rw-rw-   0 root         (0) root         (0)     6572 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Manage/InstalledPackagesModel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Manage/InstalledPackagesPanel.qml
+-rw-rw-rw-   0 root         (0) root         (0)     4145 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Manage/ManageTab.qml
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Manage/PackageDetailsPanel.qml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Manage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/_gui/Search/
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Search/SearchPackagesModel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Search/SearchTab.qml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/Search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/human_bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/l10n.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/main.qml
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/_gui/packages.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-07 01:16:09.000000 portmod-2.6.2/portmod/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6220 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5831 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/cfg_protect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/config/
+-rw-rw-rw-   0 root         (0) root         (0)     7241 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3148 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/config/license.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/config/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     3587 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/config/profiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/config/pyconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5648 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/config/sets.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/config/textures.py
+-rw-rw-rw-   0 root         (0) root         (0)    13619 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/config/use.py
+-rw-rw-rw-   0 root         (0) root         (0)    14477 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/download.py
+-rw-rw-rw-   0 root         (0) root         (0)    14699 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/execute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/fs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/fs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/functools.py
+-rw-rw-rw-   0 root         (0) root         (0)     5533 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/globals.py
+-rw-rw-rw-   0 root         (0) root         (0)     9858 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    20297 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6219 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/lock.py
+-rw-rw-rw-   0 root         (0) root         (0)    21551 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     5004 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)    12126 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/news.py
+-rw-rw-rw-   0 root         (0) root         (0)    18772 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/parsers/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)     6334 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/parsers/manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/parsers/userconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/perms.py
+-rw-rw-rw-   0 root         (0) root         (0)     6911 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/prefix.py
+-rw-rw-rw-   0 root         (0) root         (0)     7092 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/prompt.py
+-rw-rw-rw-   0 root         (0) root         (0)    23081 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/pybuild.py
+-rw-rw-rw-   0 root         (0) root         (0)    26890 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod/repo/
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/repo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12708 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/repo/keywords.py
+-rw-rw-rw-   0 root         (0) root         (0)    16589 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/repo/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)    10106 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/repo/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1552 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/repo/updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     5929 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/repos.py
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/source.py
+-rw-rw-rw-   0 root         (0) root         (0)     5232 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/sync.py
+-rw-rw-rw-   0 root         (0) root         (0)    14068 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/transactions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/tsort.py
+-rw-rw-rw-   0 root         (0) root         (0)     4726 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/vdb.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-07 01:04:18.000000 portmod-2.6.2/portmod/win32.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7248 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8775 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 01:06:06.000000 portmod-2.6.2/portmod.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      675 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-07 01:16:10.000000 portmod-2.6.2/portmod.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmodlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmodlib/_deprecated/
+-rw-rw-rw-   0 root         (0) root         (0)    11502 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/_deprecated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/_deprecated/vfs.py
+-rw-rw-rw-   0 root         (0) root         (0)    10669 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/_phase.py
+-rw-rw-rw-   0 root         (0) root         (0)     7758 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/archives.py
+-rw-rw-rw-   0 root         (0) root         (0)    11301 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/atom.py
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/colour.py
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     9613 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/fs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/functools.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/globals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/l10n.py
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/masters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/module_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/portmodlib/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/parsers/list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4212 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/portmod.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9627 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/pybuild.py
+-rw-rw-rw-   0 root         (0) root         (0)     1660 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/source.py
+-rw-rw-rw-   0 root         (0) root         (0)    21357 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/usestr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    13354 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-05-07 01:04:18.000000 portmod-2.6.2/portmodlib/winreg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/pybuild/
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-05-07 01:04:18.000000 portmod-2.6.2/pybuild/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33866 2023-05-07 01:04:18.000000 portmod-2.6.2/pybuild/_pybuild.py
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2023-05-07 01:04:18.000000 portmod-2.6.2/pybuild/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-05-07 01:04:18.000000 portmod-2.6.2/pybuild/winreg.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-07 01:04:18.000000 portmod-2.6.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-05-07 01:04:18.000000 portmod-2.6.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-05-07 01:16:10.000000 portmod-2.6.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4920 2023-05-07 01:04:18.000000 portmod-2.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/src/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-07 01:04:18.000000 portmod-2.6.2/src/dds.rs
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-05-07 01:04:18.000000 portmod-2.6.2/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     9538 2023-05-07 01:04:18.000000 portmod-2.6.2/src/index.rs
+-rw-rw-rw-   0 root         (0) root         (0)    11290 2023-05-07 01:04:18.000000 portmod-2.6.2/src/lib.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/src/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)     4787 2023-05-07 01:04:18.000000 portmod-2.6.2/src/metadata/mod.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2023-05-07 01:04:18.000000 portmod-2.6.2/src/metadata/person.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2023-05-07 01:04:18.000000 portmod-2.6.2/src/news.rs
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-07 01:04:18.000000 portmod-2.6.2/src/yaml.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/_benchmarks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/test/_benchmarks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-05-07 01:04:18.000000 portmod-2.6.2/test/_benchmarks/atom.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-05-07 01:04:18.000000 portmod-2.6.2/test/_benchmarks/hash.py
+-rw-rw-rw-   0 root         (0) root         (0)     4128 2023-05-07 01:04:18.000000 portmod-2.6.2/test/_benchmarks/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     4448 2023-05-07 01:04:18.000000 portmod-2.6.2/test/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-05-07 01:04:18.000000 portmod-2.6.2/test/merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_atom.py
+-rw-rw-rw-   0 root         (0) root         (0)     6464 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_cfg_protect.py
+-rw-rw-rw-   0 root         (0) root         (0)     1435 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_clean.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_deps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_download.py
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2434 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_existing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_fs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_gui_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3564 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_gui_installed_packages_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_gui_packages.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_init.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_inquisitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7428 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_keywords.py
+-rw-rw-rw-   0 root         (0) root         (0)    24407 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_log.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_masters.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_obscure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1884 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_portmod_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1997 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_prefix_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_resolve.py
+-rw-rw-rw-   0 root         (0) root         (0)     2706 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_select.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_unpack.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4235 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_use.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_vdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     6518 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7996 2023-05-07 01:04:18.000000 portmod-2.6.2/test/test_vfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/common/masked/
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/common/masked/masked-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/common/superclass/
+-rw-rw-rw-   0 root         (0) root         (0)      472 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/common/superclass/superclass-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/licenses/CC-BY-SA-4.0
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/licenses/eula
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/licenses/free-use
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/licenses/test
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/metadata/news/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/metadata/news/2020-04-12-installed/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/metadata/news/2020-04-12-installed/2020-04-12-installed.en.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/metadata/news/2020-04-12-keyword/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/metadata/news/2020-04-12-keyword/2020-04-12-keyword.en.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/metadata/news/2020-04-12-profile/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/metadata/news/2020-04-12-profile/2020-04-12-profile.en.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/metadata/news/2020-04-12-test/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/metadata/news/2020-04-12-test/2020-04-12-test.en.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/metadata/repos.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/profiles/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/arch.list
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/profiles/base/
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/base/defaults.conf
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/categories
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/profiles/desc/
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/desc/screen_aspect.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/license_groups.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/package.mask
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/profiles.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/repo_name
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/profiles/test/
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/test/packages
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/test/parent
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/profiles/test-config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/test-config/defaults.conf
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/test-config/parent
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/profiles/test-unstable/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/test-unstable/defaults.conf
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/test-unstable/parent
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/profiles/updates/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/updates/2Q-2020
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/use.alias.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/profiles/use.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/masked/
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/masked/masked-1.0.pybuild
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/masked/masked-1.1.pybuild
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/metadata.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/quill-of-feyfolken/
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/quill-of-feyfolken/Manifest
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/quill-of-feyfolken/metadata.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      723 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/quill-of-feyfolken/quill-of-feyfolken-2.0.2-r1.pybuild
+-rw-rw-rw-   0 root         (0) root         (0)      724 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/quill-of-feyfolken/quill-of-feyfolken-2.0.2.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test/metadata.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      736 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test/test-1.0-r1.pybuild
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test/test-1.0-r2.pybuild
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test/test-1.0.pybuild
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test/test-2.0.pybuild
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test/test-2.0_rc1.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test-eula/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test-eula/test-eula-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test-install/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test-install/Manifest
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test-install/files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test-install/files/file
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test-install/test-install-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test-module/
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test-module/test-module-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test-new/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test-new/test-new-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test-nofetch/
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test-nofetch/Manifest
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test-nofetch/test-nofetch-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test-useless/
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test-useless/test-useless-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test0/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test0/test0-1.0_rc1.pybuild
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test0/test0-2.0_alpha.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test2/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test2/test2-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test3/
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test3/test3-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test4/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test4/metadata.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test4/test4-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test5/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test5/test5-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test6/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test6/test6-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/test/testrepo/test/test7/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test7/test7-0.1.pybuild
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-05-07 01:04:18.000000 portmod-2.6.2/test/testrepo/test/test7/test7-1.0.pybuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 01:16:10.000000 portmod-2.6.2/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-07 01:04:18.000000 portmod-2.6.2/tools/update_header.py
```

### Comparing `portmod-2.6.1/.appveyor.yml` & `portmod-2.6.2/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/.coveragerc` & `portmod-2.6.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/.gitlab/issue_templates/Bug.md` & `portmod-2.6.2/.gitlab/issue_templates/Bug.md`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/.gitlab-ci.yml` & `portmod-2.6.2/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y
     export PATH="/opt/python/cp37-cp37m/bin:$HOME/.cargo/bin:$PATH"
     pip install -U twine "setuptools!=50.0" setuptools_rust wheel --cache-dir .cache/pip
     pip install .[man] --cache-dir .cache/pip
     python setup.py build_rust --inplace --release build_man
     # Remove in-place library so it doesn't get included in the wheel
     rm portmodlib/*.so
+    rm build -r
     python setup.py bdist_wheel --py-limited-api=cp37
     python setup.py check sdist
     for whl in dist/*.whl; do
         auditwheel repair "$whl" -w dist/
         rm $whl
     done
     python -m twine upload dist/*
```

### Comparing `portmod-2.6.1/.pre-commit-config.yaml` & `portmod-2.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/.pre-commit-hooks.yaml` & `portmod-2.6.2/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/CHANGELOG.md` & `portmod-2.6.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # Changelog
 
 
 ## [Unreleased]
 
+## [2.6.2] 2023-05-06
+### Docs
+- Added simple pybuild example to dev guide.
+
+### Fixed
+- Fixed caching bug when switching between prefixes which use different versions
+  of a `common` superclass due to masking (#412).
+- The `pybuild` module can now be imported outside of the packaging environment (#394).
+
 ## [2.6.1] 2023-04-17
 
 ### Fixed
 - Fixed dependencies of `man` extra so that manpages build properly.
 
 ## [2.6.0] 2023-04-15
```

### Comparing `portmod-2.6.1/Cargo.lock` & `portmod-2.6.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/Cargo.toml` & `portmod-2.6.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/LICENSE` & `portmod-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/PKG-INFO` & `portmod-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portmod
-Version: 2.6.1
+Version: 2.6.2
 Summary: A CLI package manager for mods
 Home-page: https://gitlab.com/portmod/portmod
 Download-URL: https://gitlab.com/portmod/portmod/-/releases
 Author: Portmod Authors
 Author-email: incoming+portmod-portmod-9660349-issue-@incoming.gitlab.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `portmod-2.6.1/README.md` & `portmod-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/code_of_conduct.md` & `portmod-2.6.2/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/default.nix` & `portmod-2.6.2/default.nix`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/Makefile` & `portmod-2.6.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/_build/man/man1/inquisitor.1` & `portmod-2.6.2/doc/_build/man/man1/inquisitor.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "INQUISITOR" "1" "Apr 17, 2023" "Portmod 2.6.1" "Portmod"
+.TH "INQUISITOR" "1" "May 07, 2023" "Portmod 2.6.2" "Portmod"
 .SH NAME
 inquisitor \- CLI QA tool
 .sp
 Quality assurance program for the package repository
 
 .INDENT 0.0
 .INDENT 3.5
```

### Comparing `portmod-2.6.1/doc/_build/man/man1/portmod.1` & `portmod-2.6.2/doc/_build/man/man1/portmod.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "PORTMOD" "1" "Apr 17, 2023" "Portmod 2.6.1" "Portmod"
+.TH "PORTMOD" "1" "May 07, 2023" "Portmod 2.6.2" "Portmod"
 .SH NAME
 portmod \- Main portmod CLI interface
 .sp
 CLI Package manager designed for packaging game mods
 
 .INDENT 0.0
 .INDENT 3.5
```

### Comparing `portmod-2.6.1/doc/_build/man/man3/pybuild.3` & `portmod-2.6.2/doc/_build/man/man3/pybuild.3`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "PYBUILD" "3" "Apr 17, 2023" "Portmod 2.6.1" "Portmod"
+.TH "PYBUILD" "3" "May 07, 2023" "Portmod 2.6.2" "Portmod"
 .SH NAME
 pybuild \- Pybuild API
 .SH SUBMODULES
 .TS
 center;
 |l|l|.
 _
```

### Comparing `portmod-2.6.1/doc/_build/man/man5/portmod.5` & `portmod-2.6.2/doc/_build/man/man5/portmod.5`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "PORTMOD" "5" "Apr 17, 2023" "Portmod 2.6.1" "Portmod"
+.TH "PORTMOD" "5" "May 07, 2023" "Portmod 2.6.2" "Portmod"
 .SH NAME
 portmod \- Configuration files for portmod
 .sp
 These files are found in the \fBCONFIG_DIR\fP (as displayed by \fBportmod <prefix> info\fP).
 This is typically one of the following locations, depending on your platform.
 .TS
 center;
```

### Comparing `portmod-2.6.1/doc/_build/man/man5/pybuild.5` & `portmod-2.6.2/doc/_build/man/man5/pybuild.5`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "PYBUILD" "5" "Apr 17, 2023" "Portmod 2.6.1" "Portmod"
+.TH "PYBUILD" "5" "May 07, 2023" "Portmod 2.6.2" "Portmod"
 .SH NAME
 pybuild \- Portmod Repositories and related files
 .sp
 Repositories have the following basic file structure:
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -43,344 +43,70 @@
 \&./CATEGORY_NAME/PACKAGE_NAME/PACKAGE_NAME\-OTHER_VER.pybuild
 \&./CATEGORY_NAME/PACKAGE_NAME/Manifest
 \&./CATEGORY_NAME/PACKAGE_NAME/metadata.yaml
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-.SH PROFILES
-.SS Profiles
-.sp
-Profiles are used to provide preset configurations for users.
-.SS profiles.yaml
-.sp
-The file \fBprofiles/profiles.yaml\fP describes the available profiles. It
-contains a mapping with the architecture as the key at the root,
-followed by a mapping of profile paths to profile stability keywords
-(either stable or unstable). These paths should refer to a directory
-within the profiles directory.
-.sp
-E.g.
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-openmw:
-    dev: unstable
-    default/openmw/1.0: stable
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-.SS Profile Files
-.sp
-Within each profile directory the following files can be used to
-customize the profile.
-.INDENT 0.0
-.IP \(bu 2
-\fI\%packages\fP
-.IP \(bu 2
-\fI\%package.mask\fP
-.IP \(bu 2
-\fI\%package.use\fP
-.IP \(bu 2
-\fI\%use.force\fP
-.IP \(bu 2
-\fI\%package.use.force\fP
-.IP \(bu 2
-\fI\%parent\fP
-.IP \(bu 2
-\fI\%license_groups.yaml\fP
-.IP \(bu 2
-\fI\%defaults.conf\fP
-.UNINDENT
-.SS packages
-.sp
-A list of atoms to be included in the system set and thus installed by
-default. Each line to be included in the system set should start with an
-asterisk (\fB*\fP), followed by the atom to include. Lines not beginning
-in an asterisk will be ignored.
-.SS package.mask
-.sp
-A profile\-specific list of masked packages.
-.sp
-See \fI\%package.mask\fP
-.SS package.use
-.sp
-Default per\-package use flags. The file can contain comments (starting
-with \fB#\fP) and lines containing a qualified atom (i.e.\ containing a
-category, can also include versions and operators) followed by a
-whitespace\-separated list of flags. Flags can be disabled by prefixing
-them with a \fB\-\fP\&.
-.sp
-See \fI\%package.use\fP
-.SS use.force
+.SH CATEGORIES
 .sp
-Global use flags that are required to always be enabled in this profile.
-The format is the same as the contents of the \fBUSE\fP variable in
-\fI\%defaults.conf\fP\&.
-.SS package.use.force
+Any category must be listed in \fBprofiles/categories\fP and contain a
+\fI\%metadata.yaml\fP file.
+.SH PACKAGE DIRECTORIES
+.SS Package Files
 .sp
-Per\-package use flags that are required to always be enabled in this
-profile. The format is the same as package.use.
-.SS parent
+Package files can be created as python\-like pybuild files.
 .sp
-Defines another directory (via relative path) to be included in the
-current profile. This allows profiles to share configuration, and it is
-recommended that all profiles include the \fBprofiles/base\fP directory in
-their hierarchy.
-.SS license_groups.yaml
+See the API for more details about available fields and functions.
 .sp
-A mapping of license group names to the licenses in the group. Licenses should be a whitespace\-separated list.
-Licenses listed are merged with the license groups in master repositories.
+Note that this guide is deliberately very simple. Many game engines require custom
+installation options to register mods, so portmod package repositories generally
+provide custom superclasses for use in packages to ensure that any required configuration
+is updated. See the guides on \fI\%The Wiki\fP\&.
+.SS Pybuild Packages
 .sp
-The special \fBREDISTRIBUTABLE\fP license group is used to determine if a package can be mirrored (and also if mirrors should be checked when fetching the file).
+Pybuild files have a syntax which is equivalent to python 3.7, not including restricted
+syntax listed on the \fI\%Sandbox\fP page.
 .sp
-E.g.
+They should generally follow a structure similar to the following example:
 .sp
-profiles/license_groups.yaml
+\fBexample\-suite\-0.17.pybuild\fP
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-REDISTRIBUTABLE: CC\-BY CC\-0 GPL\-3
+import os
+import shutil
+from pybuild import Pybuild2
+from pybuild.info import PV
+
+
+class Package(Pybuild2):
+    NAME = \(dqExample Suite\(dq
+    DESC = \(dqA demo showing the capabilities of the OpenMW engine\(dq
+    HOMEPAGE = \(dqhttps://github.com/OpenMW/example\-suite\(dq
+    LICENSE = \(dqCC\-BY\-3.0 CC\-BY\-SA\-3.0 CC\-BY\-4.0\(dq
+    RDEPEND = \(dq!!base/morrowind\(dq
+    KEYWORDS = \(dq~openmw\(dq
+    SRC_URI = f\(dq\(dq\(dq
+        https://github.com/OpenMW/example\-suite/releases/download/{PV}/ExampleSuiteVersion{PV}.7z
+    \(dq\(dq\(dq
+    S = f\(dqExampleSuiteVersion{PV}/openmw\-template\(dq
+    # Actually included in the default DOCS, but note that the working directory must be correct
+    # for them to recognized since subdirectories won\(aqt be searched.
+    DOCS = [\(dqAUTHORS.md\(dq, \(dqCHANGELOG.md\(dq, \(dqREADME.md\(dq]
+
+    def src_install(self):
+        os.makedirs(os.path.join(self.D, \(dqpkg\(dq, \(dqbase\(dq))
+        shutil.move(\(dqdata\(dq, os.path.join(self.D, \(dqpkg\(dq, \(dqbase\(dq, \(dqexample\-suite\(dq))
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-.SS defaults.conf
-.sp
-The format is the same as \fI\%portmod.conf\fP, but additional
-variables are available. Also note that unlike the user\-defined
-defaults.conf, variables defined in defaults.conf which are not listed
-on this page will not be set as environment variables (this is for
-security reasons, as there are variables such as PATH which could be
-abused).
-.sp
-As portmod.conf is a python file (albeit a restricted subset of the
-language), other variables defined earlier in the same file can be
-referenced directly. Additionally, you can reference the final value of
-a variable using string templating. I.e. strings containing values of
-the form \fB${VAR}\fP will be substituted for the final value of the
-referenced variable once all conf files have been parsed.
-.sp
-Collapsible Variables
-.sp
-These variables contain whitespace\-delimited sets (as strings), the
-entries of which can be disabled (if enabled in a previously loaded conf
-file) by prefixing them with a minus/hyphen (\fB\-\fP).
-.TS
-center;
-|l|l|.
-_
-T{
-Variable
-T}	T{
-Description
-T}
-_
-T{
-USE
-T}	T{
-Enabled use flags. These provide the
-profile default enabled use flags.
-T}
-_
-T{
-ACCEPT_LICENSE
-T}	T{
-A list of accepted licenses. License
-groups, as specified in
-profiles/\fI\%license_groups.yaml\fP,
-can be included by prefixing the group
-name with an \fB@\fP\&. An asterisk
-(\fB*\fP) can be used to accept all
-licenses by default, with the ability
-to disable specific licenses by
-default by prefixing them with \fB\-\fP\&.
-Recommended defaults are \fB* \-@EULA\fP
-or \fB@FREE\fP\&.
-T}
-_
-T{
-ACCEPT_KEYWORDS
-T}	T{
-The default keywords to accept. Should
-usually only contain
-T}
-_
-T{
-INFO_VARS
-T}	T{
-Variables to display when
-\fBportmod <prefix> info\fP is run.
-T}
-_
-T{
-INFO_PACKAGES
-T}	T{
-Packages to display when
-\fBportmod <prefix> info\fP is run.
-T}
-_
-T{
-USE_EXPAND
-T}	T{
-The names of USE_EXPAND variables. The
-values they can take should be
-described in the \fBprofiles/desc\fP
-directory in a yaml file with a name
-equal to the lowercased variable name,
-followed by \fB\&.yaml\fP\&.
-T}
-_
-T{
-USE_EXPAND_HIDDEN
-T}	T{
-A subset of USE_EXPAND that should be
-hidden to the user and not show up in
-searches and transaction lists.
-T}
-_
-T{
-PROFILE_ONLY_VARIABLES
-T}	T{
-This defines which variables cannot be
-modified by the user in their
-portmod.conf (technically,
-portmod.conf can configure everything
-that defaults.conf can, with the
-exception of the variables listed
-here). Note that users can still use
-\fI\%profile.user\fP
-to create a custom
-profile and override these variables.
-T}
-_
-T{
-CACHE_FIELDS
-T}	T{
-A list of fields that should be cached
-(e.g.\ fields that may be added by
-classes in this repo which it would be
-useful to have accessible to external
-software).
-T}
-_
-.TE
-.sp
-Other Variables
-.TS
-center;
-|l|l|.
-_
-T{
-Variable
-T}	T{
-Description
-T}
-_
-T{
-ARCH
-T}	T{
-The architecture for the profile. See
-\fIarch.list\fP\&. This is set automatically
-and should not be modified
-T}
-_
-T{
-ARCH_VERSION
-T}	T{
-The architecture\(aqs version.
-This is set before the profile is
-loaded by a special script.
-See \fI\%Architecture Versioning\fP for details.
-T}
-_
-T{
-TEXTURE_SIZE
-T}	T{
-The algorithm for choosing texture
-size. See \fI\%portmod.conf\fP
-T}
-_
-T{
-PORTMOD_MIRRORS
-T}	T{
-The list of download mirrors. See
-\fI\%portmod.conf\fP
-T}
-_
-T{
-CASE_INSENSITIVE_FILES
-T}	T{
-Whether or not files in the VFS should
-be case\-insensitive. When enabled,
-portmod will treat files of identical
-path other than their case as the same
-when installing. Otherwise, such files
-may be installed side by side instead
-of overriding each other.
-T}
-_
-T{
-OMWMERGE_DEFAULT_OPTS
-T}	T{
-The default options passed to
-\fBportmod <prefix> merge\fP\&. See
-\fI\%portmod.conf\fP
-T}
-_
-T{
-MODULEPATH
-T}	T{
-The directory (relative to \fBROOT\fP)
-which stores \fI\%Modules\fP\&.
-T}
-_
-T{
-DOC_DEST
-T}	T{
-The default installation directory
-for documentation when the \fIdodoc\fP
-function is called.
-T}
-_
-T{
-VARIABLE_DATA
-T}	T{
-The directory, relative to \fBROOT\fP
-should contain generated portmod files
-such as the package database.
-.sp
-This variable should never be changed
-since it takes effect immediately.
-Instead, it is recommended to create
-a new profile with a new value and
-a migration tool to update the
-filesystem.
-T}
-_
-T{
-CFG_PROTECT
-T}	T{
-A glob\-style patterns (or list of
-patterns) indicating files which
-should not be overwritten on
-installation if they have been
-modified since the file was first
-installed. Instead, a \fB\&.new\fP file
-will be created and users will be able
-to run the cfg updater to merge the
-modifications.
-T}
-_
-.TE
 .SS metadata.yaml
 .sp
 metadata.yaml files are used to store additional information about mods
 and categories. Note that no information stored in metadata.yaml should
 be specific to a particular version of a mod.
 .TS
 center;
@@ -616,68 +342,123 @@
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 When categories are created, a metadata.yaml containing a
 longdescription is required.
-.SS layout.conf
+.SS Manifest
 .sp
-Describes the repository metadata.
+In the tree, every package has a \fBManifest\fP file. The Manifest file contains
+various hashes and file size data for every external source that is to
+be fetched. This is used primarily to verify the integrity of external files.
+.SS Generating the Manifest
+.sp
+To generate the Manifest, use \fBinquisitor manifest foo.pybuild\fP\&. When
+new sources are added or removed, the \fBManifest\fP must be regenerated.
+.SS Structure
 .sp
-E.g.
+Manifest files are plain text files with the following format:
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-# Comments can be included
-masters = \(dqpython openmw\(dq
-
-# 2 is new, so it\(aqs not a bad idea to stick with 1 for now
-pybuild_versions_banned = [2]
-
-# Obviously this isn\(aqt helpful if you also include the above statement,
-# But eventually you will want to deprecate Pybuild1 since support for
-# it will be dropped.
-pybuild_versions_deprecated = [1]
+<type> <filename> <size> <hash\-type> <hash> [<hash\-type> <hash> ...]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
-.SS Fields
-.SS masters
-.sp
-A space\-separated string list of repository masters
-.SS pybuild_versions_banned
-.sp
-A python list of banned pybuild versions. E.g. if this list includes \fB2\fP, \fI\%pybuild.Pybuild2\fP will be considered banned and will not be able to be loaded. \fI\%inquisitor\fP will also produce an error for packages which use banned pybuild versions.
+.SS Members
+.TS
+center;
+|l|l|.
+_
+T{
+\fBtype\fP
+T}	T{
+The type of the file. Supported types are \fBDIST\fP (for remote package sources) and \fBLINK\fP and \fBMISC\fP (used internally for \fBCONTENTS\fP files in the package DB).
+T}
+_
+T{
+\fBfilename\fP
+T}	T{
+The name of the file the manifest entry references.
+T}
+_
+T{
+\fBsize\fP
+T}	T{
+The size of the file as a decimal number, in bytes
+T}
+_
+T{
+\fBhash\-type\fP
+T}	T{
+One of the supported hash types listed below
+T}
+_
+T{
+\fBhash\fP
+T}	T{
+The hash of the file as a hexadecimal number, matching the preceeding hash type.
+T}
+_
+.TE
+.SS Supported Hash Types
 .sp
-This is primarily a QA feature, but is also enforced at runtime.
-.SS pybuild_versions_deprecated
+The hashes currently supported by portmod are:
+.INDENT 0.0
+.IP \(bu 2
+BLAKE2B
+.IP \(bu 2
+BLAKE3 (recommended for performance)
+.IP \(bu 2
+MD5
+.IP \(bu 2
+SHA256 (SHA\-2)
+.IP \(bu 2
+SHA512 (SHA\-2)
+.UNINDENT
+.SS External Resources
 .sp
-A python list of deprecated pybuild versions. E.g. if this list includes \fB2\fP, \fI\%pybuild.Pybuild2\fP will be considered deprecated and \fI\%inquisitor\fP will emit a warning when encountering packages which use it.
-.SS Syntax
+\fI\%https://wiki.gentoo.org/wiki/Repository_format/package/Manifest\fP
 .sp
-Same as \fI\%defaults.conf\fP\&. I.e. a restricted subset of python using only basic primitives and no imports.
-.SH CATEGORIES
+Package directories must be in a subdirectory of a category and their
+directory name should be the same as the base name of the package files
+(excluding version).
 .sp
-Any category must be listed in \fBprofiles/categories\fP and contain a
-\fI\%metadata.yaml\fP file.
-.SH PACKAGES
+E.g.
+.INDENT 0.0
+.INDENT 3.5
 .sp
-Mod directories must be in a subdirectory of a category and their
-directory name should be the same as the base name of the mod’s pybuilds
-(excluding version).
+.nf
+.ft C
+category/example\-package
+├── files
+│\ \  └── some\-extra\-file.txt
+├── Manifest
+├── metadata.yaml
+└── example\-package\-1.0.pybuild
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
 .sp
-The \fBManifest\fP file is optional, but is required to contain a manifest
-entry for each source file listed in SRC_URI (i.e.\ only optional for
+The \fI\%Manifest\fP file is optional, but is required to contain a manifest
+entry for each source file listed in \fI\%SRC_URI\fP (i.e.\ only optional for
 pybuilds without sources).
 .sp
 \fI\%metadata.yaml\fP is optional.
+.sp
+One or more package files must be included. These files must begin with the \fI\%package name\fP, followed by a hyphen, then the \fI\%package version\fP, and end in \fB\&.pybuild\fP\&. For details on the content of packages, see \fI\%Package Files\fP\&.
+.sp
+Optionally, extra files can be distributed with the package in the \fBfiles\fP directory.
+These should be small, plaintext files such as patch files, and can be referred to in
+installation scripts via the \fI\%FILESDIR\fP attribute.
 .SH PROFILES DIRECTORY
 .sp
 The files in profiles are optional, except for repo_name.
 .TS
 center;
 |l|l|.
 _
@@ -761,15 +542,385 @@
 T}	T{
 A directory containing USE_EXPAND descriptor
 files. Each file has the same form as
 \fBuse.yaml\fP\&.
 T}
 _
 .TE
+.sp
+Additionally, there are a number of files related to specific profiles. See \fI\%Profiles\fP\&.
+.SS Profiles
+.sp
+Profiles are used to provide preset configurations for users.
+.SS profiles.yaml
+.sp
+The file \fBprofiles/profiles.yaml\fP describes the available profiles. It
+contains a mapping with the architecture as the key at the root,
+followed by a mapping of profile paths to profile stability keywords
+(either stable or unstable). These paths should refer to a directory
+within the profiles directory.
+.sp
+E.g.
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+openmw:
+    dev: unstable
+    default/openmw/1.0: stable
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS Profile Files
+.sp
+Within each profile directory the following files can be used to
+customize the profile.
+.INDENT 0.0
+.IP \(bu 2
+\fI\%packages\fP
+.IP \(bu 2
+\fI\%package.mask\fP
+.IP \(bu 2
+\fI\%package.use\fP
+.IP \(bu 2
+\fI\%use.force\fP
+.IP \(bu 2
+\fI\%package.use.force\fP
+.IP \(bu 2
+\fI\%parent\fP
+.IP \(bu 2
+\fI\%license_groups.yaml\fP
+.IP \(bu 2
+\fI\%defaults.conf\fP
+.UNINDENT
+.SS packages
+.sp
+A list of atoms to be included in the system set and thus installed by
+default. Each line to be included in the system set should start with an
+asterisk (\fB*\fP), followed by the atom to include. Lines not beginning
+in an asterisk will be ignored.
+.SS package.mask
+.sp
+A profile\-specific list of masked packages.
+.sp
+See \fI\%package.mask\fP
+.SS package.use
+.sp
+Default per\-package use flags. The file can contain comments (starting
+with \fB#\fP) and lines containing a qualified atom (i.e.\ containing a
+category, can also include versions and operators) followed by a
+whitespace\-separated list of flags. Flags can be disabled by prefixing
+them with a \fB\-\fP\&.
+.sp
+See \fI\%package.use\fP
+.SS use.force
+.sp
+Global use flags that are required to always be enabled in this profile.
+The format is the same as the contents of the \fBUSE\fP variable in
+\fI\%defaults.conf\fP\&.
+.SS package.use.force
+.sp
+Per\-package use flags that are required to always be enabled in this
+profile. The format is the same as package.use.
+.SS parent
+.sp
+Defines another directory (via relative path) to be included in the
+current profile. This allows profiles to share configuration, and it is
+recommended that all profiles include the \fBprofiles/base\fP directory in
+their hierarchy.
+.SS license_groups.yaml
+.sp
+A mapping of license group names to the licenses in the group. Licenses should be a whitespace\-separated list.
+Licenses listed are merged with the license groups in master repositories.
+.sp
+The special \fBREDISTRIBUTABLE\fP license group is used to determine if a package can be mirrored (and also if mirrors should be checked when fetching the file).
+.sp
+E.g.
+.sp
+profiles/license_groups.yaml
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+REDISTRIBUTABLE: CC\-BY CC\-0 GPL\-3
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS defaults.conf
+.sp
+The format is the same as \fI\%portmod.conf\fP, but additional
+variables are available. Also note that unlike the user\-defined
+defaults.conf, variables defined in defaults.conf which are not listed
+on this page will not be set as environment variables (this is for
+security reasons, as there are variables such as PATH which could be
+abused).
+.sp
+As portmod.conf is a python file (albeit a restricted subset of the
+language), other variables defined earlier in the same file can be
+referenced directly. Additionally, you can reference the final value of
+a variable using string templating. I.e. strings containing values of
+the form \fB${VAR}\fP will be substituted for the final value of the
+referenced variable once all conf files have been parsed.
+.sp
+Collapsible Variables
+.sp
+These variables contain whitespace\-delimited sets (as strings), the
+entries of which can be disabled (if enabled in a previously loaded conf
+file) by prefixing them with a minus/hyphen (\fB\-\fP).
+.TS
+center;
+|l|l|.
+_
+T{
+Variable
+T}	T{
+Description
+T}
+_
+T{
+USE
+T}	T{
+Enabled use flags. These provide the
+profile default enabled use flags.
+T}
+_
+T{
+ACCEPT_LICENSE
+T}	T{
+A list of accepted licenses. License
+groups, as specified in
+profiles/\fI\%license_groups.yaml\fP,
+can be included by prefixing the group
+name with an \fB@\fP\&. An asterisk
+(\fB*\fP) can be used to accept all
+licenses by default, with the ability
+to disable specific licenses by
+default by prefixing them with \fB\-\fP\&.
+Recommended defaults are \fB* \-@EULA\fP
+or \fB@FREE\fP\&.
+T}
+_
+T{
+ACCEPT_KEYWORDS
+T}	T{
+The default keywords to accept. Should
+usually only contain
+T}
+_
+T{
+INFO_VARS
+T}	T{
+Variables to display when
+\fBportmod <prefix> info\fP is run.
+T}
+_
+T{
+INFO_PACKAGES
+T}	T{
+Packages to display when
+\fBportmod <prefix> info\fP is run.
+T}
+_
+T{
+USE_EXPAND
+T}	T{
+The names of USE_EXPAND variables. The
+values they can take should be
+described in the \fBprofiles/desc\fP
+directory in a yaml file with a name
+equal to the lowercased variable name,
+followed by \fB\&.yaml\fP\&.
+T}
+_
+T{
+USE_EXPAND_HIDDEN
+T}	T{
+A subset of USE_EXPAND that should be
+hidden to the user and not show up in
+searches and transaction lists.
+T}
+_
+T{
+PROFILE_ONLY_VARIABLES
+T}	T{
+This defines which variables cannot be
+modified by the user in their
+portmod.conf (technically,
+portmod.conf can configure everything
+that defaults.conf can, with the
+exception of the variables listed
+here). Note that users can still use
+\fI\%profile.user\fP
+to create a custom
+profile and override these variables.
+T}
+_
+T{
+CACHE_FIELDS
+T}	T{
+A list of fields that should be cached
+(e.g.\ fields that may be added by
+classes in this repo which it would be
+useful to have accessible to external
+software).
+T}
+_
+.TE
+.sp
+Other Variables
+.TS
+center;
+|l|l|.
+_
+T{
+Variable
+T}	T{
+Description
+T}
+_
+T{
+ARCH
+T}	T{
+The architecture for the profile. See
+\fIarch.list\fP\&. This is set automatically
+and should not be modified
+T}
+_
+T{
+ARCH_VERSION
+T}	T{
+The architecture\(aqs version.
+This is set before the profile is
+loaded by a special script.
+See \fI\%Architecture Versioning\fP for details.
+T}
+_
+T{
+TEXTURE_SIZE
+T}	T{
+The algorithm for choosing texture
+size. See \fI\%portmod.conf\fP
+T}
+_
+T{
+PORTMOD_MIRRORS
+T}	T{
+The list of download mirrors. See
+\fI\%portmod.conf\fP
+T}
+_
+T{
+CASE_INSENSITIVE_FILES
+T}	T{
+Whether or not files in the VFS should
+be case\-insensitive. When enabled,
+portmod will treat files of identical
+path other than their case as the same
+when installing. Otherwise, such files
+may be installed side by side instead
+of overriding each other.
+T}
+_
+T{
+OMWMERGE_DEFAULT_OPTS
+T}	T{
+The default options passed to
+\fBportmod <prefix> merge\fP\&. See
+\fI\%portmod.conf\fP
+T}
+_
+T{
+MODULEPATH
+T}	T{
+The directory (relative to \fBROOT\fP)
+which stores \fI\%Modules\fP\&.
+T}
+_
+T{
+DOC_DEST
+T}	T{
+The default installation directory
+for documentation when the \fIdodoc\fP
+function is called.
+T}
+_
+T{
+VARIABLE_DATA
+T}	T{
+The directory, relative to \fBROOT\fP
+should contain generated portmod files
+such as the package database.
+.sp
+This variable should never be changed
+since it takes effect immediately.
+Instead, it is recommended to create
+a new profile with a new value and
+a migration tool to update the
+filesystem.
+T}
+_
+T{
+CFG_PROTECT
+T}	T{
+A glob\-style patterns (or list of
+patterns) indicating files which
+should not be overwritten on
+installation if they have been
+modified since the file was first
+installed. Instead, a \fB\&.new\fP file
+will be created and users will be able
+to run the cfg updater to merge the
+modifications.
+T}
+_
+.TE
 .SH METADATA DIRECTORY
+.SS layout.conf
+.sp
+Describes the repository metadata.
+.sp
+E.g.
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+# Comments can be included
+masters = \(dqpython openmw\(dq
+
+# 2 is new, so it\(aqs not a bad idea to stick with 1 for now
+pybuild_versions_banned = [2]
+
+# Obviously this isn\(aqt helpful if you also include the above statement,
+# But eventually you will want to deprecate Pybuild1 since support for
+# it will be dropped.
+pybuild_versions_deprecated = [1]
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS Fields
+.SS masters
+.sp
+A space\-separated string list of repository masters
+.SS pybuild_versions_banned
+.sp
+A python list of banned pybuild versions. E.g. if this list includes \fB2\fP, \fI\%pybuild.Pybuild2\fP will be considered banned and will not be able to be loaded. \fI\%inquisitor\fP will also produce an error for packages which use banned pybuild versions.
+.sp
+This is primarily a QA feature, but is also enforced at runtime.
+.SS pybuild_versions_deprecated
+.sp
+A python list of deprecated pybuild versions. E.g. if this list includes \fB2\fP, \fI\%pybuild.Pybuild2\fP will be considered deprecated and \fI\%inquisitor\fP will emit a warning when encountering packages which use it.
+.SS Syntax
+.sp
+Same as \fI\%defaults.conf\fP\&. I.e. a restricted subset of python using only basic primitives and no imports.
 .sp
 The metadata directory is optional
 .TS
 center;
 |l|l|.
 _
 T{
```

### Comparing `portmod-2.6.1/doc/_build/man/man7/portmod.7` & `portmod-2.6.2/doc/_build/man/man7/portmod.7`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "PORTMOD" "7" "Apr 17, 2023" "Portmod 2.6.1" "Portmod"
+.TH "PORTMOD" "7" "May 07, 2023" "Portmod 2.6.2" "Portmod"
 .SH NAME
 portmod \- Portmod Concepts
 .sp
 These are various concepts relevant to understanding how portmod works. It is recommended that you familiarise yourself with them before using Portmod.
 .TS
 center;
 |l|l|.
@@ -187,27 +187,28 @@
 .sp
 E.g. \fBportmod <prefix> merge \-uDN @world\fP, or
 \fBportmod <prefix> merge @rebuild\fP\&.
 .sp
 The builtin sets include:
 .INDENT 0.0
 .IP \(bu 2
-\fBworld\fP: Equivalent to \fBselected\fP + \fBsystem\fP
+\fBworld\fP: Equivalent to \fBselected\fP + \fBsystem\fP\&. This is usually the
+only set you need to interact with. It includes all packages that
+you want or need, not including their dependencies.
 .IP \(bu 2
 \fBsystem\fP: Packages required by the profile which cannot be removed.
 .IP \(bu 2
 \fBselected\fP: Equivalent to \fBselected\-sets\fP + \fBselected\-packages\fP
 .IP \(bu 2
 \fBselected\-sets\fP: User\-selected sets (not including builtin sets).
 .IP \(bu 2
 \fBselected\-packages\fP: The user\-selected list of packages. This
 includes any package you have explicitly installed (i.e.\ installed
 without the \fB\-\-oneshot/\-1\fP option). It does not include
-dependencies which were installed implicitly. This is usually the
-only set you need to interact with.
+dependencies which were installed implicitly.
 .IP \(bu 2
 \fBmodules\fP: This is an internal convenience set which is used to
 refer to portmod \fI\%Modules\fP\&.
 .IP \(bu 2
 \fBrebuild\fP: Packages are added to this set automatically for certain
 unusual packages when they are determined to need to be rebuilt. A
 warning message will be displayed when you need to use this set.
```

### Comparing `portmod-2.6.1/doc/_build/man/man7/pybuild.7` & `portmod-2.6.2/doc/_build/man/man7/pybuild.7`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "PYBUILD" "7" "Apr 17, 2023" "Portmod 2.6.1" "Portmod"
+.TH "PYBUILD" "7" "May 07, 2023" "Portmod 2.6.2" "Portmod"
 .SH NAME
 pybuild \- Portmod Packaging Guide
 .SH BASIC PACKAGING
 .SS Package Names and Versions
 .sp
 \fBNOTE:\fP
 .INDENT 0.0
@@ -172,22 +172,90 @@
 .IP \(bu 2
 \fI\%https://wiki.gentoo.org/wiki/Version_specifier\fP
 .IP \(bu 2
 \fI\%https://devmanual.gentoo.org/ebuild\-writing/file\-format/index.html#file\-naming\-rules\fP\&.
 .UNINDENT
 .sp
 Portmod\(aqs package names and versions generally follow \fI\%Section 3 of the Package Manager Specification\fP, with some exceptions. Excerpts of this section have been copied verbatim and are licensed \fI\%CC\-BY\-SA\-3.0\fP\&.
-.SS Generating the Manifest
+.SS Manifest
 .sp
 In the tree, every package has a \fBManifest\fP file. The Manifest file contains
 various hashes and file size data for every external source that is to
 be fetched. This is used primarily to verify the integrity of external files.
+.SS Generating the Manifest
 .sp
 To generate the Manifest, use \fBinquisitor manifest foo.pybuild\fP\&. When
 new sources are added or removed, the \fBManifest\fP must be regenerated.
+.SS Structure
+.sp
+Manifest files are plain text files with the following format:
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+<type> <filename> <size> <hash\-type> <hash> [<hash\-type> <hash> ...]
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS Members
+.TS
+center;
+|l|l|.
+_
+T{
+\fBtype\fP
+T}	T{
+The type of the file. Supported types are \fBDIST\fP (for remote package sources) and \fBLINK\fP and \fBMISC\fP (used internally for \fBCONTENTS\fP files in the package DB).
+T}
+_
+T{
+\fBfilename\fP
+T}	T{
+The name of the file the manifest entry references.
+T}
+_
+T{
+\fBsize\fP
+T}	T{
+The size of the file as a decimal number, in bytes
+T}
+_
+T{
+\fBhash\-type\fP
+T}	T{
+One of the supported hash types listed below
+T}
+_
+T{
+\fBhash\fP
+T}	T{
+The hash of the file as a hexadecimal number, matching the preceeding hash type.
+T}
+_
+.TE
+.SS Supported Hash Types
+.sp
+The hashes currently supported by portmod are:
+.INDENT 0.0
+.IP \(bu 2
+BLAKE2B
+.IP \(bu 2
+BLAKE3 (recommended for performance)
+.IP \(bu 2
+MD5
+.IP \(bu 2
+SHA256 (SHA\-2)
+.IP \(bu 2
+SHA512 (SHA\-2)
+.UNINDENT
+.SS External Resources
+.sp
+\fI\%https://wiki.gentoo.org/wiki/Repository_format/package/Manifest\fP
 .SS Dependencies
 .sp
 One of portmod\(aqs most useful features is automated dependency resolution.
 You can mark packages as requiring or conflicting with other packages, as well as having these relationthips be conditional on both the configuration of the package and the packages being depended on.
 .SS Runtime Dependencies
 .sp
 Most mod dependencies are runtime dependencies, that is, they are dependencies that must be satisfied eventually (so that the game can run), but may not need to be satisfied for package installation.
@@ -3045,15 +3113,17 @@
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 When you have finished working with the repository, you may want to revert your changes to repos.cfg to make sure the repository is kept up to date when you run \fBportmod sync\fP\&. Otherwise you will need to manually make sure your fork is up to date.
 .SS Packaging Mods
 .sp
-Refer to the guides on \fI\%the wiki\fP\&. The package repositories for each supported game have different packaging conventions to match the installation requirements of the engines.
+See \fI\%Package Directories\fP for the basics of the files which go into the package directory.
+.sp
+For details more specific to the game and repository you are packaging for, refer to the guides on \fI\%the wiki\fP\&. The package repositories for each supported game have different packaging conventions to match the installation requirements of the engines.
 .sp
 You may also want to consult the base \fI\%pybuild\fP documentation, which package repositories build on top of.
 .SS Custom Repositories
 .sp
 Alternatively, you can create your own package repository as described in \fI\%repos.cfg\fP\&. Full details of repository metadata are described in \fI\%Package Repositories\fP\&.
 .sp
 If you publish your custom repository other people can
```

### Comparing `portmod-2.6.1/doc/_ext/summary.py` & `portmod-2.6.2/doc/_ext/summary.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/_static/css/custom.css` & `portmod-2.6.2/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/_templates/package.rst_t` & `portmod-2.6.2/doc/_templates/package.rst_t`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/basic-usage.rst` & `portmod-2.6.2/doc/basic-usage.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/concepts/cfg-protect.rst` & `portmod-2.6.2/doc/concepts/cfg-protect.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/concepts/index.rst` & `portmod-2.6.2/doc/concepts/index.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/concepts/keywords.rst` & `portmod-2.6.2/doc/concepts/keywords.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/concepts/modules.rst` & `portmod-2.6.2/doc/concepts/modules.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/concepts/sandbox.rst` & `portmod-2.6.2/doc/concepts/sandbox.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/concepts/sets.rst` & `portmod-2.6.2/doc/concepts/sets.rst`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 You can refer to a set using ``@``, followed by the set name.
 
 E.g. ``portmod <prefix> merge -uDN @world``, or
 ``portmod <prefix> merge @rebuild``.
 
 The builtin sets include:
 
--  ``world``: Equivalent to ``selected`` + ``system``
+-  ``world``: Equivalent to ``selected`` + ``system``. This is usually the
+   only set you need to interact with. It includes all packages that
+   you want or need, not including their dependencies.
 -  ``system``: Packages required by the profile which cannot be removed.
 -  ``selected``: Equivalent to ``selected-sets`` + ``selected-packages``
 -  ``selected-sets``: User-selected sets (not including builtin sets).
 -  ``selected-packages``: The user-selected list of packages. This
    includes any package you have explicitly installed (i.e. installed
    without the ``--oneshot/-1`` option). It does not include
-   dependencies which were installed implicitly. This is usually the
-   only set you need to interact with.
+   dependencies which were installed implicitly.
 -  ``modules``: This is an internal convenience set which is used to
    refer to portmod :ref:`modules`.
 -  ``rebuild``: Packages are added to this set automatically for certain
    unusual packages when they are determined to need to be rebuilt. A
    warning message will be displayed when you need to use this set.
 
 You can also create custom :ref:`user-sets`
```

### Comparing `portmod-2.6.1/doc/concepts/use-flags.rst` & `portmod-2.6.2/doc/concepts/use-flags.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/conf.py` & `portmod-2.6.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/config/index.rst` & `portmod-2.6.2/doc/config/index.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/config/package.accept_keywords.rst` & `portmod-2.6.2/doc/config/package.accept_keywords.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/config/package.accept_license.rst` & `portmod-2.6.2/doc/config/package.accept_license.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/config/package.mask.rst` & `portmod-2.6.2/doc/config/package.mask.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/config/package.use.rst` & `portmod-2.6.2/doc/config/package.use.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/config/portmod.conf.rst` & `portmod-2.6.2/doc/config/portmod.conf.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/config/profile.user.rst` & `portmod-2.6.2/doc/config/profile.user.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/config/repos.cfg.rst` & `portmod-2.6.2/doc/config/repos.cfg.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/config/sets.rst` & `portmod-2.6.2/doc/config/sets.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/arch_version.rst` & `portmod-2.6.2/doc/dev/arch_version.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/archives.rst` & `portmod-2.6.2/doc/dev/archives.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/common.rst` & `portmod-2.6.2/doc/dev/common.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _common:
+
 Common Packages
 ===============
 
 Packages in the `common` category are a special type of package which can be imported within other packages without needing to be installed.
 
 E.g. Usage
```

### Comparing `portmod-2.6.1/doc/dev/dependencies.rst` & `portmod-2.6.2/doc/dev/dependencies.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/index.rst` & `portmod-2.6.2/doc/dev/index.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/l10n.rst` & `portmod-2.6.2/doc/dev/l10n.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/modules.rst` & `portmod-2.6.2/doc/dev/modules.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/naming.rst` & `portmod-2.6.2/doc/dev/naming.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 Category Names
 --------------
 
 A category name may contain any of the characters ``[A-Za-z0-9+_.-]``.
 It must not begin with a hyphen, a dot or a plus sign.
 
+.. _package-name:
+
 Package Names
 -------------
 
 A package name may contain any of the characters ``[A-Za-z0-9+_-]``.
 It must not begin with a hyphen or a plus sign, and must not end in a
 hyphen followed by anything matching the :ref:`version-syntax`.
```

### Comparing `portmod-2.6.1/doc/dev/packages.rst` & `portmod-2.6.2/doc/dev/packages.rst`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,17 @@
    auto_sync = False
    ...
 
 When you have finished working with the repository, you may want to revert your changes to repos.cfg to make sure the repository is kept up to date when you run ``portmod sync``. Otherwise you will need to manually make sure your fork is up to date.
 
 Packaging Mods
 ~~~~~~~~~~~~~~
-Refer to the guides on `the wiki <https://gitlab.com/portmod/portmod/-/wikis/home>`_. The package repositories for each supported game have different packaging conventions to match the installation requirements of the engines.
+See :ref:`package-directories` for the basics of the files which go into the package directory.
+
+For details more specific to the game and repository you are packaging for, refer to the guides on `the wiki <https://gitlab.com/portmod/portmod/-/wikis/home>`_. The package repositories for each supported game have different packaging conventions to match the installation requirements of the engines.
 
 You may also want to consult the base :py:mod:`pybuild` documentation, which package repositories build on top of.
 
 Custom Repositories
 ~~~~~~~~~~~~~~~~~~~
 
 Alternatively, you can create your own package repository as described in :ref:`repos.cfg`. Full details of repository metadata are described in :ref:`repositories`.
```

### Comparing `portmod-2.6.1/doc/dev/repo/index.rst` & `portmod-2.6.2/doc/dev/repo/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -13,43 +13,60 @@
    ./profiles/repo_name
    ./CATEGORY_NAME/metadata.yaml
    ./CATEGORY_NAME/PACKAGE_NAME/PACKAGE_NAME-VER.pybuild
    ./CATEGORY_NAME/PACKAGE_NAME/PACKAGE_NAME-OTHER_VER.pybuild
    ./CATEGORY_NAME/PACKAGE_NAME/Manifest
    ./CATEGORY_NAME/PACKAGE_NAME/metadata.yaml
 
-Profiles
---------
-
-.. toctree::
-   :maxdepth: 2
-
-   profiles
-   metadata.yaml
-   layout.conf
-
 Categories
 ----------
 
 Any category must be listed in ``profiles/categories`` and contain a
 :ref:`metadata.yaml` file.
 
-Packages
---------
+.. _package-directories:
 
-Mod directories must be in a subdirectory of a category and their
-directory name should be the same as the base name of the mod’s pybuilds
+Package Directories
+-------------------
+
+.. toctree::
+   :maxdepth: 1
+
+   package-files
+   metadata.yaml
+   ../manifest
+
+Package directories must be in a subdirectory of a category and their
+directory name should be the same as the base name of the package files
 (excluding version).
 
-The ``Manifest`` file is optional, but is required to contain a manifest
-entry for each source file listed in SRC_URI (i.e. only optional for
+E.g.
+
+.. code:: sh
+
+  category/example-package
+  ├── files
+  │   └── some-extra-file.txt
+  ├── Manifest
+  ├── metadata.yaml
+  └── example-package-1.0.pybuild
+
+
+The :ref:`Manifest` file is optional, but is required to contain a manifest
+entry for each source file listed in :py:attr:`SRC_URI <pybuild.Pybuild2.SRC_URI>` (i.e. only optional for
 pybuilds without sources).
 
 :ref:`metadata.yaml` is optional.
 
+One or more package files must be included. These files must begin with the :ref:`package name <package-name>`, followed by a hyphen, then the :ref:`package version <version-syntax>`, and end in ``.pybuild``. For details on the content of packages, see :ref:`package-files`.
+
+Optionally, extra files can be distributed with the package in the ``files`` directory.
+These should be small, plaintext files such as patch files, and can be referred to in
+installation scripts via the :py:attr:`FILESDIR <pybuild.Pybuild2.FILESDIR>` attribute.
+
 Profiles Directory
 ------------------
 
 The files in profiles are optional, except for repo_name.
 
 +------------------+---------------------------------------------------+
 | File             | Description                                       |
@@ -92,17 +109,30 @@
 |                  | of use flag names to package atoms.               |
 +------------------+---------------------------------------------------+
 | desc             | A directory containing USE_EXPAND descriptor      |
 |                  | files. Each file has the same form as             |
 |                  | ``use.yaml``.                                     |
 +------------------+---------------------------------------------------+
 
+
+Additionally, there are a number of files related to specific profiles. See :ref:`profiles`.
+
+.. toctree::
+   :maxdepth: 3
+
+   profiles
+
 Metadata Directory
 ------------------
 
+.. toctree::
+   :maxdepth: 1
+
+   layout.conf
+
 The metadata directory is optional
 
 .. list-table::
    :widths: 25 75
    :header-rows: 1
 
    * - File
```

### Comparing `portmod-2.6.1/doc/dev/repo/layout.conf.rst` & `portmod-2.6.2/doc/dev/repo/layout.conf.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/repo/metadata.yaml.rst` & `portmod-2.6.2/doc/dev/repo/metadata.yaml.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/repo/profiles.rst` & `portmod-2.6.2/doc/dev/repo/profiles.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/setup.rst` & `portmod-2.6.2/doc/dev/setup.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/dev/use-flags.rst` & `portmod-2.6.2/doc/dev/use-flags.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/index.rst` & `portmod-2.6.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/install/index.rst` & `portmod-2.6.2/doc/install/index.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/install/windows.rst` & `portmod-2.6.2/doc/install/windows.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/make.bat` & `portmod-2.6.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/doc/setup.rst` & `portmod-2.6.2/doc/setup.rst`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/l10n/en-GB/gui.ftl` & `portmod-2.6.2/l10n/en-GB/gui.ftl`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/l10n/en-GB/main.ftl` & `portmod-2.6.2/l10n/en-GB/main.ftl`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/l10n/fr/main.ftl` & `portmod-2.6.2/l10n/fr/main.ftl`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/l10n/sv-SE/main.ftl` & `portmod-2.6.2/l10n/sv-SE/main.ftl`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/__init__.py` & `portmod-2.6.2/portmod/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/cfg_update.py` & `portmod-2.6.2/portmod/_cli/cfg_update.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/destroy.py` & `portmod-2.6.2/portmod/_cli/destroy.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/init.py` & `portmod-2.6.2/portmod/_cli/init.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/inquisitor.py` & `portmod-2.6.2/portmod/_cli/inquisitor.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/main.py` & `portmod-2.6.2/portmod/_cli/main.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/merge.py` & `portmod-2.6.2/portmod/_cli/merge.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/mirror.py` & `portmod-2.6.2/portmod/_cli/mirror.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/pybuild.py` & `portmod-2.6.2/portmod/_cli/pybuild.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/query.py` & `portmod-2.6.2/portmod/_cli/query.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/run.py` & `portmod-2.6.2/portmod/_cli/run.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/search.py` & `portmod-2.6.2/portmod/_cli/search.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/select.py` & `portmod-2.6.2/portmod/_cli/select.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/sync.py` & `portmod-2.6.2/portmod/_cli/sync.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/use.py` & `portmod-2.6.2/portmod/_cli/use.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_cli/validate.py` & `portmod-2.6.2/portmod/_cli/validate.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_deprecated/rebuild.py` & `portmod-2.6.2/portmod/_deprecated/rebuild.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_deprecated/vfs.py` & `portmod-2.6.2/portmod/_deprecated/vfs.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_deps/__init__.py` & `portmod-2.6.2/portmod/_deps/__init__.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_deps/formula.py` & `portmod-2.6.2/portmod/_deps/formula.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_deps/tokens.py` & `portmod-2.6.2/portmod/_deps/tokens.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_deps/weights.py` & `portmod-2.6.2/portmod/_deps/weights.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/Manage/FlagListModel.py` & `portmod-2.6.2/portmod/_gui/Manage/FlagListModel.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/Manage/InstalledPackagesModel.py` & `portmod-2.6.2/portmod/_gui/Manage/InstalledPackagesModel.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/Manage/InstalledPackagesPanel.qml` & `portmod-2.6.2/portmod/_gui/Manage/InstalledPackagesPanel.qml`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/Manage/ManageTab.qml` & `portmod-2.6.2/portmod/_gui/Manage/ManageTab.qml`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/Manage/PackageDetailsPanel.qml` & `portmod-2.6.2/portmod/_gui/Manage/PackageDetailsPanel.qml`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/Search/SearchPackagesModel.py` & `portmod-2.6.2/portmod/_gui/Search/SearchPackagesModel.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/Search/SearchTab.qml` & `portmod-2.6.2/portmod/_gui/Search/SearchTab.qml`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/__init__.py` & `portmod-2.6.2/portmod/_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/config.py` & `portmod-2.6.2/portmod/_gui/config.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/human_bytes.py` & `portmod-2.6.2/portmod/_gui/human_bytes.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/main.qml` & `portmod-2.6.2/portmod/_gui/main.qml`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/_gui/packages.py` & `portmod-2.6.2/portmod/_gui/packages.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/cache.py` & `portmod-2.6.2/portmod/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,14 +134,18 @@
     if path in cache._failed:
         raise PreviouslyEncounteredException(cache._failed[path])
 
     atom = get_atom_from_path(path)
     repo_name = atom.R
     if installed:
         cache_file = os.path.join(env.prefix().PYBUILD_INSTALLED_CACHE, atom.C, atom.PF)
+    elif env.PREFIX_NAME:
+        cache_file = os.path.join(
+            env.prefix().PYBUILD_CACHE, repo_name, atom.C, atom.PF
+        )
     else:
         cache_file = os.path.join(env.PYBUILD_CACHE_DIR, repo_name, atom.C, atom.PF)
 
     if not cache_valid(path, cache_file):
         from .loader import SandboxedError
 
         os.makedirs(os.path.dirname(cache_file), exist_ok=True)
```

### Comparing `portmod-2.6.1/portmod/cfg_protect.py` & `portmod-2.6.2/portmod/cfg_protect.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/config/__init__.py` & `portmod-2.6.2/portmod/config/__init__.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/config/license.py` & `portmod-2.6.2/portmod/config/license.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/config/mask.py` & `portmod-2.6.2/portmod/config/mask.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/config/profiles.py` & `portmod-2.6.2/portmod/config/profiles.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/config/pyconf.py` & `portmod-2.6.2/portmod/config/pyconf.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/config/sets.py` & `portmod-2.6.2/portmod/config/sets.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/config/textures.py` & `portmod-2.6.2/portmod/config/textures.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/config/use.py` & `portmod-2.6.2/portmod/config/use.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/download.py` & `portmod-2.6.2/portmod/download.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/execute.py` & `portmod-2.6.2/portmod/execute.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/functools.py` & `portmod-2.6.2/portmod/functools.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/globals.py` & `portmod-2.6.2/portmod/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 import tempfile
 from functools import lru_cache
 from typing import Any, List, Optional
 
 import portmod
+from portmodlib.globals import download_dir
 from portmodlib.l10n import l10n
 from portmodlib.portmod import directories
 
 
 @lru_cache()
 def get_version() -> str:
     """Returns portmod version"""
@@ -81,15 +82,18 @@
             self.SET_DIR: str = os.path.join(self.CONFIG_DIR, "sets")
             self.CONFIG: str = os.path.join(self.CONFIG_DIR, "portmod.conf")
 
             self.ROOT: str = os.path.realpath(
                 prefix.path or os.path.join(env.DATA_DIR, prefix_name)
             )
             self.CACHE_DIR = os.path.join(env.CACHE_DIR, "prefix", prefix_name)
-            self.PYBUILD_INSTALLED_CACHE = os.path.join(self.CACHE_DIR, "pybuild")
+            self.PYBUILD_INSTALLED_CACHE = os.path.join(
+                self.CACHE_DIR, "installed-pybuilds"
+            )
+            self.PYBUILD_CACHE = os.path.join(self.CACHE_DIR, "pybuild")
             self.CONFIG_PROTECT_DIR = os.path.join(self.CACHE_DIR, "cfg_protect")
             self.LOCAL_MODS = os.path.join(self.ROOT, "local")
             self.REPOS = []
 
         def __setattr__(self, name: str, value: Any):
             if isinstance(value, str):
                 os.environ["PORTMOD_" + name] = value
@@ -117,15 +121,15 @@
             self.PREFIX_NAME = None
         return OLD_PREFIX_NAME
 
     def __init__(self):
         self.PREFIX_FILE = os.path.join(self.DATA_DIR, "prefix")
         self.REPOS_DIR = os.path.join(self.DATA_DIR, "repos")
         self.PYBUILD_CACHE_DIR = os.path.join(self.CACHE_DIR, "pybuild")
-        self.DOWNLOAD_DIR = os.path.join(self.CACHE_DIR, "downloads")
+        self.DOWNLOAD_DIR = download_dir()
         self.GLOBAL_PORTMOD_CONFIG = os.path.join(self.CONFIG_DIR, "portmod.conf")
         self.REPOS_FILE = os.path.join(self.CONFIG_DIR, "repos.cfg")
         self.REPOS = []
 
         tempfile.tempdir = None
         self.TMP_DIR = os.path.join(tempfile.gettempdir(), "portmod")
         self.PYBUILD_TMP_DIR = os.path.join(self.TMP_DIR, "pybuild")
```

### Comparing `portmod-2.6.1/portmod/io.py` & `portmod-2.6.2/portmod/io.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/loader.py` & `portmod-2.6.2/portmod/loader.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/lock.py` & `portmod-2.6.2/portmod/lock.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/merge.py` & `portmod-2.6.2/portmod/merge.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/modules.py` & `portmod-2.6.2/portmod/modules.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/news.py` & `portmod-2.6.2/portmod/news.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/package.py` & `portmod-2.6.2/portmod/package.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/parsers/flags.py` & `portmod-2.6.2/portmod/parsers/flags.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/parsers/manifest.py` & `portmod-2.6.2/portmod/parsers/manifest.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/parsers/userconf.py` & `portmod-2.6.2/portmod/parsers/userconf.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/perms.py` & `portmod-2.6.2/portmod/perms.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/prefix.py` & `portmod-2.6.2/portmod/prefix.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/prompt.py` & `portmod-2.6.2/portmod/prompt.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/pybuild.py` & `portmod-2.6.2/portmod/pybuild.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/query.py` & `portmod-2.6.2/portmod/query.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/repo/__init__.py` & `portmod-2.6.2/portmod/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/repo/keywords.py` & `portmod-2.6.2/portmod/repo/keywords.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/repo/loader.py` & `portmod-2.6.2/portmod/repo/loader.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/repo/metadata.py` & `portmod-2.6.2/portmod/repo/metadata.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/repo/updates.py` & `portmod-2.6.2/portmod/repo/updates.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/repos.py` & `portmod-2.6.2/portmod/repos.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/source.py` & `portmod-2.6.2/portmod/source.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/sync.py` & `portmod-2.6.2/portmod/sync.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/transactions.py` & `portmod-2.6.2/portmod/transactions.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/tsort.py` & `portmod-2.6.2/portmod/tsort.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/util.py` & `portmod-2.6.2/portmod/util.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/vdb.py` & `portmod-2.6.2/portmod/vdb.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod/win32.py` & `portmod-2.6.2/portmod/win32.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmod.egg-info/PKG-INFO` & `portmod-2.6.2/portmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portmod
-Version: 2.6.1
+Version: 2.6.2
 Summary: A CLI package manager for mods
 Home-page: https://gitlab.com/portmod/portmod
 Download-URL: https://gitlab.com/portmod/portmod/-/releases
 Author: Portmod Authors
 Author-email: incoming+portmod-portmod-9660349-issue-@incoming.gitlab.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `portmod-2.6.1/portmod.egg-info/SOURCES.txt` & `portmod-2.6.2/portmod.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 doc/dev/naming.rst
 doc/dev/packages.rst
 doc/dev/setup.rst
 doc/dev/use-flags.rst
 doc/dev/repo/index.rst
 doc/dev/repo/layout.conf.rst
 doc/dev/repo/metadata.yaml.rst
+doc/dev/repo/package-files.rst
 doc/dev/repo/profiles.rst
 doc/install/index.rst
 doc/install/linux.rst
 doc/install/macos.rst
 doc/install/windows.rst
 l10n/l10n.toml
 l10n/en-GB/gui.ftl
```

### Comparing `portmod-2.6.1/portmod.egg-info/requires.txt` & `portmod-2.6.2/portmod.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/_deprecated/__init__.py` & `portmod-2.6.2/portmodlib/_deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/_deprecated/vfs.py` & `portmod-2.6.2/portmodlib/_deprecated/vfs.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/_loader.py` & `portmod-2.6.2/portmodlib/_loader.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/_phase.py` & `portmod-2.6.2/portmodlib/_phase.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/_wrapper.py` & `portmod-2.6.2/portmodlib/_wrapper.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/archives.py` & `portmod-2.6.2/portmodlib/archives.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/atom.py` & `portmod-2.6.2/portmodlib/atom.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/colour.py` & `portmod-2.6.2/portmodlib/colour.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/execute.py` & `portmod-2.6.2/portmodlib/execute.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/fs.py` & `portmod-2.6.2/portmodlib/fs.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/functools.py` & `portmod-2.6.2/portmodlib/functools.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/l10n.py` & `portmod-2.6.2/portmodlib/l10n.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/log.py` & `portmod-2.6.2/portmodlib/log.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/masters.py` & `portmod-2.6.2/portmodlib/masters.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/module_util.py` & `portmod-2.6.2/portmodlib/module_util.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/parsers/list.py` & `portmod-2.6.2/portmodlib/parsers/list.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/portmod.pyi` & `portmod-2.6.2/portmodlib/portmod.pyi`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/pybuild.py` & `portmod-2.6.2/portmodlib/pybuild.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/source.py` & `portmod-2.6.2/portmodlib/source.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/usestr.py` & `portmod-2.6.2/portmodlib/usestr.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/util.py` & `portmod-2.6.2/portmodlib/util.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/version.py` & `portmod-2.6.2/portmodlib/version.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/portmodlib/winreg.py` & `portmod-2.6.2/portmodlib/winreg.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/pybuild/__init__.py` & `portmod-2.6.2/pybuild/__init__.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/pybuild/_pybuild.py` & `portmod-2.6.2/pybuild/_pybuild.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/pybuild/info.py` & `portmod-2.6.2/pybuild/info.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/pybuild/winreg.py` & `portmod-2.6.2/pybuild/winreg.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/requirements.txt` & `portmod-2.6.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/setup.cfg` & `portmod-2.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/setup.py` & `portmod-2.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/src/dds.rs` & `portmod-2.6.2/src/dds.rs`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/src/error.rs` & `portmod-2.6.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/src/index.rs` & `portmod-2.6.2/src/index.rs`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/src/lib.rs` & `portmod-2.6.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/src/metadata/mod.rs` & `portmod-2.6.2/src/metadata/mod.rs`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/src/metadata/person.rs` & `portmod-2.6.2/src/metadata/person.rs`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/src/news.rs` & `portmod-2.6.2/src/news.rs`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/src/yaml.rs` & `portmod-2.6.2/src/yaml.rs`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/_benchmarks/atom.py` & `portmod-2.6.2/test/_benchmarks/atom.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/_benchmarks/hash.py` & `portmod-2.6.2/test/_benchmarks/hash.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/_benchmarks/loader.py` & `portmod-2.6.2/test/_benchmarks/loader.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/env.py` & `portmod-2.6.2/test/env.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_alias.py` & `portmod-2.6.2/test/test_alias.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_atom.py` & `portmod-2.6.2/test/test_atom.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_cfg_protect.py` & `portmod-2.6.2/test/test_cfg_protect.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_clean.py` & `portmod-2.6.2/test/test_clean.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_deps.py` & `portmod-2.6.2/test/test_deps.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_download.py` & `portmod-2.6.2/test/test_download.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_execute.py` & `portmod-2.6.2/test/test_execute.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_existing.py` & `portmod-2.6.2/test/test_existing.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_filters.py` & `portmod-2.6.2/test/test_filters.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_fs.py` & `portmod-2.6.2/test/test_fs.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_gui_config.py` & `portmod-2.6.2/test/test_gui_config.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_gui_installed_packages_model.py` & `portmod-2.6.2/test/test_gui_installed_packages_model.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_gui_packages.py` & `portmod-2.6.2/test/test_gui_packages.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_init.py` & `portmod-2.6.2/test/test_init.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_inquisitor.py` & `portmod-2.6.2/test/test_inquisitor.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_keywords.py` & `portmod-2.6.2/test/test_keywords.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_loader.py` & `portmod-2.6.2/test/test_loader.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_log.py` & `portmod-2.6.2/test/test_log.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_manifest.py` & `portmod-2.6.2/test/test_manifest.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_mask.py` & `portmod-2.6.2/test/test_mask.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_masters.py` & `portmod-2.6.2/test/test_masters.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_merge.py` & `portmod-2.6.2/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_metadata.py` & `portmod-2.6.2/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_modules.py` & `portmod-2.6.2/test/test_modules.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_news.py` & `portmod-2.6.2/test/test_news.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_obscure.py` & `portmod-2.6.2/test/test_obscure.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_portmod_config.py` & `portmod-2.6.2/test/test_portmod_config.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_prefix_cli.py` & `portmod-2.6.2/test/test_prefix_cli.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_profile.py` & `portmod-2.6.2/test/test_profile.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_query.py` & `portmod-2.6.2/test/test_query.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_resolve.py` & `portmod-2.6.2/test/test_resolve.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_select.py` & `portmod-2.6.2/test/test_select.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_unpack.py` & `portmod-2.6.2/test/test_unpack.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_updates.py` & `portmod-2.6.2/test/test_updates.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_use.py` & `portmod-2.6.2/test/test_use.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_vdb.py` & `portmod-2.6.2/test/test_vdb.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_version.py` & `portmod-2.6.2/test/test_version.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/test_vfs.py` & `portmod-2.6.2/test/test_vfs.py`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/profiles/base/defaults.conf` & `portmod-2.6.2/test/testrepo/profiles/base/defaults.conf`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/test/quill-of-feyfolken/quill-of-feyfolken-2.0.2-r1.pybuild` & `portmod-2.6.2/test/testrepo/test/quill-of-feyfolken/quill-of-feyfolken-2.0.2-r1.pybuild`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/test/quill-of-feyfolken/quill-of-feyfolken-2.0.2.pybuild` & `portmod-2.6.2/test/testrepo/test/quill-of-feyfolken/quill-of-feyfolken-2.0.2.pybuild`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/test/test/test-1.0-r1.pybuild` & `portmod-2.6.2/test/testrepo/test/test/test-1.0-r1.pybuild`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/test/test/test-1.0-r2.pybuild` & `portmod-2.6.2/test/testrepo/test/test/test-1.0-r2.pybuild`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/test/test/test-1.0.pybuild` & `portmod-2.6.2/test/testrepo/test/test/test-1.0.pybuild`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/test/test/test-2.0.pybuild` & `portmod-2.6.2/test/testrepo/test/test/test-2.0.pybuild`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/test/test-module/test-module-1.0.pybuild` & `portmod-2.6.2/test/testrepo/test/test-module/test-module-1.0.pybuild`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/test/test2/test2-1.0.pybuild` & `portmod-2.6.2/test/testrepo/test/test2/test2-1.0.pybuild`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/test/testrepo/test/test7/test7-1.0.pybuild` & `portmod-2.6.2/test/testrepo/test/test7/test7-1.0.pybuild`

 * *Files identical despite different names*

### Comparing `portmod-2.6.1/tools/update_header.py` & `portmod-2.6.2/tools/update_header.py`

 * *Files identical despite different names*

