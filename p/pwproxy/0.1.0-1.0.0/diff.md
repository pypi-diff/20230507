# Comparing `tmp/pwproxy-0.1.0.tar.gz` & `tmp/pwproxy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwproxy-0.1.0.tar", last modified: Sun Apr 23 04:28:29 2023, max compression
+gzip compressed data, was "pwproxy-1.0.0.tar", last modified: Sun May  7 03:22:58 2023, max compression
```

## Comparing `pwproxy-0.1.0.tar` & `pwproxy-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 04:28:29.842771 pwproxy-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-04-23 04:11:21.000000 pwproxy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1254 2023-04-23 04:28:29.841767 pwproxy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-04-23 04:20:17.000000 pwproxy-0.1.0/README.md
--rw-rw-rw-   0        0        0      728 2023-04-23 04:28:14.000000 pwproxy-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 04:28:29.842771 pwproxy-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-23 04:28:29.830768 pwproxy-0.1.0/src/
--rw-rw-rw-   0        0        0        0 2023-04-23 04:11:21.000000 pwproxy-0.1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:28:29.833771 pwproxy-0.1.0/src/pwproxy/
--rw-rw-rw-   0        0        0      567 2023-04-23 04:11:21.000000 pwproxy-0.1.0/src/pwproxy/__init__.py
--rw-rw-rw-   0        0        0     1028 2023-04-23 04:11:21.000000 pwproxy-0.1.0/src/pwproxy/function.py
--rw-rw-rw-   0        0        0     2184 2023-04-23 04:11:21.000000 pwproxy-0.1.0/src/pwproxy/run.py
-drwxrwxrwx   0        0        0        0 2023-04-23 04:28:29.837767 pwproxy-0.1.0/src/pwproxy.egg-info/
--rw-rw-rw-   0        0        0     1254 2023-04-23 04:28:29.000000 pwproxy-0.1.0/src/pwproxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-04-23 04:28:29.000000 pwproxy-0.1.0/src/pwproxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 04:28:29.000000 pwproxy-0.1.0/src/pwproxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-23 04:28:29.000000 pwproxy-0.1.0/src/pwproxy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 04:28:29.000000 pwproxy-0.1.0/src/pwproxy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 04:28:29.840771 pwproxy-0.1.0/test/
--rw-rw-rw-   0        0        0      366 2023-04-23 04:11:21.000000 pwproxy-0.1.0/test/test_1.py
--rw-rw-rw-   0        0        0      637 2023-04-23 04:11:21.000000 pwproxy-0.1.0/test/test_2.py
--rw-rw-rw-   0        0        0      342 2023-04-23 04:11:21.000000 pwproxy-0.1.0/test/test_3.py
--rw-rw-rw-   0        0        0      351 2023-04-23 04:11:21.000000 pwproxy-0.1.0/test/test_4.py
--rw-rw-rw-   0        0        0      466 2023-04-23 04:11:21.000000 pwproxy-0.1.0/test/test_5.py
+drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.959820 pwproxy-1.0.0/
+-rw-r--r--   0 gaochuang   (501) staff       (20)    11357 2023-05-07 03:21:17.000000 pwproxy-1.0.0/LICENSE
+-rw-r--r--   0 gaochuang   (501) staff       (20)     1134 2023-05-07 03:22:58.959682 pwproxy-1.0.0/PKG-INFO
+-rw-r--r--   0 gaochuang   (501) staff       (20)      895 2023-05-07 03:21:17.000000 pwproxy-1.0.0/README.md
+-rw-r--r--   0 gaochuang   (501) staff       (20)      545 2023-05-07 03:21:17.000000 pwproxy-1.0.0/pyproject.toml
+-rw-r--r--   0 gaochuang   (501) staff       (20)       38 2023-05-07 03:22:58.959859 pwproxy-1.0.0/setup.cfg
+drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.957527 pwproxy-1.0.0/src/
+-rw-r--r--   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:21:17.000000 pwproxy-1.0.0/src/__init__.py
+drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.958098 pwproxy-1.0.0/src/pwproxy/
+-rw-r--r--   0 gaochuang   (501) staff       (20)      544 2023-05-07 03:21:17.000000 pwproxy-1.0.0/src/pwproxy/__init__.py
+-rw-r--r--   0 gaochuang   (501) staff       (20)      990 2023-05-07 03:21:17.000000 pwproxy-1.0.0/src/pwproxy/function.py
+-rw-r--r--   0 gaochuang   (501) staff       (20)     2106 2023-05-07 03:21:17.000000 pwproxy-1.0.0/src/pwproxy/run.py
+drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.958792 pwproxy-1.0.0/src/pwproxy.egg-info/
+-rw-r--r--   0 gaochuang   (501) staff       (20)     1134 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/PKG-INFO
+-rw-r--r--   0 gaochuang   (501) staff       (20)      364 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 gaochuang   (501) staff       (20)        1 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 gaochuang   (501) staff       (20)       24 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/requires.txt
+-rw-r--r--   0 gaochuang   (501) staff       (20)        8 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/top_level.txt
+drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.959458 pwproxy-1.0.0/test/
+-rw-r--r--   0 gaochuang   (501) staff       (20)      352 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_1.py
+-rw-r--r--   0 gaochuang   (501) staff       (20)      617 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_2.py
+-rw-r--r--   0 gaochuang   (501) staff       (20)      326 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_3.py
+-rw-r--r--   0 gaochuang   (501) staff       (20)      336 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_4.py
+-rw-r--r--   0 gaochuang   (501) staff       (20)      447 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_5.py
```

### Comparing `pwproxy-0.1.0/LICENSE` & `pwproxy-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `pwproxy-0.1.0/PKG-INFO` & `pwproxy-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-Metadata-Version: 2.1
-Name: pwproxy
-Version: 0.1.0
-Author-email: gc <895091550@qq.com>
-Project-URL: Homepage, https://github.com/gcil125/pwproxy
-Keywords: playwright,mitmproxy,intercept request,modify response
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pwproxy
-
-<hr>
-
-> 基于playwright实现mitmproxy的核心功能:请求拦截,响应篡改<br>
-
-优点
-
-1. 基于playwright，直接调用本地浏览器，不用以设置代理的方式启动浏览器, mitmproxy必须以冷启动设置代理的方法启动本地浏览器才能实现拦截
-2. 不需要考虑安全证书的问题
-
-# 安装
-
-`pip install pwproxy`
-
-# 使用
-
-<hr>
-目录结构:<br>
-
-```python
-├─run.py
-├─demo.py
-```
-
-```python
-# run.py
-from pwproxy.run import Run
-
-Run.run("demo.py", url="http://example.com/")
-```
-
-```python
-# demo.py
-from playwright.sync_api import Route
-
-
-def replace_resp(route: Route):
-    if "http://example.com/" in route.request.url:
-        response = route.fetch()
-        body = response.text()
-        body = body.replace("Example Domain", "Goodo")
-        route.fulfill(
-            body=body
-        )
-
-addons = [
-    replace_resp
-]
-```
-
-
+Metadata-Version: 2.1
+Name: pwproxy
+Version: 1.0.0
+Author-email: gc <895091550@qq.com>
+Keywords: playwright,mitmproxy,intercept request,modify response
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pwproxy
+
+<hr>
+
+> 基于playwright实现mitmproxy的核心功能:请求拦截,响应篡改<br>
+
+优点
+
+1. 基于playwright，直接调用本地浏览器，不用以设置代理的方式启动浏览器, mitmproxy必须以冷启动设置代理的方法启动本地浏览器才能实现拦截
+2. 不需要考虑安全证书的问题
+
+# 安装
+
+`pip install pwproxy`
+
+# 使用
+
+<hr>
+目录结构:<br>
+
+```python
+├─run.py
+├─demo.py
+```
+
+```python
+# run.py
+from pwproxy.run import Run
+
+Run.run("demo.py", url="http://example.com/")
+```
+
+```python
+# demo.py
+from playwright.sync_api import Route
+
+
+def replace_resp(route: Route):
+    if "http://example.com/" in route.request.url:
+        response = route.fetch()
+        body = response.text()
+        body = body.replace("Example Domain", "Goodo")
+        route.fulfill(
+            body=body
+        )
+
+addons = [
+    replace_resp
+]
+```
+
+
```

### Comparing `pwproxy-0.1.0/pyproject.toml` & `pwproxy-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,26 @@
-[build-system]
-requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "pwproxy"
-version = "0.1.0"
-authors = [
-    { name = "gc", email = "895091550@qq.com" },
-]
-requires-python = ">=3.10"
-readme = "README.md"
-dependencies = [
-    "playwright",
-    "pandas"
-]
-keywords = ["playwright", "mitmproxy", "intercept request", "modify response"]
-
-[options]
-python_requires = ">=3.10"
-dependency_links = ["https://pypi.tuna.tsinghua.edu.cn/simple/"]
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[distutils]
-index-servers = "pypi"
-
-[pypi]
-username = "gcil125"
-password = "qweASD123..."
-
-
-[project.urls]
-"Homepage" = "https://github.com/gcil125/pwproxy"
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pwproxy"
+version = "1.0.0"
+authors = [
+    { name = "gc", email = "895091550@qq.com" },
+]
+requires-python = ">=3.10"
+readme = "README.md"
+dependencies = [
+    "playwright",
+    "nest_asyncio"
+
+]
+keywords = ["playwright", "mitmproxy", "intercept request", "modify response"]
+
+[options]
+python_requires = ">=3.10"
+dependency_links = ["https://pypi.tuna.tsinghua.edu.cn/simple/"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
```

### Comparing `pwproxy-0.1.0/src/pwproxy/function.py` & `pwproxy-1.0.0/src/pwproxy/function.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import List, Dict
-import pandas as pd
-from random import choice
-
-__all__ = [
-    "delete_col",
-    "replace_data"
-]
-
-
-def dframe_to_dict(func):
-    def inner(*args, **kwargs):
-        dataf = func(*args, **kwargs)
-        if dataf is not None:
-            return dataf.to_dict("records")
-
-    return inner
-
-
-@dframe_to_dict
-def delete_col(self, *, data: List[Dict], cols: list = None):
-    frame = pd.DataFrame(data)
-    return frame.drop(cols, axis=1)
-
-
-@dframe_to_dict
-def replace_data(self, *, data: List[Dict], _new: dict[str, list | tuple] = None, rate: float = 0.5):
-    frame = pd.DataFrame(data)
-    f_columns = set(frame.columns)
-    _new_columns = set(_new.keys())
-    _mod = _new_columns - f_columns
-    if _mod == set():
-        for field, values in _new.items():
-            ser = frame[field].copy(deep=False)
-            for i in range(int(len(ser) * rate)):
-                ser[i] = choice(values)
-        return frame
-    raise KeyError(f"{_mod!s} not exist!")
+from typing import List, Dict
+import pandas as pd
+from random import choice
+
+__all__ = [
+    "delete_col",
+    "replace_data"
+]
+
+
+def dframe_to_dict(func):
+    def inner(*args, **kwargs):
+        dataf = func(*args, **kwargs)
+        if dataf is not None:
+            return dataf.to_dict("records")
+
+    return inner
+
+
+@dframe_to_dict
+def delete_col(self, *, data: List[Dict], cols: list = None):
+    frame = pd.DataFrame(data)
+    return frame.drop(cols, axis=1)
+
+
+@dframe_to_dict
+def replace_data(self, *, data: List[Dict], _new: dict[str, list | tuple] = None, rate: float = 0.5):
+    frame = pd.DataFrame(data)
+    f_columns = set(frame.columns)
+    _new_columns = set(_new.keys())
+    _mod = _new_columns - f_columns
+    if _mod == set():
+        for field, values in _new.items():
+            ser = frame[field].copy(deep=False)
+            for i in range(int(len(ser) * rate)):
+                ser[i] = choice(values)
+        return frame
+    raise KeyError(f"{_mod!s} not exist!")
```

### Comparing `pwproxy-0.1.0/src/pwproxy.egg-info/PKG-INFO` & `pwproxy-1.0.0/src/pwproxy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-Metadata-Version: 2.1
-Name: pwproxy
-Version: 0.1.0
-Author-email: gc <895091550@qq.com>
-Project-URL: Homepage, https://github.com/gcil125/pwproxy
-Keywords: playwright,mitmproxy,intercept request,modify response
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pwproxy
-
-<hr>
-
-> 基于playwright实现mitmproxy的核心功能:请求拦截,响应篡改<br>
-
-优点
-
-1. 基于playwright，直接调用本地浏览器，不用以设置代理的方式启动浏览器, mitmproxy必须以冷启动设置代理的方法启动本地浏览器才能实现拦截
-2. 不需要考虑安全证书的问题
-
-# 安装
-
-`pip install pwproxy`
-
-# 使用
-
-<hr>
-目录结构:<br>
-
-```python
-├─run.py
-├─demo.py
-```
-
-```python
-# run.py
-from pwproxy.run import Run
-
-Run.run("demo.py", url="http://example.com/")
-```
-
-```python
-# demo.py
-from playwright.sync_api import Route
-
-
-def replace_resp(route: Route):
-    if "http://example.com/" in route.request.url:
-        response = route.fetch()
-        body = response.text()
-        body = body.replace("Example Domain", "Goodo")
-        route.fulfill(
-            body=body
-        )
-
-addons = [
-    replace_resp
-]
-```
-
-
+Metadata-Version: 2.1
+Name: pwproxy
+Version: 1.0.0
+Author-email: gc <895091550@qq.com>
+Keywords: playwright,mitmproxy,intercept request,modify response
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pwproxy
+
+<hr>
+
+> 基于playwright实现mitmproxy的核心功能:请求拦截,响应篡改<br>
+
+优点
+
+1. 基于playwright，直接调用本地浏览器，不用以设置代理的方式启动浏览器, mitmproxy必须以冷启动设置代理的方法启动本地浏览器才能实现拦截
+2. 不需要考虑安全证书的问题
+
+# 安装
+
+`pip install pwproxy`
+
+# 使用
+
+<hr>
+目录结构:<br>
+
+```python
+├─run.py
+├─demo.py
+```
+
+```python
+# run.py
+from pwproxy.run import Run
+
+Run.run("demo.py", url="http://example.com/")
+```
+
+```python
+# demo.py
+from playwright.sync_api import Route
+
+
+def replace_resp(route: Route):
+    if "http://example.com/" in route.request.url:
+        response = route.fetch()
+        body = response.text()
+        body = body.replace("Example Domain", "Goodo")
+        route.fulfill(
+            body=body
+        )
+
+addons = [
+    replace_resp
+]
+```
+
+
```

