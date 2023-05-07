# Comparing `tmp/nazo_rand-0.0.7.tar.gz` & `tmp/nazo_rand-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazo_rand-0.0.7.tar", last modified: Thu Apr 20 14:27:20 2023, max compression
+gzip compressed data, was "nazo_rand-0.0.8.tar", last modified: Sun May  7 10:03:22 2023, max compression
```

## Comparing `nazo_rand-0.0.7.tar` & `nazo_rand-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:20.004364 nazo_rand-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-20 14:27:20.004364 nazo_rand-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:20.000364 nazo_rand-0.0.7/nazo_rand/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   249266 2023-04-20 14:27:09.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:20.004364 nazo_rand-0.0.7/nazo_rand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-20 14:27:19.000000 nazo_rand-0.0.7/nazo_rand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-20 14:27:19.000000 nazo_rand-0.0.7/nazo_rand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:27:19.000000 nazo_rand-0.0.7/nazo_rand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 14:27:19.000000 nazo_rand-0.0.7/nazo_rand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:27:20.004364 nazo_rand-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/
+-rw-rw-rw-   0        0        0    18431 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      130 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1971 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1164 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/nazo_rand/
+-rw-rw-rw-   0        0        0       26 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/__init__.py
+-rw-rw-rw-   0        0        0   274726 2023-05-07 10:03:21.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.cpp
+-rw-rw-rw-   0        0        0     1954 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.hpp
+-rw-rw-rw-   0        0        0      700 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.pxd
+-rw-rw-rw-   0        0        0     2624 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.pyi
+-rw-rw-rw-   0        0        0     2572 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/nazo_rand/nazo_rand.pyx
+drwxrwxrwx   0        0        0        0 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/nazo_rand.egg-info/
+-rw-rw-rw-   0        0        0     1971 2023-05-07 10:03:22.000000 nazo_rand-0.0.8/nazo_rand.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-05-07 10:03:22.000000 nazo_rand-0.0.8/nazo_rand.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 10:03:22.000000 nazo_rand-0.0.8/nazo_rand.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-07 10:03:22.000000 nazo_rand-0.0.8/nazo_rand.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      484 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 10:03:22.118795 nazo_rand-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2172 2023-05-07 10:02:43.000000 nazo_rand-0.0.8/setup.py
```

### Comparing `nazo_rand-0.0.7/LICENSE` & `nazo_rand-0.0.8/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 2, June 1991
-
- Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
- 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The licenses for most software are designed to take away your
-freedom to share and change it.  By contrast, the GNU General Public
-License is intended to guarantee your freedom to share and change free
-software--to make sure the software is free for all its users.  This
-General Public License applies to most of the Free Software
-Foundation's software and to any other program whose authors commit to
-using it.  (Some other Free Software Foundation software is covered by
-the GNU Lesser General Public License instead.)  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-this service if you wish), that you receive source code or can get it
-if you want it, that you can change the software or use pieces of it
-in new free programs; and that you know you can do these things.
-
-  To protect your rights, we need to make restrictions that forbid
-anyone to deny you these rights or to ask you to surrender the rights.
-These restrictions translate to certain responsibilities for you if you
-distribute copies of the software, or if you modify it.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must give the recipients all the rights that
-you have.  You must make sure that they, too, receive or can get the
-source code.  And you must show them these terms so they know their
-rights.
-
-  We protect your rights with two steps: (1) copyright the software, and
-(2) offer you this license which gives you legal permission to copy,
-distribute and/or modify the software.
-
-  Also, for each author's protection and ours, we want to make certain
-that everyone understands that there is no warranty for this free
-software.  If the software is modified by someone else and passed on, we
-want its recipients to know that what they have is not the original, so
-that any problems introduced by others will not reflect on the original
-authors' reputations.
-
-  Finally, any free program is threatened constantly by software
-patents.  We wish to avoid the danger that redistributors of a free
-program will individually obtain patent licenses, in effect making the
-program proprietary.  To prevent this, we have made it clear that any
-patent must be licensed for everyone's free use or not licensed at all.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                    GNU GENERAL PUBLIC LICENSE
-   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-  0. This License applies to any program or other work which contains
-a notice placed by the copyright holder saying it may be distributed
-under the terms of this General Public License.  The "Program", below,
-refers to any such program or work, and a "work based on the Program"
-means either the Program or any derivative work under copyright law:
-that is to say, a work containing the Program or a portion of it,
-either verbatim or with modifications and/or translated into another
-language.  (Hereinafter, translation is included without limitation in
-the term "modification".)  Each licensee is addressed as "you".
-
-Activities other than copying, distribution and modification are not
-covered by this License; they are outside its scope.  The act of
-running the Program is not restricted, and the output from the Program
-is covered only if its contents constitute a work based on the
-Program (independent of having been made by running the Program).
-Whether that is true depends on what the Program does.
-
-  1. You may copy and distribute verbatim copies of the Program's
-source code as you receive it, in any medium, provided that you
-conspicuously and appropriately publish on each copy an appropriate
-copyright notice and disclaimer of warranty; keep intact all the
-notices that refer to this License and to the absence of any warranty;
-and give any other recipients of the Program a copy of this License
-along with the Program.
-
-You may charge a fee for the physical act of transferring a copy, and
-you may at your option offer warranty protection in exchange for a fee.
-
-  2. You may modify your copy or copies of the Program or any portion
-of it, thus forming a work based on the Program, and copy and
-distribute such modifications or work under the terms of Section 1
-above, provided that you also meet all of these conditions:
-
-    a) You must cause the modified files to carry prominent notices
-    stating that you changed the files and the date of any change.
-
-    b) You must cause any work that you distribute or publish, that in
-    whole or in part contains or is derived from the Program or any
-    part thereof, to be licensed as a whole at no charge to all third
-    parties under the terms of this License.
-
-    c) If the modified program normally reads commands interactively
-    when run, you must cause it, when started running for such
-    interactive use in the most ordinary way, to print or display an
-    announcement including an appropriate copyright notice and a
-    notice that there is no warranty (or else, saying that you provide
-    a warranty) and that users may redistribute the program under
-    these conditions, and telling the user how to view a copy of this
-    License.  (Exception: if the Program itself is interactive but
-    does not normally print such an announcement, your work based on
-    the Program is not required to print an announcement.)
-
-These requirements apply to the modified work as a whole.  If
-identifiable sections of that work are not derived from the Program,
-and can be reasonably considered independent and separate works in
-themselves, then this License, and its terms, do not apply to those
-sections when you distribute them as separate works.  But when you
-distribute the same sections as part of a whole which is a work based
-on the Program, the distribution of the whole must be on the terms of
-this License, whose permissions for other licensees extend to the
-entire whole, and thus to each and every part regardless of who wrote it.
-
-Thus, it is not the intent of this section to claim rights or contest
-your rights to work written entirely by you; rather, the intent is to
-exercise the right to control the distribution of derivative or
-collective works based on the Program.
-
-In addition, mere aggregation of another work not based on the Program
-with the Program (or with a work based on the Program) on a volume of
-a storage or distribution medium does not bring the other work under
-the scope of this License.
-
-  3. You may copy and distribute the Program (or a work based on it,
-under Section 2) in object code or executable form under the terms of
-Sections 1 and 2 above provided that you also do one of the following:
-
-    a) Accompany it with the complete corresponding machine-readable
-    source code, which must be distributed under the terms of Sections
-    1 and 2 above on a medium customarily used for software interchange; or,
-
-    b) Accompany it with a written offer, valid for at least three
-    years, to give any third party, for a charge no more than your
-    cost of physically performing source distribution, a complete
-    machine-readable copy of the corresponding source code, to be
-    distributed under the terms of Sections 1 and 2 above on a medium
-    customarily used for software interchange; or,
-
-    c) Accompany it with the information you received as to the offer
-    to distribute corresponding source code.  (This alternative is
-    allowed only for noncommercial distribution and only if you
-    received the program in object code or executable form with such
-    an offer, in accord with Subsection b above.)
-
-The source code for a work means the preferred form of the work for
-making modifications to it.  For an executable work, complete source
-code means all the source code for all modules it contains, plus any
-associated interface definition files, plus the scripts used to
-control compilation and installation of the executable.  However, as a
-special exception, the source code distributed need not include
-anything that is normally distributed (in either source or binary
-form) with the major components (compiler, kernel, and so on) of the
-operating system on which the executable runs, unless that component
-itself accompanies the executable.
-
-If distribution of executable or object code is made by offering
-access to copy from a designated place, then offering equivalent
-access to copy the source code from the same place counts as
-distribution of the source code, even though third parties are not
-compelled to copy the source along with the object code.
-
-  4. You may not copy, modify, sublicense, or distribute the Program
-except as expressly provided under this License.  Any attempt
-otherwise to copy, modify, sublicense or distribute the Program is
-void, and will automatically terminate your rights under this License.
-However, parties who have received copies, or rights, from you under
-this License will not have their licenses terminated so long as such
-parties remain in full compliance.
-
-  5. You are not required to accept this License, since you have not
-signed it.  However, nothing else grants you permission to modify or
-distribute the Program or its derivative works.  These actions are
-prohibited by law if you do not accept this License.  Therefore, by
-modifying or distributing the Program (or any work based on the
-Program), you indicate your acceptance of this License to do so, and
-all its terms and conditions for copying, distributing or modifying
-the Program or works based on it.
-
-  6. Each time you redistribute the Program (or any work based on the
-Program), the recipient automatically receives a license from the
-original licensor to copy, distribute or modify the Program subject to
-these terms and conditions.  You may not impose any further
-restrictions on the recipients' exercise of the rights granted herein.
-You are not responsible for enforcing compliance by third parties to
-this License.
-
-  7. If, as a consequence of a court judgment or allegation of patent
-infringement or for any other reason (not limited to patent issues),
-conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot
-distribute so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you
-may not distribute the Program at all.  For example, if a patent
-license would not permit royalty-free redistribution of the Program by
-all those who receive copies directly or indirectly through you, then
-the only way you could satisfy both it and this License would be to
-refrain entirely from distribution of the Program.
-
-If any portion of this section is held invalid or unenforceable under
-any particular circumstance, the balance of the section is intended to
-apply and the section as a whole is intended to apply in other
-circumstances.
-
-It is not the purpose of this section to induce you to infringe any
-patents or other property right claims or to contest validity of any
-such claims; this section has the sole purpose of protecting the
-integrity of the free software distribution system, which is
-implemented by public license practices.  Many people have made
-generous contributions to the wide range of software distributed
-through that system in reliance on consistent application of that
-system; it is up to the author/donor to decide if he or she is willing
-to distribute software through any other system and a licensee cannot
-impose that choice.
-
-This section is intended to make thoroughly clear what is believed to
-be a consequence of the rest of this License.
-
-  8. If the distribution and/or use of the Program is restricted in
-certain countries either by patents or by copyrighted interfaces, the
-original copyright holder who places the Program under this License
-may add an explicit geographical distribution limitation excluding
-those countries, so that distribution is permitted only in or among
-countries not thus excluded.  In such case, this License incorporates
-the limitation as if written in the body of this License.
-
-  9. The Free Software Foundation may publish revised and/or new versions
-of the General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-Each version is given a distinguishing version number.  If the Program
-specifies a version number of this License which applies to it and "any
-later version", you have the option of following the terms and conditions
-either of that version or of any later version published by the Free
-Software Foundation.  If the Program does not specify a version number of
-this License, you may choose any version ever published by the Free Software
-Foundation.
-
-  10. If you wish to incorporate parts of the Program into other free
-programs whose distribution conditions are different, write to the author
-to ask for permission.  For software which is copyrighted by the Free
-Software Foundation, write to the Free Software Foundation; we sometimes
-make exceptions for this.  Our decision will be guided by the two goals
-of preserving the free status of all derivatives of our free software and
-of promoting the sharing and reuse of software generally.
-
-                            NO WARRANTY
-
-  11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
-FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW.  EXCEPT WHEN
-OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
-PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED
-OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
-MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  THE ENTIRE RISK AS
-TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU.  SHOULD THE
-PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING,
-REPAIR OR CORRECTION.
-
-  12. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR
-REDISTRIBUTE THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
-INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
-OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
-TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
-YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
-PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGES.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-convey the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software; you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation; either version 2 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License along
-    with this program; if not, write to the Free Software Foundation, Inc.,
-    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-
-Also add information on how to contact you by electronic and paper mail.
-
-If the program is interactive, make it output a short notice like this
-when it starts in an interactive mode:
-
-    Gnomovision version 69, Copyright (C) year name of author
-    Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, the commands you use may
-be called something other than `show w' and `show c'; they could even be
-mouse-clicks or menu items--whatever suits your program.
-
-You should also get your employer (if you work as a programmer) or your
-school, if any, to sign a "copyright disclaimer" for the program, if
-necessary.  Here is a sample; alter the names:
-
-  Yoyodyne, Inc., hereby disclaims all copyright interest in the program
-  `Gnomovision' (which makes passes at compilers) written by James Hacker.
-
-  <signature of Ty Coon>, 1 April 1989
-  Ty Coon, President of Vice
-
-This General Public License does not permit incorporating your program into
-proprietary programs.  If your program is a subroutine library, you may
-consider it more useful to permit linking proprietary applications with the
-library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 2, June 1991
+
+ Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
+ 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The licenses for most software are designed to take away your
+freedom to share and change it.  By contrast, the GNU General Public
+License is intended to guarantee your freedom to share and change free
+software--to make sure the software is free for all its users.  This
+General Public License applies to most of the Free Software
+Foundation's software and to any other program whose authors commit to
+using it.  (Some other Free Software Foundation software is covered by
+the GNU Lesser General Public License instead.)  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+this service if you wish), that you receive source code or can get it
+if you want it, that you can change the software or use pieces of it
+in new free programs; and that you know you can do these things.
+
+  To protect your rights, we need to make restrictions that forbid
+anyone to deny you these rights or to ask you to surrender the rights.
+These restrictions translate to certain responsibilities for you if you
+distribute copies of the software, or if you modify it.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must give the recipients all the rights that
+you have.  You must make sure that they, too, receive or can get the
+source code.  And you must show them these terms so they know their
+rights.
+
+  We protect your rights with two steps: (1) copyright the software, and
+(2) offer you this license which gives you legal permission to copy,
+distribute and/or modify the software.
+
+  Also, for each author's protection and ours, we want to make certain
+that everyone understands that there is no warranty for this free
+software.  If the software is modified by someone else and passed on, we
+want its recipients to know that what they have is not the original, so
+that any problems introduced by others will not reflect on the original
+authors' reputations.
+
+  Finally, any free program is threatened constantly by software
+patents.  We wish to avoid the danger that redistributors of a free
+program will individually obtain patent licenses, in effect making the
+program proprietary.  To prevent this, we have made it clear that any
+patent must be licensed for everyone's free use or not licensed at all.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                    GNU GENERAL PUBLIC LICENSE
+   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+  0. This License applies to any program or other work which contains
+a notice placed by the copyright holder saying it may be distributed
+under the terms of this General Public License.  The "Program", below,
+refers to any such program or work, and a "work based on the Program"
+means either the Program or any derivative work under copyright law:
+that is to say, a work containing the Program or a portion of it,
+either verbatim or with modifications and/or translated into another
+language.  (Hereinafter, translation is included without limitation in
+the term "modification".)  Each licensee is addressed as "you".
+
+Activities other than copying, distribution and modification are not
+covered by this License; they are outside its scope.  The act of
+running the Program is not restricted, and the output from the Program
+is covered only if its contents constitute a work based on the
+Program (independent of having been made by running the Program).
+Whether that is true depends on what the Program does.
+
+  1. You may copy and distribute verbatim copies of the Program's
+source code as you receive it, in any medium, provided that you
+conspicuously and appropriately publish on each copy an appropriate
+copyright notice and disclaimer of warranty; keep intact all the
+notices that refer to this License and to the absence of any warranty;
+and give any other recipients of the Program a copy of this License
+along with the Program.
+
+You may charge a fee for the physical act of transferring a copy, and
+you may at your option offer warranty protection in exchange for a fee.
+
+  2. You may modify your copy or copies of the Program or any portion
+of it, thus forming a work based on the Program, and copy and
+distribute such modifications or work under the terms of Section 1
+above, provided that you also meet all of these conditions:
+
+    a) You must cause the modified files to carry prominent notices
+    stating that you changed the files and the date of any change.
+
+    b) You must cause any work that you distribute or publish, that in
+    whole or in part contains or is derived from the Program or any
+    part thereof, to be licensed as a whole at no charge to all third
+    parties under the terms of this License.
+
+    c) If the modified program normally reads commands interactively
+    when run, you must cause it, when started running for such
+    interactive use in the most ordinary way, to print or display an
+    announcement including an appropriate copyright notice and a
+    notice that there is no warranty (or else, saying that you provide
+    a warranty) and that users may redistribute the program under
+    these conditions, and telling the user how to view a copy of this
+    License.  (Exception: if the Program itself is interactive but
+    does not normally print such an announcement, your work based on
+    the Program is not required to print an announcement.)
+
+These requirements apply to the modified work as a whole.  If
+identifiable sections of that work are not derived from the Program,
+and can be reasonably considered independent and separate works in
+themselves, then this License, and its terms, do not apply to those
+sections when you distribute them as separate works.  But when you
+distribute the same sections as part of a whole which is a work based
+on the Program, the distribution of the whole must be on the terms of
+this License, whose permissions for other licensees extend to the
+entire whole, and thus to each and every part regardless of who wrote it.
+
+Thus, it is not the intent of this section to claim rights or contest
+your rights to work written entirely by you; rather, the intent is to
+exercise the right to control the distribution of derivative or
+collective works based on the Program.
+
+In addition, mere aggregation of another work not based on the Program
+with the Program (or with a work based on the Program) on a volume of
+a storage or distribution medium does not bring the other work under
+the scope of this License.
+
+  3. You may copy and distribute the Program (or a work based on it,
+under Section 2) in object code or executable form under the terms of
+Sections 1 and 2 above provided that you also do one of the following:
+
+    a) Accompany it with the complete corresponding machine-readable
+    source code, which must be distributed under the terms of Sections
+    1 and 2 above on a medium customarily used for software interchange; or,
+
+    b) Accompany it with a written offer, valid for at least three
+    years, to give any third party, for a charge no more than your
+    cost of physically performing source distribution, a complete
+    machine-readable copy of the corresponding source code, to be
+    distributed under the terms of Sections 1 and 2 above on a medium
+    customarily used for software interchange; or,
+
+    c) Accompany it with the information you received as to the offer
+    to distribute corresponding source code.  (This alternative is
+    allowed only for noncommercial distribution and only if you
+    received the program in object code or executable form with such
+    an offer, in accord with Subsection b above.)
+
+The source code for a work means the preferred form of the work for
+making modifications to it.  For an executable work, complete source
+code means all the source code for all modules it contains, plus any
+associated interface definition files, plus the scripts used to
+control compilation and installation of the executable.  However, as a
+special exception, the source code distributed need not include
+anything that is normally distributed (in either source or binary
+form) with the major components (compiler, kernel, and so on) of the
+operating system on which the executable runs, unless that component
+itself accompanies the executable.
+
+If distribution of executable or object code is made by offering
+access to copy from a designated place, then offering equivalent
+access to copy the source code from the same place counts as
+distribution of the source code, even though third parties are not
+compelled to copy the source along with the object code.
+
+  4. You may not copy, modify, sublicense, or distribute the Program
+except as expressly provided under this License.  Any attempt
+otherwise to copy, modify, sublicense or distribute the Program is
+void, and will automatically terminate your rights under this License.
+However, parties who have received copies, or rights, from you under
+this License will not have their licenses terminated so long as such
+parties remain in full compliance.
+
+  5. You are not required to accept this License, since you have not
+signed it.  However, nothing else grants you permission to modify or
+distribute the Program or its derivative works.  These actions are
+prohibited by law if you do not accept this License.  Therefore, by
+modifying or distributing the Program (or any work based on the
+Program), you indicate your acceptance of this License to do so, and
+all its terms and conditions for copying, distributing or modifying
+the Program or works based on it.
+
+  6. Each time you redistribute the Program (or any work based on the
+Program), the recipient automatically receives a license from the
+original licensor to copy, distribute or modify the Program subject to
+these terms and conditions.  You may not impose any further
+restrictions on the recipients' exercise of the rights granted herein.
+You are not responsible for enforcing compliance by third parties to
+this License.
+
+  7. If, as a consequence of a court judgment or allegation of patent
+infringement or for any other reason (not limited to patent issues),
+conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot
+distribute so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you
+may not distribute the Program at all.  For example, if a patent
+license would not permit royalty-free redistribution of the Program by
+all those who receive copies directly or indirectly through you, then
+the only way you could satisfy both it and this License would be to
+refrain entirely from distribution of the Program.
+
+If any portion of this section is held invalid or unenforceable under
+any particular circumstance, the balance of the section is intended to
+apply and the section as a whole is intended to apply in other
+circumstances.
+
+It is not the purpose of this section to induce you to infringe any
+patents or other property right claims or to contest validity of any
+such claims; this section has the sole purpose of protecting the
+integrity of the free software distribution system, which is
+implemented by public license practices.  Many people have made
+generous contributions to the wide range of software distributed
+through that system in reliance on consistent application of that
+system; it is up to the author/donor to decide if he or she is willing
+to distribute software through any other system and a licensee cannot
+impose that choice.
+
+This section is intended to make thoroughly clear what is believed to
+be a consequence of the rest of this License.
+
+  8. If the distribution and/or use of the Program is restricted in
+certain countries either by patents or by copyrighted interfaces, the
+original copyright holder who places the Program under this License
+may add an explicit geographical distribution limitation excluding
+those countries, so that distribution is permitted only in or among
+countries not thus excluded.  In such case, this License incorporates
+the limitation as if written in the body of this License.
+
+  9. The Free Software Foundation may publish revised and/or new versions
+of the General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+Each version is given a distinguishing version number.  If the Program
+specifies a version number of this License which applies to it and "any
+later version", you have the option of following the terms and conditions
+either of that version or of any later version published by the Free
+Software Foundation.  If the Program does not specify a version number of
+this License, you may choose any version ever published by the Free Software
+Foundation.
+
+  10. If you wish to incorporate parts of the Program into other free
+programs whose distribution conditions are different, write to the author
+to ask for permission.  For software which is copyrighted by the Free
+Software Foundation, write to the Free Software Foundation; we sometimes
+make exceptions for this.  Our decision will be guided by the two goals
+of preserving the free status of all derivatives of our free software and
+of promoting the sharing and reuse of software generally.
+
+                            NO WARRANTY
+
+  11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
+FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW.  EXCEPT WHEN
+OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
+PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED
+OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  THE ENTIRE RISK AS
+TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU.  SHOULD THE
+PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING,
+REPAIR OR CORRECTION.
+
+  12. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR
+REDISTRIBUTE THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
+INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
+OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
+TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
+YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
+PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGES.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+convey the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software; you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation; either version 2 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License along
+    with this program; if not, write to the Free Software Foundation, Inc.,
+    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+
+Also add information on how to contact you by electronic and paper mail.
+
+If the program is interactive, make it output a short notice like this
+when it starts in an interactive mode:
+
+    Gnomovision version 69, Copyright (C) year name of author
+    Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, the commands you use may
+be called something other than `show w' and `show c'; they could even be
+mouse-clicks or menu items--whatever suits your program.
+
+You should also get your employer (if you work as a programmer) or your
+school, if any, to sign a "copyright disclaimer" for the program, if
+necessary.  Here is a sample; alter the names:
+
+  Yoyodyne, Inc., hereby disclaims all copyright interest in the program
+  `Gnomovision' (which makes passes at compilers) written by James Hacker.
+
+  <signature of Ty Coon>, 1 April 1989
+  Ty Coon, President of Vice
+
+This General Public License does not permit incorporating your program into
+proprietary programs.  If your program is a subroutine library, you may
+consider it more useful to permit linking proprietary applications with the
+library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.
```

### Comparing `nazo_rand-0.0.7/PKG-INFO` & `nazo_rand-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-Metadata-Version: 2.1
-Name: nazo_rand
-Version: 0.0.7
-Summary: A fast random number generator for python
-Author: bymoye
-Author-email: s3moye@gmail.com
-License: Free for non-commercial use
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: C++
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# nazo_rand
-
-Inspired to write from [Pyewacket](https://github.com/BrokenShell/Pyewacket)
-
-A fast random number generator for python
-
-`rand_int.choice(seq: list|Tuple) -> Any`
-example：
-
-```python
-from nazo_rand import choice
-temp = [1,2,3,4,5,6]
-choice(temp)
-```
-
-`rand_int.randbelow(a: int) -> int`
-example:
-
-```python
-from nazo_rand import randbelow
-randbelow(10)   # -> [0, 10)
-randbelow(0)    # -> [0, 0) => 0
-randbelow(-10)  # -> (-10, 0]
-```
-
-`rand_int.randint(a: int , b: int) -> int`
-example:
-
-```python
-from nazo_rand import randint
-randint(1, 10)   # -> [1, 10]
-randint(10, 1)   # -> [1, 10]
-randint(10, 10)  # -> [10, 10] => 10
-```
-
-`rand_int.randrange(start: int , stop: int = 0 , step: int = 1 )`
-example:
-
-```python
-from nazo_rand import randrange
-randrange(10)           # -> [0, 10) by whole numbers
-randrange(1, 10)        # -> [1, 10) by whole numbers
-randrange(1, 10, 2)     # -> [1, 10) by 2, odd numbers
-randrange(-10)          # -> [-10, 0) by 1
-randrange(10, 1)        # -> [1, 10) by 1
-randrange(10, 0, 2)     # -> [0, 10) by 2, even numbers
-randrange(10, 10, 0)    # -> [10, 10) => 10
-```
+Metadata-Version: 2.1
+Name: nazo_rand
+Version: 0.0.8
+Summary: A fast random number generator for python
+Author: bymoye
+Author-email: s3moye@gmail.com
+License: Free for non-commercial use
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: C++
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# nazo_rand
+
+Inspired to write from [Pyewacket](https://github.com/BrokenShell/Pyewacket)
+
+A fast random number generator for python
+
+`rand_int.choice(seq: list|Tuple) -> Any`
+exampleï¼š
+
+```python
+from nazo_rand import choice
+temp = [1,2,3,4,5,6]
+choice(temp)
+```
+
+`rand_int.randbelow(a: int) -> int`
+example:
+
+```python
+from nazo_rand import randbelow
+randbelow(10)   # -> [0, 10)
+randbelow(0)    # -> [0, 0) => 0
+randbelow(-10)  # -> (-10, 0]
+```
+
+`rand_int.randint(a: int , b: int) -> int`
+example:
+
+```python
+from nazo_rand import randint
+randint(1, 10)   # -> [1, 10]
+randint(10, 1)   # -> [1, 10]
+randint(10, 10)  # -> [10, 10] => 10
+```
+
+`rand_int.randrange(start: int , stop: int = 0 , step: int = 1 )`
+example:
+
+```python
+from nazo_rand import randrange
+randrange(10)           # -> [0, 10) by whole numbers
+randrange(1, 10)        # -> [1, 10) by whole numbers
+randrange(1, 10, 2)     # -> [1, 10) by 2, odd numbers
+randrange(-10)          # -> [-10, 0) by 1
+randrange(10, 1)        # -> [1, 10) by 1
+randrange(10, 0, 2)     # -> [0, 10) by 2, even numbers
+randrange(10, 10, 0)    # -> [10, 10) => 10
+```
```

### Comparing `nazo_rand-0.0.7/nazo_rand/nazo_rand.cpp` & `nazo_rand-0.0.8/nazo_rand/nazo_rand.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "nazo_rand/nazo_rand.hpp"
+            "nazo_rand\\nazo_rand.hpp"
         ],
         "extra_compile_args": [
-            "-std=c++17",
-            "-O3"
-        ],
-        "extra_link_args": [
-            "-Wl,-O3"
+            "/std:c++17",
+            "/O2"
         ],
         "include_dirs": [
             "nazo_rand"
         ],
         "language": "c++",
         "name": "nazo_rand.nazo_rand",
         "sources": [
@@ -988,23 +985,59 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "nazo_rand/nazo_rand.pyx",
+  "nazo_rand\\nazo_rand.pyx",
 };
+/* BufferFormatStructs.proto */
+#define IS_UNSIGNED(type) (((type) -1) > 0)
+struct __Pyx_StructField_;
+#define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
+typedef struct {
+  const char* name;
+  struct __Pyx_StructField_* fields;
+  size_t size;
+  size_t arraysize[8];
+  int ndim;
+  char typegroup;
+  char is_unsigned;
+  int flags;
+} __Pyx_TypeInfo;
+typedef struct __Pyx_StructField_ {
+  __Pyx_TypeInfo* type;
+  const char* name;
+  size_t offset;
+} __Pyx_StructField;
+typedef struct {
+  __Pyx_StructField* field;
+  size_t parent_offset;
+} __Pyx_BufFmt_StackElem;
+typedef struct {
+  __Pyx_StructField root;
+  __Pyx_BufFmt_StackElem* head;
+  size_t fmt_offset;
+  size_t new_count, enc_count;
+  size_t struct_alignment;
+  int is_complex;
+  char enc_type;
+  char new_packmode;
+  char enc_packmode;
+  char is_valid_array;
+} __Pyx_BufFmt_Context;
+
 
 /*--- Type declarations ---*/
 struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange;
 
 /* "nazo_rand/nazo_rand.pxd":14
- * cdef int64_t cy_random_below(int64_t number) nogil
- * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil
+ * # def int randbelow(int a)
+ * # def int randint(int a,int b)
  * cpdef int randrange(int start,int stop=?,int step=?)             # <<<<<<<<<<<<<<
  * cpdef double random_double(double a, double b)
  * cpdef double random_double_noargs()
  */
 struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange {
   int __pyx_n;
   int stop;
@@ -1081,24 +1114,37 @@
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
-/* SetItemInt.proto */
-#define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
-               __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
-static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
-static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
-                                               int is_list, int wraparound, int boundscheck);
+/* IsLittleEndian.proto */
+static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
+
+/* BufferFormatCheck.proto */
+static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
+static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
+                              __Pyx_BufFmt_StackElem* stack,
+                              __Pyx_TypeInfo* type);
+
+/* BufferGetAndValidate.proto */
+#define __Pyx_GetBufferAndValidate(buf, obj, dtype, flags, nd, cast, stack)\
+    ((obj == Py_None || obj == NULL) ?\
+    (__Pyx_ZeroBuffer(buf), 0) :\
+    __Pyx__GetBufferAndValidate(buf, obj, dtype, flags, nd, cast, stack))
+static int  __Pyx__GetBufferAndValidate(Py_buffer* buf, PyObject* obj,
+    __Pyx_TypeInfo* dtype, int flags, int nd, int cast, __Pyx_BufFmt_StackElem* stack);
+static void __Pyx_ZeroBuffer(Py_buffer* buf);
+static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
+static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
+static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
+#define __Pyx_BufPtrFull1d(type, buf, i0, s0, o0) (type)(__Pyx_BufPtrFull1d_imp(buf, i0, s0, o0))
+static CYTHON_INLINE void* __Pyx_BufPtrFull1d_imp(void* buf, Py_ssize_t i0, Py_ssize_t s0, Py_ssize_t o0);
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
 #define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
@@ -1199,14 +1245,24 @@
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* SetItemInt.proto */
+#define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
+               __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
+static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
+static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
+                                               int is_list, int wraparound, int boundscheck);
+
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
@@ -1314,34 +1370,57 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
+/* BufferStructDeclare.proto */
+typedef struct {
+  Py_ssize_t shape, strides, suboffsets;
+} __Pyx_Buf_DimInfo;
+typedef struct {
+  size_t refcount;
+  Py_buffer pybuffer;
+} __Pyx_Buffer;
+typedef struct {
+  __Pyx_Buffer *rcbuffer;
+  char *data;
+  __Pyx_Buf_DimInfo diminfo[8];
+} __Pyx_LocalBuf_ND;
+
+#if PY_MAJOR_VERSION < 3
+    static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags);
+    static void __Pyx_ReleaseBuffer(Py_buffer *view);
+#else
+    #define __Pyx_GetBuffer PyObject_GetBuffer
+    #define __Pyx_ReleaseBuffer PyBuffer_Release
+#endif
+
+
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
@@ -1365,30 +1444,30 @@
 
 
 /* Module declarations from 'libc.stdint' */
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'nazo_rand.nazo_rand' */
+static CYTHON_INLINE int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(int64_t); /*proto*/
+static CYTHON_INLINE int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(int64_t, int64_t); /*proto*/
 static void __pyx_f_9nazo_rand_9nazo_rand_shuffle(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choice(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choices(PyObject *, Py_ssize_t, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_sample(PyObject *, Py_ssize_t, int __pyx_skip_dispatch); /*proto*/
-static int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(int64_t); /*proto*/
-static int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(int64_t, int64_t); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_randrange(int, int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double, double, int __pyx_skip_dispatch); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(int __pyx_skip_dispatch); /*proto*/
+static __Pyx_TypeInfo __Pyx_TypeInfo_object = { "Python object", NULL, sizeof(PyObject *), { 0 }, 0, 'O', 0, 0 };
 #define __Pyx_MODULE_NAME "nazo_rand.nazo_rand"
 extern int __pyx_module_is_main_nazo_rand__nazo_rand;
 int __pyx_module_is_main_nazo_rand__nazo_rand = 0;
 
 /* Implementation of 'nazo_rand.nazo_rand' */
-static PyObject *__pyx_builtin_reversed;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ValueError;
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
@@ -1398,28 +1477,27 @@
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_count[] = "count";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_randint[] = "randint";
 static const char __pyx_k_shuffle[] = "shuffle";
-static const char __pyx_k_reversed[] = "reversed";
 static const char __pyx_k_container[] = "container";
 static const char __pyx_k_randbelow[] = "randbelow";
 static const char __pyx_k_randrange[] = "randrange";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_random_choice[] = "random_choice";
 static const char __pyx_k_random_double[] = "random_double";
 static const char __pyx_k_random_sample[] = "random_sample";
 static const char __pyx_k_random_choices[] = "random_choices";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_nazo_rand_nazo_rand[] = "nazo_rand.nazo_rand";
 static const char __pyx_k_random_double_noargs[] = "random_double_noargs";
 static const char __pyx_k_random_integer_noargs[] = "random_integer_noargs";
-static const char __pyx_k_nazo_rand_nazo_rand_pyx[] = "nazo_rand/nazo_rand.pyx";
+static const char __pyx_k_nazo_rand_nazo_rand_pyx[] = "nazo_rand\\nazo_rand.pyx";
 static const char __pyx_k_Sample_larger_than_population[] = "Sample larger than population";
 static PyObject *__pyx_kp_u_Sample_larger_than_population;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_a;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_b;
 static PyObject *__pyx_n_s_cline_in_traceback;
@@ -1437,15 +1515,14 @@
 static PyObject *__pyx_n_s_random_double;
 static PyObject *__pyx_n_s_random_double_noargs;
 static PyObject *__pyx_n_s_random_integer_noargs;
 static PyObject *__pyx_n_s_random_sample;
 static PyObject *__pyx_n_s_randrange;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_return;
-static PyObject *__pyx_n_s_reversed;
 static PyObject *__pyx_n_s_shuffle;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_2shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array); /* proto */
@@ -1477,70 +1554,70 @@
 static PyObject *__pyx_codeobj__18;
 static PyObject *__pyx_codeobj__19;
 /* Late includes */
 
 /* "nazo_rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b) nogil
  * 
- * cdef int64_t cy_random_below(int64_t number) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline int64_t cy_random_below(int64_t number) nogil:             # <<<<<<<<<<<<<<
  *     return random_below(number)
  * 
  */
 
-static int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(int64_t __pyx_v_number) {
+static CYTHON_INLINE int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(int64_t __pyx_v_number) {
   int64_t __pyx_r;
 
   /* "nazo_rand/nazo_rand.pyx":16
  * 
- * cdef int64_t cy_random_below(int64_t number) nogil:
+ * cdef inline int64_t cy_random_below(int64_t number) nogil:
  *     return random_below(number)             # <<<<<<<<<<<<<<
  * 
- * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:
+ * cdef inline int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:
  */
   __pyx_r = Storm::random_below(__pyx_v_number);
   goto __pyx_L0;
 
   /* "nazo_rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b) nogil
  * 
- * cdef int64_t cy_random_below(int64_t number) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline int64_t cy_random_below(int64_t number) nogil:             # <<<<<<<<<<<<<<
  *     return random_below(number)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "nazo_rand/nazo_rand.pyx":18
  *     return random_below(number)
  * 
- * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
 
-static int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(int64_t __pyx_v_a, int64_t __pyx_v_b) {
+static CYTHON_INLINE int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(int64_t __pyx_v_a, int64_t __pyx_v_b) {
   int64_t __pyx_r;
 
   /* "nazo_rand/nazo_rand.pyx":19
  * 
- * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:
+ * cdef inline int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:
  *     return uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * cpdef int random_integer_noargs():
  */
   __pyx_r = Storm::uniform_int_variate(__pyx_v_a, __pyx_v_b);
   goto __pyx_L0;
 
   /* "nazo_rand/nazo_rand.pyx":18
  *     return random_below(number)
  * 
- * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -1561,15 +1638,15 @@
   __Pyx_RefNannySetupContext("random_integer_noargs", 0);
 
   /* "nazo_rand/nazo_rand.pyx":22
  * 
  * cpdef int random_integer_noargs():
  *     return uniform_int_variate_noargs()             # <<<<<<<<<<<<<<
  * 
- * cpdef void shuffle(list array):
+ * cpdef void shuffle(list[object] array):
  */
   __pyx_r = Storm::uniform_int_variate_noargs();
   goto __pyx_L0;
 
   /* "nazo_rand/nazo_rand.pyx":21
  *     return uniform_int_variate(a, b)
  * 
@@ -1623,170 +1700,221 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
- * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
- *     for i in reversed(range(len(array) - 1)):
- *         j = randrange(i, len(array), 1)
+ * cpdef void shuffle(list[object] array):             # <<<<<<<<<<<<<<
+ *     cdef int i, j
+ *     cdef object temp
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
 static void __pyx_f_9nazo_rand_9nazo_rand_shuffle(PyObject *__pyx_v_array, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  Py_ssize_t __pyx_v_i;
+  int __pyx_v_i;
   int __pyx_v_j;
+  PyObject *__pyx_v_temp = 0;
+  int __pyx_v_length;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_array;
+  __Pyx_Buffer __pyx_pybuffer_array;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
-  Py_ssize_t __pyx_t_2;
-  Py_ssize_t __pyx_t_3;
-  int __pyx_t_4;
-  struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_4;
+  PyObject **__pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
-
-  /* "nazo_rand/nazo_rand.pyx":25
- * 
- * cpdef void shuffle(list array):
- *     for i in reversed(range(len(array) - 1)):             # <<<<<<<<<<<<<<
- *         j = randrange(i, len(array), 1)
- *         array[i], array[j] = array[j], array[i]
- */
-  if (unlikely(__pyx_v_array == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_pybuffer_array.pybuffer.buf = NULL;
+  __pyx_pybuffer_array.refcount = 0;
+  __pyx_pybuffernd_array.data = NULL;
+  __pyx_pybuffernd_array.rcbuffer = &__pyx_pybuffer_array;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_INDIRECT| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 24, __pyx_L1_error)
   }
-  __pyx_t_1 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 25, __pyx_L1_error)
-  for (__pyx_t_2 = (__pyx_t_1 - 1)-1; __pyx_t_2 >= 0; __pyx_t_2-=1) {
+  __pyx_pybuffernd_array.diminfo[0].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_array.diminfo[0].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_array.diminfo[0].suboffsets = __pyx_pybuffernd_array.rcbuffer->pybuffer.suboffsets[0];
+
+  /* "nazo_rand/nazo_rand.pyx":27
+ *     cdef int i, j
+ *     cdef object temp
+ *     cdef int length = len(array)             # <<<<<<<<<<<<<<
+ *     for i in range(length - 1, 0, -1):
+ *         j = cy_uniform_int_variate(0, i)
+ */
+  __pyx_t_1 = PyObject_Length(__pyx_v_array); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_v_length = __pyx_t_1;
+
+  /* "nazo_rand/nazo_rand.pyx":28
+ *     cdef object temp
+ *     cdef int length = len(array)
+ *     for i in range(length - 1, 0, -1):             # <<<<<<<<<<<<<<
+ *         j = cy_uniform_int_variate(0, i)
+ *         temp = array[i]
+ */
+  for (__pyx_t_2 = (__pyx_v_length - 1); __pyx_t_2 > 0; __pyx_t_2-=1) {
     __pyx_v_i = __pyx_t_2;
 
-    /* "nazo_rand/nazo_rand.pyx":26
- * cpdef void shuffle(list array):
- *     for i in reversed(range(len(array) - 1)):
- *         j = randrange(i, len(array), 1)             # <<<<<<<<<<<<<<
- *         array[i], array[j] = array[j], array[i]
- * 
- */
-    if (unlikely(__pyx_v_array == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 26, __pyx_L1_error)
-    }
-    __pyx_t_3 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 26, __pyx_L1_error)
-    __pyx_t_5.__pyx_n = 2;
-    __pyx_t_5.stop = __pyx_t_3;
-    __pyx_t_5.step = 1;
-    __pyx_t_4 = __pyx_f_9nazo_rand_9nazo_rand_randrange(__pyx_v_i, 0, &__pyx_t_5); 
-    __pyx_v_j = __pyx_t_4;
-
-    /* "nazo_rand/nazo_rand.pyx":27
- *     for i in reversed(range(len(array) - 1)):
- *         j = randrange(i, len(array), 1)
- *         array[i], array[j] = array[j], array[i]             # <<<<<<<<<<<<<<
- * 
+    /* "nazo_rand/nazo_rand.pyx":29
+ *     cdef int length = len(array)
+ *     for i in range(length - 1, 0, -1):
+ *         j = cy_uniform_int_variate(0, i)             # <<<<<<<<<<<<<<
+ *         temp = array[i]
+ *         array[i] = array[j]
+ */
+    __pyx_v_j = __pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(0, __pyx_v_i);
+
+    /* "nazo_rand/nazo_rand.pyx":30
+ *     for i in range(length - 1, 0, -1):
+ *         j = cy_uniform_int_variate(0, i)
+ *         temp = array[i]             # <<<<<<<<<<<<<<
+ *         array[i] = array[j]
+ *         array[j] = temp
+ */
+    __pyx_t_4 = __pyx_v_i;
+    __pyx_t_3 = (PyObject *) *__Pyx_BufPtrFull1d(PyObject **, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_pybuffernd_array.diminfo[0].suboffsets);
+    if (unlikely(__pyx_t_3 == NULL)) __pyx_t_3 = Py_None;
+    __Pyx_INCREF((PyObject*)__pyx_t_3);
+    __Pyx_XDECREF_SET(__pyx_v_temp, __pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "nazo_rand/nazo_rand.pyx":31
+ *         j = cy_uniform_int_variate(0, i)
+ *         temp = array[i]
+ *         array[i] = array[j]             # <<<<<<<<<<<<<<
+ *         array[j] = temp
+ * 
+ */
+    __pyx_t_4 = __pyx_v_j;
+    __pyx_t_3 = (PyObject *) *__Pyx_BufPtrFull1d(PyObject **, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_pybuffernd_array.diminfo[0].suboffsets);
+    if (unlikely(__pyx_t_3 == NULL)) __pyx_t_3 = Py_None;
+    __Pyx_INCREF((PyObject*)__pyx_t_3);
+    __pyx_t_4 = __pyx_v_i;
+    __pyx_t_5 = __Pyx_BufPtrFull1d(PyObject **, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_pybuffernd_array.diminfo[0].suboffsets);
+    __Pyx_XGOTREF(*__pyx_t_5);
+    __Pyx_INCREF(__pyx_t_3); __Pyx_XDECREF(*__pyx_t_5);
+    *__pyx_t_5 = __pyx_t_3;
+    __Pyx_XGIVEREF(*__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "nazo_rand/nazo_rand.pyx":32
+ *         temp = array[i]
+ *         array[i] = array[j]
+ *         array[j] = temp             # <<<<<<<<<<<<<<
  * 
+ * def randbelow(a:int) -> int:
  */
-    if (unlikely(__pyx_v_array == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 27, __pyx_L1_error)
-    }
-    __pyx_t_6 = PyList_GET_ITEM(__pyx_v_array, __pyx_v_j);
-    __Pyx_INCREF(__pyx_t_6);
-    if (unlikely(__pyx_v_array == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 27, __pyx_L1_error)
-    }
-    __pyx_t_7 = PyList_GET_ITEM(__pyx_v_array, __pyx_v_i);
-    __Pyx_INCREF(__pyx_t_7);
-    if (unlikely(__pyx_v_array == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 27, __pyx_L1_error)
-    }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_6, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 27, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(__pyx_v_array == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 27, __pyx_L1_error)
-    }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_j, __pyx_t_7, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 27, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_4 = __pyx_v_j;
+    __pyx_t_5 = __Pyx_BufPtrFull1d(PyObject **, __pyx_pybuffernd_array.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_array.diminfo[0].strides, __pyx_pybuffernd_array.diminfo[0].suboffsets);
+    __Pyx_XGOTREF(*__pyx_t_5);
+    __Pyx_INCREF(__pyx_v_temp); __Pyx_XDECREF(*__pyx_t_5);
+    *__pyx_t_5 = __pyx_v_temp;
+    __Pyx_XGIVEREF(*__pyx_t_5);
   }
 
   /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
- * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
- *     for i in reversed(range(len(array) - 1)):
- *         j = randrange(i, len(array), 1)
+ * cpdef void shuffle(list[object] array):             # <<<<<<<<<<<<<<
+ *     cdef int i, j
+ *     cdef object temp
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_3);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
   __Pyx_WriteUnraisable("nazo_rand.nazo_rand.shuffle", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  goto __pyx_L2;
   __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XDECREF(__pyx_v_temp);
   __Pyx_RefNannyFinishContext();
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array); /*proto*/
 static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_3shuffle = {"shuffle", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_3shuffle, METH_O, 0};
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shuffle (wrapper)", 0);
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), (&PyList_Type), 1, "array", 1))) __PYX_ERR(0, 24, __pyx_L1_error)
-  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_2shuffle(__pyx_self, ((PyObject*)__pyx_v_array));
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_2shuffle(__pyx_self, ((PyObject *)__pyx_v_array));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_2shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array) {
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_array;
+  __Pyx_Buffer __pyx_pybuffer_array;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
+  __pyx_pybuffer_array.pybuffer.buf = NULL;
+  __pyx_pybuffer_array.refcount = 0;
+  __pyx_pybuffernd_array.data = NULL;
+  __pyx_pybuffernd_array.rcbuffer = &__pyx_pybuffer_array;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_array, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_INDIRECT, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_array.diminfo[0].strides = __pyx_pybuffernd_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_array.diminfo[0].shape = __pyx_pybuffernd_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_array.diminfo[0].suboffsets = __pyx_pybuffernd_array.rcbuffer->pybuffer.suboffsets[0];
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_9nazo_rand_9nazo_rand_shuffle(__pyx_v_array, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_9nazo_rand_9nazo_rand_shuffle(((PyObject *)__pyx_v_array), 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
   __Pyx_AddTraceback("nazo_rand.nazo_rand.shuffle", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
+  goto __pyx_L2;
   __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_array.rcbuffer->pybuffer);
+  __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":30
- * 
+/* "nazo_rand/nazo_rand.pyx":34
+ *         array[j] = temp
  * 
  * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
 
 /* Python wrapper */
@@ -1809,31 +1937,31 @@
   int64_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randbelow", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":31
+  /* "nazo_rand/nazo_rand.pyx":35
  * 
  * def randbelow(a:int) -> int:
  *     return random_below(a)             # <<<<<<<<<<<<<<
  * 
  * def randint(a:int, b:int) -> int:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int64_t(Storm::random_below(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int64_t(Storm::random_below(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":30
- * 
+  /* "nazo_rand/nazo_rand.pyx":34
+ *         array[j] = temp
  * 
  * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
 
   /* function exit code */
@@ -1843,15 +1971,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":33
+/* "nazo_rand/nazo_rand.pyx":37
  *     return random_below(a)
  * 
  * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
  *     return cy_uniform_int_variate(a, b)
  * 
  */
 
@@ -1886,32 +2014,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 33, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 37, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 33, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 37, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_a = values[0];
     __pyx_v_b = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 33, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 37, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_6randint(__pyx_self, __pyx_v_a, __pyx_v_b);
 
@@ -1927,31 +2055,31 @@
   int64_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randint", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":34
+  /* "nazo_rand/nazo_rand.pyx":38
  * 
  * def randint(a:int, b:int) -> int:
  *     return cy_uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_b); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(__pyx_t_1, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_b); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(__pyx_t_1, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":33
+  /* "nazo_rand/nazo_rand.pyx":37
  *     return random_below(a)
  * 
  * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
  *     return cy_uniform_int_variate(a, b)
  * 
  */
 
@@ -1962,15 +2090,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":40
+/* "nazo_rand/nazo_rand.pyx":44
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
 
@@ -1982,39 +2110,39 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":41
+  /* "nazo_rand/nazo_rand.pyx":45
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):
  *     cdef Py_ssize_t index = cy_random_below(len(container))             # <<<<<<<<<<<<<<
  *     return container[index]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 45, __pyx_L1_error)
   __pyx_v_index = __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(__pyx_t_1);
 
-  /* "nazo_rand/nazo_rand.pyx":42
+  /* "nazo_rand/nazo_rand.pyx":46
  * cpdef object random_choice(object container):
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_container, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_container, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":40
+  /* "nazo_rand/nazo_rand.pyx":44
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
 
@@ -2048,15 +2176,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choice(__pyx_v_container, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choice(__pyx_v_container, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2065,15 +2193,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":46
+/* "nazo_rand/nazo_rand.pyx":50
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
 
@@ -2090,51 +2218,51 @@
   int64_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choices", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":47
+  /* "nazo_rand/nazo_rand.pyx":51
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):
  *     cdef Py_ssize_t container_length = len(container)             # <<<<<<<<<<<<<<
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 51, __pyx_L1_error)
   __pyx_v_container_length = __pyx_t_1;
 
-  /* "nazo_rand/nazo_rand.pyx":48
+  /* "nazo_rand/nazo_rand.pyx":52
  * cpdef list[object] random_choices(object container, Py_ssize_t count):
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_v_count;
     __pyx_t_3 = __pyx_t_1;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_7genexpr__pyx_v__ = __pyx_t_4;
       __pyx_t_5 = __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(__pyx_v_container_length);
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_container, __pyx_t_5, int64_t, 1, __Pyx_PyInt_From_int64_t, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 48, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_container, __pyx_t_5, int64_t, 1, __Pyx_PyInt_From_int64_t, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 52, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 48, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 52, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   } /* exit inner scope */
   __pyx_r = ((PyObject *)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":46
+  /* "nazo_rand/nazo_rand.pyx":50
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
 
@@ -2181,32 +2309,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_container)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, 1); __PYX_ERR(0, 46, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, 1); __PYX_ERR(0, 50, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_choices") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_choices") < 0)) __PYX_ERR(0, 50, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_container = values[0];
-    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
+    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 50, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choices", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_10random_choices(__pyx_self, __pyx_v_container, __pyx_v_count);
 
@@ -2220,15 +2348,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choices", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choices(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choices(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2237,15 +2365,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":52
+/* "nazo_rand/nazo_rand.pyx":56
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
 
@@ -2264,146 +2392,146 @@
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_sample", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":53
+  /* "nazo_rand/nazo_rand.pyx":57
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):
  *     cdef Py_ssize_t container_length = len(container)             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j
  *     cdef list result = [None] * count
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 57, __pyx_L1_error)
   __pyx_v_container_length = __pyx_t_1;
 
-  /* "nazo_rand/nazo_rand.pyx":55
+  /* "nazo_rand/nazo_rand.pyx":59
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  *     cdef list result = [None] * count             # <<<<<<<<<<<<<<
  *     cdef list temp = list(container)
  * 
  */
-  __pyx_t_2 = PyList_New(1 * ((__pyx_v_count<0) ? 0:__pyx_v_count)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1 * ((__pyx_v_count<0) ? 0:__pyx_v_count)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   { Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < __pyx_v_count; __pyx_temp++) {
       __Pyx_INCREF(Py_None);
       __Pyx_GIVEREF(Py_None);
       PyList_SET_ITEM(__pyx_t_2, __pyx_temp, Py_None);
     }
   }
   __pyx_v_result = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":56
+  /* "nazo_rand/nazo_rand.pyx":60
  *     cdef Py_ssize_t i, j
  *     cdef list result = [None] * count
  *     cdef list temp = list(container)             # <<<<<<<<<<<<<<
  * 
  *     if count > container_length:
  */
-  __pyx_t_2 = PySequence_List(__pyx_v_container); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_v_container); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_temp = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":58
+  /* "nazo_rand/nazo_rand.pyx":62
  *     cdef list temp = list(container)
  * 
  *     if count > container_length:             # <<<<<<<<<<<<<<
  *         raise ValueError("Sample larger than population")
  * 
  */
   __pyx_t_3 = ((__pyx_v_count > __pyx_v_container_length) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "nazo_rand/nazo_rand.pyx":59
+    /* "nazo_rand/nazo_rand.pyx":63
  * 
  *     if count > container_length:
  *         raise ValueError("Sample larger than population")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(count):
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 59, __pyx_L1_error)
+    __PYX_ERR(0, 63, __pyx_L1_error)
 
-    /* "nazo_rand/nazo_rand.pyx":58
+    /* "nazo_rand/nazo_rand.pyx":62
  *     cdef list temp = list(container)
  * 
  *     if count > container_length:             # <<<<<<<<<<<<<<
  *         raise ValueError("Sample larger than population")
  * 
  */
   }
 
-  /* "nazo_rand/nazo_rand.pyx":61
+  /* "nazo_rand/nazo_rand.pyx":65
  *         raise ValueError("Sample larger than population")
  * 
  *     for i in range(count):             # <<<<<<<<<<<<<<
  *         j = uniform_int_variate(i, container_length - 1)
  *         result[i] = temp[j]
  */
   __pyx_t_1 = __pyx_v_count;
   __pyx_t_4 = __pyx_t_1;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "nazo_rand/nazo_rand.pyx":62
+    /* "nazo_rand/nazo_rand.pyx":66
  * 
  *     for i in range(count):
  *         j = uniform_int_variate(i, container_length - 1)             # <<<<<<<<<<<<<<
  *         result[i] = temp[j]
  *         temp[j] = temp[i]
  */
     __pyx_v_j = Storm::uniform_int_variate(__pyx_v_i, (__pyx_v_container_length - 1));
 
-    /* "nazo_rand/nazo_rand.pyx":63
+    /* "nazo_rand/nazo_rand.pyx":67
  *     for i in range(count):
  *         j = uniform_int_variate(i, container_length - 1)
  *         result[i] = temp[j]             # <<<<<<<<<<<<<<
  *         temp[j] = temp[i]
  * 
  */
     __pyx_t_2 = PyList_GET_ITEM(__pyx_v_temp, __pyx_v_j);
     __Pyx_INCREF(__pyx_t_2);
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_result, __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 63, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_result, __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 67, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "nazo_rand/nazo_rand.pyx":64
+    /* "nazo_rand/nazo_rand.pyx":68
  *         j = uniform_int_variate(i, container_length - 1)
  *         result[i] = temp[j]
  *         temp[j] = temp[i]             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
     __pyx_t_2 = PyList_GET_ITEM(__pyx_v_temp, __pyx_v_i);
     __Pyx_INCREF(__pyx_t_2);
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_temp, __pyx_v_j, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 64, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_temp, __pyx_v_j, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
 
-  /* "nazo_rand/nazo_rand.pyx":66
+  /* "nazo_rand/nazo_rand.pyx":70
  *         temp[j] = temp[i]
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":52
+  /* "nazo_rand/nazo_rand.pyx":56
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
 
@@ -2451,32 +2579,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_container)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, 1); __PYX_ERR(0, 52, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, 1); __PYX_ERR(0, 56, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_sample") < 0)) __PYX_ERR(0, 52, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_sample") < 0)) __PYX_ERR(0, 56, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_container = values[0];
-    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L3_error)
+    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 56, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 52, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 56, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_12random_sample(__pyx_self, __pyx_v_container, __pyx_v_count);
 
@@ -2490,15 +2618,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_sample", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_sample(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_sample(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2507,15 +2635,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":68
+/* "nazo_rand/nazo_rand.pyx":72
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
@@ -2534,56 +2662,56 @@
       __pyx_v_stop = __pyx_optional_args->stop;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_step = __pyx_optional_args->step;
       }
     }
   }
 
-  /* "nazo_rand/nazo_rand.pyx":69
+  /* "nazo_rand/nazo_rand.pyx":73
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   __pyx_t_1 = ((__pyx_v_stop == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "nazo_rand/nazo_rand.pyx":70
+    /* "nazo_rand/nazo_rand.pyx":74
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:
  *         stop, start = start, 0             # <<<<<<<<<<<<<<
  *     return random_range(start, stop, step)
  * 
  */
     __pyx_t_2 = __pyx_v_start;
     __pyx_t_3 = 0;
     __pyx_v_stop = __pyx_t_2;
     __pyx_v_start = __pyx_t_3;
 
-    /* "nazo_rand/nazo_rand.pyx":69
+    /* "nazo_rand/nazo_rand.pyx":73
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   }
 
-  /* "nazo_rand/nazo_rand.pyx":71
+  /* "nazo_rand/nazo_rand.pyx":75
  *     if stop == 0:
  *         stop, start = start, 0
  *     return random_range(start, stop, step)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::random_range(__pyx_v_start, __pyx_v_stop, __pyx_v_step);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":68
+  /* "nazo_rand/nazo_rand.pyx":72
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
@@ -2637,42 +2765,42 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_step);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 68, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 72, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
+      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
     } else {
       __pyx_v_stop = ((int)0);
     }
     if (values[2]) {
-      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
+      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
     } else {
       __pyx_v_step = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 68, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 72, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.randrange", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_14randrange(__pyx_self, __pyx_v_start, __pyx_v_stop, __pyx_v_step);
 
@@ -2692,15 +2820,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randrange", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.stop = __pyx_v_stop;
   __pyx_t_2.step = __pyx_v_step;
   __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_randrange(__pyx_v_start, 0, &__pyx_t_2); 
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2709,39 +2837,39 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":74
+/* "nazo_rand/nazo_rand.pyx":78
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_17random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double __pyx_v_a, double __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":75
+  /* "nazo_rand/nazo_rand.pyx":79
  * 
  * cpdef double random_double(double a, double b):
  *     return uniform_real_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::uniform_real_variate(__pyx_v_a, __pyx_v_b);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":74
+  /* "nazo_rand/nazo_rand.pyx":78
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
@@ -2782,32 +2910,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 74, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 78, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 74, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 78, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
-    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
+    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L3_error)
+    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 74, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 78, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_16random_double(__pyx_self, __pyx_v_a, __pyx_v_b);
 
@@ -2821,15 +2949,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2838,36 +2966,36 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":78
+/* "nazo_rand/nazo_rand.pyx":82
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_19random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":79
+  /* "nazo_rand/nazo_rand.pyx":83
  * 
  * cpdef double random_double_noargs():
  *     return uniform_real_variate_noargs()             # <<<<<<<<<<<<<<
  */
   __pyx_r = Storm::uniform_real_variate_noargs();
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":78
+  /* "nazo_rand/nazo_rand.pyx":82
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
   /* function exit code */
@@ -2895,15 +3023,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2982,43 +3110,41 @@
   {&__pyx_n_s_random_double, __pyx_k_random_double, sizeof(__pyx_k_random_double), 0, 0, 1, 1},
   {&__pyx_n_s_random_double_noargs, __pyx_k_random_double_noargs, sizeof(__pyx_k_random_double_noargs), 0, 0, 1, 1},
   {&__pyx_n_s_random_integer_noargs, __pyx_k_random_integer_noargs, sizeof(__pyx_k_random_integer_noargs), 0, 0, 1, 1},
   {&__pyx_n_s_random_sample, __pyx_k_random_sample, sizeof(__pyx_k_random_sample), 0, 0, 1, 1},
   {&__pyx_n_s_randrange, __pyx_k_randrange, sizeof(__pyx_k_randrange), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
-  {&__pyx_n_s_reversed, __pyx_k_reversed, sizeof(__pyx_k_reversed), 0, 0, 1, 1},
   {&__pyx_n_s_shuffle, __pyx_k_shuffle, sizeof(__pyx_k_shuffle), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 63, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":59
+  /* "nazo_rand/nazo_rand.pyx":63
  * 
  *     if count > container_length:
  *         raise ValueError("Sample larger than population")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(count):
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Sample_larger_than_population); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Sample_larger_than_population); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 63, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "nazo_rand/nazo_rand.pyx":21
  *     return uniform_int_variate(a, b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
@@ -3026,114 +3152,114 @@
  * 
  */
   __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 21, __pyx_L1_error)
 
   /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
- * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
- *     for i in reversed(range(len(array) - 1)):
- *         j = randrange(i, len(array), 1)
+ * cpdef void shuffle(list[object] array):             # <<<<<<<<<<<<<<
+ *     cdef int i, j
+ *     cdef object temp
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 24, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":30
- * 
+  /* "nazo_rand/nazo_rand.pyx":34
+ *         array[j] = temp
  * 
  * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_a); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_a); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 34, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":33
+  /* "nazo_rand/nazo_rand.pyx":37
  *     return random_below(a)
  * 
  * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
  *     return cy_uniform_int_variate(a, b)
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randint, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randint, 37, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 37, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":40
+  /* "nazo_rand/nazo_rand.pyx":44
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_container); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_container); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 44, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 44, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":46
+  /* "nazo_rand/nazo_rand.pyx":50
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
-  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choices, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choices, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 50, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":52
+  /* "nazo_rand/nazo_rand.pyx":56
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
-  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_sample, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_sample, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 56, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":68
+  /* "nazo_rand/nazo_rand.pyx":72
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randrange, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randrange, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 72, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":74
+  /* "nazo_rand/nazo_rand.pyx":78
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double, 74, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 78, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":78
+  /* "nazo_rand/nazo_rand.pyx":82
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 82, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3171,21 +3297,21 @@
 static int __Pyx_modinit_function_export_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
+  if (__Pyx_ExportFunction("cy_random_below", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_cy_random_below, "int64_t (int64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("cy_uniform_int_variate", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate, "int64_t (int64_t, int64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("shuffle", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_shuffle, "void (PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_integer_noargs", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs, "int (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_choice", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_choice, "PyObject *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_choices", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_choices, "PyObject *(PyObject *, Py_ssize_t, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_sample", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_sample, "PyObject *(PyObject *, Py_ssize_t, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("cy_random_below", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_cy_random_below, "int64_t (int64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("cy_uniform_int_variate", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate, "int64_t (int64_t, int64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("randrange", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randrange, "int (int, int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_double", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_double, "double (double, double, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_double_noargs", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs, "double (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
@@ -3436,129 +3562,129 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_integer_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
- * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
- *     for i in reversed(range(len(array) - 1)):
- *         j = randrange(i, len(array), 1)
+ * cpdef void shuffle(list[object] array):             # <<<<<<<<<<<<<<
+ *     cdef int i, j
+ *     cdef object temp
  */
   __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":30
- * 
+  /* "nazo_rand/nazo_rand.pyx":34
+ *         array[j] = temp
  * 
  * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_2) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_2) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":33
+  /* "nazo_rand/nazo_rand.pyx":37
  *     return random_below(a)
  * 
  * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
  *     return cy_uniform_int_variate(a, b)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_b, __pyx_n_u_int) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_7randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_b, __pyx_n_u_int) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_7randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":40
+  /* "nazo_rand/nazo_rand.pyx":44
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_9random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_9random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":46
+  /* "nazo_rand/nazo_rand.pyx":50
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_11random_choices, 0, __pyx_n_s_random_choices, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_11random_choices, 0, __pyx_n_s_random_choices, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choices, __pyx_t_1) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choices, __pyx_t_1) < 0) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":52
+  /* "nazo_rand/nazo_rand.pyx":56
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_13random_sample, 0, __pyx_n_s_random_sample, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_13random_sample, 0, __pyx_n_s_random_sample, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_sample, __pyx_t_1) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_sample, __pyx_t_1) < 0) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":68
+  /* "nazo_rand/nazo_rand.pyx":72
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_15randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_15randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":74
+  /* "nazo_rand/nazo_rand.pyx":78
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_17random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_17random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":78
+  /* "nazo_rand/nazo_rand.pyx":82
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_19random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_19random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "nazo_rand/nazo_rand.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * # distutils: language = c++
  * cimport cython
  */
@@ -3634,65 +3760,584 @@
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
-/* SetItemInt */
-static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
-    int r;
-    if (!j) return -1;
-    r = PyObject_SetItem(o, j, v);
-    Py_DECREF(j);
-    return r;
+/* IsLittleEndian */
+static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
+{
+  union {
+    uint32_t u32;
+    uint8_t u8[4];
+  } S;
+  S.u32 = 0x01020304;
+  return S.u8[0] == 4;
+}
+
+/* BufferFormatCheck */
+static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
+                              __Pyx_BufFmt_StackElem* stack,
+                              __Pyx_TypeInfo* type) {
+  stack[0].field = &ctx->root;
+  stack[0].parent_offset = 0;
+  ctx->root.type = type;
+  ctx->root.name = "buffer dtype";
+  ctx->root.offset = 0;
+  ctx->head = stack;
+  ctx->head->field = &ctx->root;
+  ctx->fmt_offset = 0;
+  ctx->head->parent_offset = 0;
+  ctx->new_packmode = '@';
+  ctx->enc_packmode = '@';
+  ctx->new_count = 1;
+  ctx->enc_count = 0;
+  ctx->enc_type = 0;
+  ctx->is_complex = 0;
+  ctx->is_valid_array = 0;
+  ctx->struct_alignment = 0;
+  while (type->typegroup == 'S') {
+    ++ctx->head;
+    ctx->head->field = type->fields;
+    ctx->head->parent_offset = 0;
+    type = type->fields->type;
+  }
 }
-static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v, int is_list,
-                                               CYTHON_NCP_UNUSED int wraparound, CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = (!wraparound) ? i : ((likely(i >= 0)) ? i : i + PyList_GET_SIZE(o));
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o)))) {
-            PyObject* old = PyList_GET_ITEM(o, n);
-            Py_INCREF(v);
-            PyList_SET_ITEM(o, n, v);
-            Py_DECREF(old);
-            return 1;
-        }
+static int __Pyx_BufFmt_ParseNumber(const char** ts) {
+    int count;
+    const char* t = *ts;
+    if (*t < '0' || *t > '9') {
+      return -1;
     } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_ass_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return -1;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_ass_item(o, i, v);
-        }
+        count = *t++ - '0';
+        while (*t >= '0' && *t <= '9') {
+            count *= 10;
+            count += *t++ - '0';
+        }
+    }
+    *ts = t;
+    return count;
+}
+static int __Pyx_BufFmt_ExpectNumber(const char **ts) {
+    int number = __Pyx_BufFmt_ParseNumber(ts);
+    if (number == -1)
+        PyErr_Format(PyExc_ValueError,\
+                     "Does not understand character buffer dtype format string ('%c')", **ts);
+    return number;
+}
+static void __Pyx_BufFmt_RaiseUnexpectedChar(char ch) {
+  PyErr_Format(PyExc_ValueError,
+               "Unexpected format string character: '%c'", ch);
+}
+static const char* __Pyx_BufFmt_DescribeTypeChar(char ch, int is_complex) {
+  switch (ch) {
+    case '?': return "'bool'";
+    case 'c': return "'char'";
+    case 'b': return "'signed char'";
+    case 'B': return "'unsigned char'";
+    case 'h': return "'short'";
+    case 'H': return "'unsigned short'";
+    case 'i': return "'int'";
+    case 'I': return "'unsigned int'";
+    case 'l': return "'long'";
+    case 'L': return "'unsigned long'";
+    case 'q': return "'long long'";
+    case 'Q': return "'unsigned long long'";
+    case 'f': return (is_complex ? "'complex float'" : "'float'");
+    case 'd': return (is_complex ? "'complex double'" : "'double'");
+    case 'g': return (is_complex ? "'complex long double'" : "'long double'");
+    case 'T': return "a struct";
+    case 'O': return "Python object";
+    case 'P': return "a pointer";
+    case 's': case 'p': return "a string";
+    case 0: return "end";
+    default: return "unparseable format string";
+  }
+}
+static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return 2;
+    case 'i': case 'I': case 'l': case 'L': return 4;
+    case 'q': case 'Q': return 8;
+    case 'f': return (is_complex ? 8 : 4);
+    case 'd': return (is_complex ? 16 : 8);
+    case 'g': {
+      PyErr_SetString(PyExc_ValueError, "Python does not define a standard format string size for long double ('g')..");
+      return 0;
     }
-#else
-#if CYTHON_COMPILING_IN_PYPY
-    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
-#else
-    if (is_list || PySequence_Check(o))
+    case 'O': case 'P': return sizeof(void*);
+    default:
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+}
+static size_t __Pyx_BufFmt_TypeCharToNativeSize(char ch, int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return sizeof(short);
+    case 'i': case 'I': return sizeof(int);
+    case 'l': case 'L': return sizeof(long);
+    #ifdef HAVE_LONG_LONG
+    case 'q': case 'Q': return sizeof(PY_LONG_LONG);
+    #endif
+    case 'f': return sizeof(float) * (is_complex ? 2 : 1);
+    case 'd': return sizeof(double) * (is_complex ? 2 : 1);
+    case 'g': return sizeof(long double) * (is_complex ? 2 : 1);
+    case 'O': case 'P': return sizeof(void*);
+    default: {
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+  }
+}
+typedef struct { char c; short x; } __Pyx_st_short;
+typedef struct { char c; int x; } __Pyx_st_int;
+typedef struct { char c; long x; } __Pyx_st_long;
+typedef struct { char c; float x; } __Pyx_st_float;
+typedef struct { char c; double x; } __Pyx_st_double;
+typedef struct { char c; long double x; } __Pyx_st_longdouble;
+typedef struct { char c; void *x; } __Pyx_st_void_p;
+#ifdef HAVE_LONG_LONG
+typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
 #endif
-    {
-        return PySequence_SetItem(o, i, v);
+static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
+    case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
+    case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
+#ifdef HAVE_LONG_LONG
+    case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
+#endif
+    case 'f': return sizeof(__Pyx_st_float) - sizeof(float);
+    case 'd': return sizeof(__Pyx_st_double) - sizeof(double);
+    case 'g': return sizeof(__Pyx_st_longdouble) - sizeof(long double);
+    case 'P': case 'O': return sizeof(__Pyx_st_void_p) - sizeof(void*);
+    default:
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
     }
+}
+/* These are for computing the padding at the end of the struct to align
+   on the first member of the struct. This will probably the same as above,
+   but we don't have any guarantees.
+ */
+typedef struct { short x; char c; } __Pyx_pad_short;
+typedef struct { int x; char c; } __Pyx_pad_int;
+typedef struct { long x; char c; } __Pyx_pad_long;
+typedef struct { float x; char c; } __Pyx_pad_float;
+typedef struct { double x; char c; } __Pyx_pad_double;
+typedef struct { long double x; char c; } __Pyx_pad_longdouble;
+typedef struct { void *x; char c; } __Pyx_pad_void_p;
+#ifdef HAVE_LONG_LONG
+typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
 #endif
-    return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
+static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
+    case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
+    case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
+#ifdef HAVE_LONG_LONG
+    case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
+#endif
+    case 'f': return sizeof(__Pyx_pad_float) - sizeof(float);
+    case 'd': return sizeof(__Pyx_pad_double) - sizeof(double);
+    case 'g': return sizeof(__Pyx_pad_longdouble) - sizeof(long double);
+    case 'P': case 'O': return sizeof(__Pyx_pad_void_p) - sizeof(void*);
+    default:
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+}
+static char __Pyx_BufFmt_TypeCharToGroup(char ch, int is_complex) {
+  switch (ch) {
+    case 'c':
+        return 'H';
+    case 'b': case 'h': case 'i':
+    case 'l': case 'q': case 's': case 'p':
+        return 'I';
+    case '?': case 'B': case 'H': case 'I': case 'L': case 'Q':
+        return 'U';
+    case 'f': case 'd': case 'g':
+        return (is_complex ? 'C' : 'R');
+    case 'O':
+        return 'O';
+    case 'P':
+        return 'P';
+    default: {
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+  }
+}
+static void __Pyx_BufFmt_RaiseExpected(__Pyx_BufFmt_Context* ctx) {
+  if (ctx->head == NULL || ctx->head->field == &ctx->root) {
+    const char* expected;
+    const char* quote;
+    if (ctx->head == NULL) {
+      expected = "end";
+      quote = "";
+    } else {
+      expected = ctx->head->field->type->name;
+      quote = "'";
+    }
+    PyErr_Format(PyExc_ValueError,
+                 "Buffer dtype mismatch, expected %s%s%s but got %s",
+                 quote, expected, quote,
+                 __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex));
+  } else {
+    __Pyx_StructField* field = ctx->head->field;
+    __Pyx_StructField* parent = (ctx->head - 1)->field;
+    PyErr_Format(PyExc_ValueError,
+                 "Buffer dtype mismatch, expected '%s' but got %s in '%s.%s'",
+                 field->type->name, __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex),
+                 parent->type->name, field->name);
+  }
+}
+static int __Pyx_BufFmt_ProcessTypeChunk(__Pyx_BufFmt_Context* ctx) {
+  char group;
+  size_t size, offset, arraysize = 1;
+  if (ctx->enc_type == 0) return 0;
+  if (ctx->head->field->type->arraysize[0]) {
+    int i, ndim = 0;
+    if (ctx->enc_type == 's' || ctx->enc_type == 'p') {
+        ctx->is_valid_array = ctx->head->field->type->ndim == 1;
+        ndim = 1;
+        if (ctx->enc_count != ctx->head->field->type->arraysize[0]) {
+            PyErr_Format(PyExc_ValueError,
+                         "Expected a dimension of size %zu, got %zu",
+                         ctx->head->field->type->arraysize[0], ctx->enc_count);
+            return -1;
+        }
+    }
+    if (!ctx->is_valid_array) {
+      PyErr_Format(PyExc_ValueError, "Expected %d dimensions, got %d",
+                   ctx->head->field->type->ndim, ndim);
+      return -1;
+    }
+    for (i = 0; i < ctx->head->field->type->ndim; i++) {
+      arraysize *= ctx->head->field->type->arraysize[i];
+    }
+    ctx->is_valid_array = 0;
+    ctx->enc_count = 1;
+  }
+  group = __Pyx_BufFmt_TypeCharToGroup(ctx->enc_type, ctx->is_complex);
+  do {
+    __Pyx_StructField* field = ctx->head->field;
+    __Pyx_TypeInfo* type = field->type;
+    if (ctx->enc_packmode == '@' || ctx->enc_packmode == '^') {
+      size = __Pyx_BufFmt_TypeCharToNativeSize(ctx->enc_type, ctx->is_complex);
+    } else {
+      size = __Pyx_BufFmt_TypeCharToStandardSize(ctx->enc_type, ctx->is_complex);
+    }
+    if (ctx->enc_packmode == '@') {
+      size_t align_at = __Pyx_BufFmt_TypeCharToAlignment(ctx->enc_type, ctx->is_complex);
+      size_t align_mod_offset;
+      if (align_at == 0) return -1;
+      align_mod_offset = ctx->fmt_offset % align_at;
+      if (align_mod_offset > 0) ctx->fmt_offset += align_at - align_mod_offset;
+      if (ctx->struct_alignment == 0)
+          ctx->struct_alignment = __Pyx_BufFmt_TypeCharToPadding(ctx->enc_type,
+                                                                 ctx->is_complex);
+    }
+    if (type->size != size || type->typegroup != group) {
+      if (type->typegroup == 'C' && type->fields != NULL) {
+        size_t parent_offset = ctx->head->parent_offset + field->offset;
+        ++ctx->head;
+        ctx->head->field = type->fields;
+        ctx->head->parent_offset = parent_offset;
+        continue;
+      }
+      if ((type->typegroup == 'H' || group == 'H') && type->size == size) {
+      } else {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return -1;
+      }
+    }
+    offset = ctx->head->parent_offset + field->offset;
+    if (ctx->fmt_offset != offset) {
+      PyErr_Format(PyExc_ValueError,
+                   "Buffer dtype mismatch; next field is at offset %" CYTHON_FORMAT_SSIZE_T "d but %" CYTHON_FORMAT_SSIZE_T "d expected",
+                   (Py_ssize_t)ctx->fmt_offset, (Py_ssize_t)offset);
+      return -1;
+    }
+    ctx->fmt_offset += size;
+    if (arraysize)
+      ctx->fmt_offset += (arraysize - 1) * size;
+    --ctx->enc_count;
+    while (1) {
+      if (field == &ctx->root) {
+        ctx->head = NULL;
+        if (ctx->enc_count != 0) {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return -1;
+        }
+        break;
+      }
+      ctx->head->field = ++field;
+      if (field->type == NULL) {
+        --ctx->head;
+        field = ctx->head->field;
+        continue;
+      } else if (field->type->typegroup == 'S') {
+        size_t parent_offset = ctx->head->parent_offset + field->offset;
+        if (field->type->fields->type == NULL) continue;
+        field = field->type->fields;
+        ++ctx->head;
+        ctx->head->field = field;
+        ctx->head->parent_offset = parent_offset;
+        break;
+      } else {
+        break;
+      }
+    }
+  } while (ctx->enc_count);
+  ctx->enc_type = 0;
+  ctx->is_complex = 0;
+  return 0;
+}
+static PyObject *
+__pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
+{
+    const char *ts = *tsp;
+    int i = 0, number, ndim;
+    ++ts;
+    if (ctx->new_count != 1) {
+        PyErr_SetString(PyExc_ValueError,
+                        "Cannot handle repeated arrays in format string");
+        return NULL;
+    }
+    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+    ndim = ctx->head->field->type->ndim;
+    while (*ts && *ts != ')') {
+        switch (*ts) {
+            case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
+            default:  break;
+        }
+        number = __Pyx_BufFmt_ExpectNumber(&ts);
+        if (number == -1) return NULL;
+        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i])
+            return PyErr_Format(PyExc_ValueError,
+                        "Expected a dimension of size %zu, got %d",
+                        ctx->head->field->type->arraysize[i], number);
+        if (*ts != ',' && *ts != ')')
+            return PyErr_Format(PyExc_ValueError,
+                                "Expected a comma in format string, got '%c'", *ts);
+        if (*ts == ',') ts++;
+        i++;
+    }
+    if (i != ndim)
+        return PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
+                            ctx->head->field->type->ndim, i);
+    if (!*ts) {
+        PyErr_SetString(PyExc_ValueError,
+                        "Unexpected end of format string, expected ')'");
+        return NULL;
+    }
+    ctx->is_valid_array = 1;
+    ctx->new_count = 1;
+    *tsp = ++ts;
+    return Py_None;
+}
+static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts) {
+  int got_Z = 0;
+  while (1) {
+    switch(*ts) {
+      case 0:
+        if (ctx->enc_type != 0 && ctx->head == NULL) {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return NULL;
+        }
+        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+        if (ctx->head != NULL) {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return NULL;
+        }
+        return ts;
+      case ' ':
+      case '\r':
+      case '\n':
+        ++ts;
+        break;
+      case '<':
+        if (!__Pyx_Is_Little_Endian()) {
+          PyErr_SetString(PyExc_ValueError, "Little-endian buffer not supported on big-endian compiler");
+          return NULL;
+        }
+        ctx->new_packmode = '=';
+        ++ts;
+        break;
+      case '>':
+      case '!':
+        if (__Pyx_Is_Little_Endian()) {
+          PyErr_SetString(PyExc_ValueError, "Big-endian buffer not supported on little-endian compiler");
+          return NULL;
+        }
+        ctx->new_packmode = '=';
+        ++ts;
+        break;
+      case '=':
+      case '@':
+      case '^':
+        ctx->new_packmode = *ts++;
+        break;
+      case 'T':
+        {
+          const char* ts_after_sub;
+          size_t i, struct_count = ctx->new_count;
+          size_t struct_alignment = ctx->struct_alignment;
+          ctx->new_count = 1;
+          ++ts;
+          if (*ts != '{') {
+            PyErr_SetString(PyExc_ValueError, "Buffer acquisition: Expected '{' after 'T'");
+            return NULL;
+          }
+          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+          ctx->enc_type = 0;
+          ctx->enc_count = 0;
+          ctx->struct_alignment = 0;
+          ++ts;
+          ts_after_sub = ts;
+          for (i = 0; i != struct_count; ++i) {
+            ts_after_sub = __Pyx_BufFmt_CheckString(ctx, ts);
+            if (!ts_after_sub) return NULL;
+          }
+          ts = ts_after_sub;
+          if (struct_alignment) ctx->struct_alignment = struct_alignment;
+        }
+        break;
+      case '}':
+        {
+          size_t alignment = ctx->struct_alignment;
+          ++ts;
+          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+          ctx->enc_type = 0;
+          if (alignment && ctx->fmt_offset % alignment) {
+            ctx->fmt_offset += alignment - (ctx->fmt_offset % alignment);
+          }
+        }
+        return ts;
+      case 'x':
+        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+        ctx->fmt_offset += ctx->new_count;
+        ctx->new_count = 1;
+        ctx->enc_count = 0;
+        ctx->enc_type = 0;
+        ctx->enc_packmode = ctx->new_packmode;
+        ++ts;
+        break;
+      case 'Z':
+        got_Z = 1;
+        ++ts;
+        if (*ts != 'f' && *ts != 'd' && *ts != 'g') {
+          __Pyx_BufFmt_RaiseUnexpectedChar('Z');
+          return NULL;
+        }
+        CYTHON_FALLTHROUGH;
+      case '?': case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
+      case 'l': case 'L': case 'q': case 'Q':
+      case 'f': case 'd': case 'g':
+      case 'O': case 'p':
+        if ((ctx->enc_type == *ts) && (got_Z == ctx->is_complex) &&
+            (ctx->enc_packmode == ctx->new_packmode) && (!ctx->is_valid_array)) {
+          ctx->enc_count += ctx->new_count;
+          ctx->new_count = 1;
+          got_Z = 0;
+          ++ts;
+          break;
+        }
+        CYTHON_FALLTHROUGH;
+      case 's':
+        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+        ctx->enc_count = ctx->new_count;
+        ctx->enc_packmode = ctx->new_packmode;
+        ctx->enc_type = *ts;
+        ctx->is_complex = got_Z;
+        ++ts;
+        ctx->new_count = 1;
+        got_Z = 0;
+        break;
+      case ':':
+        ++ts;
+        while(*ts != ':') ++ts;
+        ++ts;
+        break;
+      case '(':
+        if (!__pyx_buffmt_parse_array(ctx, &ts)) return NULL;
+        break;
+      default:
+        {
+          int number = __Pyx_BufFmt_ExpectNumber(&ts);
+          if (number == -1) return NULL;
+          ctx->new_count = (size_t)number;
+        }
+    }
+  }
 }
 
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
+/* BufferGetAndValidate */
+  static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info) {
+  if (unlikely(info->buf == NULL)) return;
+  if (info->suboffsets == __Pyx_minusones) info->suboffsets = NULL;
+  __Pyx_ReleaseBuffer(info);
+}
+static void __Pyx_ZeroBuffer(Py_buffer* buf) {
+  buf->buf = NULL;
+  buf->obj = NULL;
+  buf->strides = __Pyx_zeros;
+  buf->shape = __Pyx_zeros;
+  buf->suboffsets = __Pyx_minusones;
+}
+static int __Pyx__GetBufferAndValidate(
+        Py_buffer* buf, PyObject* obj,  __Pyx_TypeInfo* dtype, int flags,
+        int nd, int cast, __Pyx_BufFmt_StackElem* stack)
+{
+  buf->buf = NULL;
+  if (unlikely(__Pyx_GetBuffer(obj, buf, flags) == -1)) {
+    __Pyx_ZeroBuffer(buf);
+    return -1;
+  }
+  if (unlikely(buf->ndim != nd)) {
+    PyErr_Format(PyExc_ValueError,
+                 "Buffer has wrong number of dimensions (expected %d, got %d)",
+                 nd, buf->ndim);
+    goto fail;
+  }
+  if (!cast) {
+    __Pyx_BufFmt_Context ctx;
+    __Pyx_BufFmt_Init(&ctx, stack, dtype);
+    if (!__Pyx_BufFmt_CheckString(&ctx, buf->format)) goto fail;
+  }
+  if (unlikely((size_t)buf->itemsize != dtype->size)) {
+    PyErr_Format(PyExc_ValueError,
+      "Item size of buffer (%" CYTHON_FORMAT_SSIZE_T "d byte%s) does not match size of '%s' (%" CYTHON_FORMAT_SSIZE_T "d byte%s)",
+      buf->itemsize, (buf->itemsize > 1) ? "s" : "",
+      dtype->name, (Py_ssize_t)dtype->size, (dtype->size > 1) ? "s" : "");
+    goto fail;
+  }
+  if (buf->suboffsets == NULL) buf->suboffsets = __Pyx_minusones;
+  return 0;
+fail:;
+  __Pyx_SafeReleaseBuffer(buf);
+  return -1;
+}
+
+
+static CYTHON_INLINE void* __Pyx_BufPtrFull1d_imp(void* buf, Py_ssize_t i0, Py_ssize_t s0, Py_ssize_t o0) {
+  char* ptr = (char*)buf;
+ptr += s0 * i0;
+if (o0 >= 0) ptr = *((char**)ptr) + o0;
+
+return ptr;
+}
+  /* PyErrFetchRestore */
+  #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -3708,15 +4353,15 @@
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* WriteUnraisableException */
-static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+  static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
                                   CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
                                   int full_traceback, CYTHON_UNUSED int nogil) {
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
@@ -3748,15 +4393,15 @@
 #ifdef WITH_THREAD
     if (nogil)
         PyGILState_Release(state);
 #endif
 }
 
 /* ArgTypeTest */
-static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+  static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     else if (exact) {
         #if PY_MAJOR_VERSION == 2
@@ -3769,15 +4414,15 @@
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
 /* RaiseArgTupleInvalid */
-static void __Pyx_RaiseArgtupleInvalid(
+  static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
 {
     Py_ssize_t num_expected;
@@ -3795,29 +4440,29 @@
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* RaiseDoubleKeywords */
-static void __Pyx_RaiseDoubleKeywordsError(
+  static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
         #if PY_MAJOR_VERSION >= 3
         "%s() got multiple values for keyword argument '%U'", func_name, kw_name);
         #else
         "%s() got multiple values for keyword argument '%s'", func_name,
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
-static int __Pyx_ParseOptionalKeywords(
+  static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
@@ -3911,15 +4556,15 @@
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+  static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
@@ -3998,15 +4643,15 @@
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
@@ -4018,15 +4663,15 @@
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* RaiseException */
-#if PY_MAJOR_VERSION < 3
+  #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
     Py_XINCREF(type);
     if (!value || value == Py_None)
         value = NULL;
     else
@@ -4176,16 +4821,65 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
+/* SetItemInt */
+  static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
+    int r;
+    if (!j) return -1;
+    r = PyObject_SetItem(o, j, v);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v, int is_list,
+                                               CYTHON_NCP_UNUSED int wraparound, CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = (!wraparound) ? i : ((likely(i >= 0)) ? i : i + PyList_GET_SIZE(o));
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o)))) {
+            PyObject* old = PyList_GET_ITEM(o, n);
+            Py_INCREF(v);
+            PyList_SET_ITEM(o, n, v);
+            Py_DECREF(old);
+            return 1;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_ass_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return -1;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_ass_item(o, i, v);
+        }
+    }
+#else
+#if CYTHON_COMPILING_IN_PYPY
+    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
+#else
+    if (is_list || PySequence_Check(o))
+#endif
+    {
+        return PySequence_SetItem(o, i, v);
+    }
+#endif
+    return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
+}
+
 /* FetchCommonType */
-static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+  static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
     PyObject* fake_module;
     PyTypeObject* cached_type = NULL;
     fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
     if (!fake_module) return NULL;
     Py_INCREF(fake_module);
     cached_type = (PyTypeObject*) PyObject_GetAttrString(fake_module, type->tp_name);
     if (cached_type) {
@@ -4216,15 +4910,15 @@
 bad:
     Py_XDECREF(cached_type);
     cached_type = NULL;
     goto done;
 }
 
 /* CythonFunctionShared */
-#include <structmember.h>
+  #include <structmember.h>
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, CYTHON_UNUSED void *closure)
 {
     if (unlikely(op->func_doc == NULL)) {
         if (op->func.m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
             op->func_doc = PyUnicode_FromString(op->func.m_ml->ml_doc);
@@ -4832,28 +5526,28 @@
 static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
     __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
     m->func_annotations = dict;
     Py_INCREF(dict);
 }
 
 /* CythonFunction */
-static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
     PyObject *op = __Pyx_CyFunction_Init(
         PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
         ml, flags, qualname, closure, module, globals, code
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* PyDictVersioning */
-#if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
+  #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
     PyObject **dictptr = NULL;
     Py_ssize_t offset = Py_TYPE(obj)->tp_dictoffset;
@@ -4871,15 +5565,15 @@
     if (unlikely(!dict) || unlikely(tp_dict_version != __PYX_GET_DICT_VERSION(dict)))
         return 0;
     return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
 #endif
 
 /* CLineInTraceback */
-#ifndef CYTHON_CLINE_IN_TRACEBACK
+  #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
@@ -4913,15 +5607,15 @@
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -4993,15 +5687,15 @@
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
-#include "compile.h"
+  #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
 #if PY_VERSION_HEX >= 0x030b00a6
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
@@ -5099,16 +5793,36 @@
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
-/* CIntFromPyVerify */
-#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+#if PY_MAJOR_VERSION < 3
+static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
+    if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
+    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
+    return -1;
+}
+static void __Pyx_ReleaseBuffer(Py_buffer *view) {
+    PyObject *obj = view->obj;
+    if (!obj) return;
+    if (PyObject_CheckBuffer(obj)) {
+        PyBuffer_Release(view);
+        return;
+    }
+    if ((0)) {}
+    view->obj = NULL;
+    Py_DECREF(obj);
+}
+#endif
+
+
+  /* CIntFromPyVerify */
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
         func_type value = func_value;\
         if (sizeof(target_type) < sizeof(func_type)) {\
@@ -5122,15 +5836,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntFromPy */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -5318,15 +6032,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -5355,16 +6069,54 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
-static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *x) {
+  static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -5552,15 +6304,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int64_t");
     return (int64_t) -1;
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value) {
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -5589,54 +6341,16 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int64_t),
                                      little, !is_unsigned);
     }
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -5824,15 +6538,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* FastTypeChecks */
-#if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = a->tp_base;
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
@@ -5924,15 +6638,15 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-static int __Pyx_check_binary_version(void) {
+  static int __Pyx_check_binary_version(void) {
     char ctversion[5];
     int same=1, i, found_dot;
     const char* rt_from_call = Py_GetVersion();
     PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
     found_dot = 0;
     for (i = 0; i < 4; i++) {
         if (!ctversion[i]) {
@@ -5962,15 +6676,15 @@
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* FunctionExport */
-static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig) {
+  static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(__pyx_m, (char *)"__pyx_capi__");
@@ -5999,15 +6713,15 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* InitStrings */
-static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
         #if PY_MAJOR_VERSION < 3
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
```

### Comparing `nazo_rand-0.0.7/nazo_rand/nazo_rand.hpp` & `nazo_rand-0.0.8/nazo_rand/nazo_rand.hpp`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-#pragma once
-#include <algorithm>
-#include <cstdint>
-#include <limits>
-#include <random>
-
-namespace Storm
-{
-    using Integer = int64_t;
-
-    inline std::mt19937_64 &get_generator()
-    {
-        static std::mt19937_64 generator{std::random_device{}()};
-        return generator;
-    }
-
-    inline void seed(uint64_t seed)
-    {
-        get_generator().seed(seed);
-    }
-
-    inline Integer uniform_int_variate(Integer a, Integer b)
-    {
-        std::uniform_int_distribution<Integer> distribution{std::min(a, b), std::max(b, a)};
-        return distribution(get_generator());
-    }
-
-    inline Integer uniform_int_variate_noargs()
-    {
-        return uniform_int_variate(std::numeric_limits<Integer>::min(), std::numeric_limits<Integer>::max());
-    }
-
-    inline Integer random_below(Integer number)
-    {
-        return uniform_int_variate(0, number - 1);
-    }
-
-    inline Integer random_range(Integer start, Integer stop, Integer step)
-    {
-        if (start == stop || step == 0)
-            return start;
-
-        Integer width = std::abs(stop - start) - 1;
-        Integer step_size = std::abs(step);
-        Integer num_steps = (width + step_size) / step_size;
-        Integer random_step = random_below(num_steps);
-
-        if (step > 0)
-        {
-            Integer pivot = std::min(start, stop);
-            return pivot + step_size * random_step;
-        }
-        else
-        {
-            Integer pivot = std::max(start, stop);
-            return pivot - step_size * random_step;
-        }
-    }
-
-    inline double uniform_real_variate(double a, double b)
-    {
-        std::uniform_real_distribution<double> distribution{a, b};
-        return distribution(get_generator());
-    }
-
-    inline double uniform_real_variate_noargs()
-    {
-        std::uniform_real_distribution<double> distribution{0.0, 1.0};
-        return distribution(get_generator());
-    }
-
-}
+#pragma once
+#include <algorithm>
+#include <cstdint>
+#include <limits>
+#include <random>
+
+namespace Storm
+{
+    using Integer = int64_t;
+
+    inline std::mt19937_64 &get_generator()
+    {
+        static std::mt19937_64 generator{std::random_device{}()};
+        return generator;
+    }
+
+    inline void seed(uint64_t seed)
+    {
+        get_generator().seed(seed);
+    }
+
+    inline Integer uniform_int_variate(Integer a, Integer b)
+    {
+        std::uniform_int_distribution<Integer> distribution{std::min(a, b), std::max(b, a)};
+        return distribution(get_generator());
+    }
+
+    inline Integer uniform_int_variate_noargs()
+    {
+        return uniform_int_variate(std::numeric_limits<Integer>::min(), std::numeric_limits<Integer>::max());
+    }
+
+    inline Integer random_below(Integer number)
+    {
+        return uniform_int_variate(0, number - 1);
+    }
+
+    inline Integer random_range(Integer start, Integer stop, Integer step)
+    {
+        if (start == stop || step == 0)
+            return start;
+
+        Integer width = std::abs(stop - start) - 1;
+        Integer step_size = std::abs(step);
+        Integer num_steps = (width + step_size) / step_size;
+        Integer random_step = random_below(num_steps);
+
+        if (step > 0)
+        {
+            Integer pivot = std::min(start, stop);
+            return pivot + step_size * random_step;
+        }
+        else
+        {
+            Integer pivot = std::max(start, stop);
+            return pivot - step_size * random_step;
+        }
+    }
+
+    inline double uniform_real_variate(double a, double b)
+    {
+        std::uniform_real_distribution<double> distribution{a, b};
+        return distribution(get_generator());
+    }
+
+    inline double uniform_real_variate_noargs()
+    {
+        std::uniform_real_distribution<double> distribution{0.0, 1.0};
+        return distribution(get_generator());
+    }
+
+}
```

### Comparing `nazo_rand-0.0.7/nazo_rand.egg-info/PKG-INFO` & `nazo_rand-0.0.8/nazo_rand.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-Metadata-Version: 2.1
-Name: nazo-rand
-Version: 0.0.7
-Summary: A fast random number generator for python
-Author: bymoye
-Author-email: s3moye@gmail.com
-License: Free for non-commercial use
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: C++
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# nazo_rand
-
-Inspired to write from [Pyewacket](https://github.com/BrokenShell/Pyewacket)
-
-A fast random number generator for python
-
-`rand_int.choice(seq: list|Tuple) -> Any`
-example：
-
-```python
-from nazo_rand import choice
-temp = [1,2,3,4,5,6]
-choice(temp)
-```
-
-`rand_int.randbelow(a: int) -> int`
-example:
-
-```python
-from nazo_rand import randbelow
-randbelow(10)   # -> [0, 10)
-randbelow(0)    # -> [0, 0) => 0
-randbelow(-10)  # -> (-10, 0]
-```
-
-`rand_int.randint(a: int , b: int) -> int`
-example:
-
-```python
-from nazo_rand import randint
-randint(1, 10)   # -> [1, 10]
-randint(10, 1)   # -> [1, 10]
-randint(10, 10)  # -> [10, 10] => 10
-```
-
-`rand_int.randrange(start: int , stop: int = 0 , step: int = 1 )`
-example:
-
-```python
-from nazo_rand import randrange
-randrange(10)           # -> [0, 10) by whole numbers
-randrange(1, 10)        # -> [1, 10) by whole numbers
-randrange(1, 10, 2)     # -> [1, 10) by 2, odd numbers
-randrange(-10)          # -> [-10, 0) by 1
-randrange(10, 1)        # -> [1, 10) by 1
-randrange(10, 0, 2)     # -> [0, 10) by 2, even numbers
-randrange(10, 10, 0)    # -> [10, 10) => 10
-```
+Metadata-Version: 2.1
+Name: nazo-rand
+Version: 0.0.8
+Summary: A fast random number generator for python
+Author: bymoye
+Author-email: s3moye@gmail.com
+License: Free for non-commercial use
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: C++
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# nazo_rand
+
+Inspired to write from [Pyewacket](https://github.com/BrokenShell/Pyewacket)
+
+A fast random number generator for python
+
+`rand_int.choice(seq: list|Tuple) -> Any`
+exampleï¼š
+
+```python
+from nazo_rand import choice
+temp = [1,2,3,4,5,6]
+choice(temp)
+```
+
+`rand_int.randbelow(a: int) -> int`
+example:
+
+```python
+from nazo_rand import randbelow
+randbelow(10)   # -> [0, 10)
+randbelow(0)    # -> [0, 0) => 0
+randbelow(-10)  # -> (-10, 0]
+```
+
+`rand_int.randint(a: int , b: int) -> int`
+example:
+
+```python
+from nazo_rand import randint
+randint(1, 10)   # -> [1, 10]
+randint(10, 1)   # -> [1, 10]
+randint(10, 10)  # -> [10, 10] => 10
+```
+
+`rand_int.randrange(start: int , stop: int = 0 , step: int = 1 )`
+example:
+
+```python
+from nazo_rand import randrange
+randrange(10)           # -> [0, 10) by whole numbers
+randrange(1, 10)        # -> [1, 10) by whole numbers
+randrange(1, 10, 2)     # -> [1, 10) by 2, odd numbers
+randrange(-10)          # -> [-10, 0) by 1
+randrange(10, 1)        # -> [1, 10) by 1
+randrange(10, 0, 2)     # -> [0, 10) by 2, even numbers
+randrange(10, 10, 0)    # -> [10, 10) => 10
+```
```

