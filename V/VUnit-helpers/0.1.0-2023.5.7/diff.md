# Comparing `tmp/VUnit-helpers-0.1.0.tar.gz` & `tmp/VUnit-helpers-2023.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VUnit-helpers-0.1.0.tar", last modified: Fri May  5 11:48:58 2023, max compression
+gzip compressed data, was "VUnit-helpers-2023.5.7.tar", last modified: Mon May  8 11:06:37 2023, max compression
```

## Comparing `VUnit-helpers-0.1.0.tar` & `VUnit-helpers-2023.5.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:48:58.458074 VUnit-helpers-0.1.0/
--rw-rw-rw-   0        0        0    17097 2023-05-04 11:38:33.000000 VUnit-helpers-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4399 2023-05-05 11:48:58.455094 VUnit-helpers-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3260 2023-05-05 10:50:48.000000 VUnit-helpers-0.1.0/README.md
--rw-rw-rw-   0        0        0     1320 2023-05-05 11:38:50.000000 VUnit-helpers-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 11:48:58.459082 VUnit-helpers-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 11:48:58.418006 VUnit-helpers-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 11:48:58.452575 VUnit-helpers-0.1.0/src/VUnit_helpers.egg-info/
--rw-rw-rw-   0        0        0     4399 2023-05-05 11:48:58.000000 VUnit-helpers-0.1.0/src/VUnit_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-05-05 11:48:58.000000 VUnit-helpers-0.1.0/src/VUnit_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:48:58.000000 VUnit-helpers-0.1.0/src/VUnit_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 11:48:58.000000 VUnit-helpers-0.1.0/src/VUnit_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-05 11:48:58.000000 VUnit-helpers-0.1.0/src/VUnit_helpers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      278 2023-05-04 11:38:33.000000 VUnit-helpers-0.1.0/src/__init__.py
--rw-rw-rw-   0        0        0    12019 2023-05-04 17:31:27.000000 VUnit-helpers-0.1.0/src/vunit_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:06:37.246524 VUnit-helpers-2023.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-08 11:06:28.000000 VUnit-helpers-2023.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-08 11:06:37.246524 VUnit-helpers-2023.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-08 11:06:28.000000 VUnit-helpers-2023.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-08 11:06:28.000000 VUnit-helpers-2023.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:06:37.246524 VUnit-helpers-2023.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:06:37.246524 VUnit-helpers-2023.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:06:37.246524 VUnit-helpers-2023.5.7/src/VUnit_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-08 11:06:37.000000 VUnit-helpers-2023.5.7/src/VUnit_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 11:06:37.000000 VUnit-helpers-2023.5.7/src/VUnit_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:06:37.000000 VUnit-helpers-2023.5.7/src/VUnit_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 11:06:37.000000 VUnit-helpers-2023.5.7/src/VUnit_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 11:06:37.000000 VUnit-helpers-2023.5.7/src/VUnit_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 11:06:28.000000 VUnit-helpers-2023.5.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-05-08 11:06:28.000000 VUnit-helpers-2023.5.7/src/vunit_helpers.py
```

### Comparing `VUnit-helpers-0.1.0/LICENSE` & `VUnit-helpers-2023.5.7/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,373 +1,373 @@
-Mozilla Public License Version 2.0
-==================================
-
-1. Definitions
---------------
-
-1.1. "Contributor"
-    means each individual or legal entity that creates, contributes to
-    the creation of, or owns Covered Software.
-
-1.2. "Contributor Version"
-    means the combination of the Contributions of others (if any) used
-    by a Contributor and that particular Contributor's Contribution.
-
-1.3. "Contribution"
-    means Covered Software of a particular Contributor.
-
-1.4. "Covered Software"
-    means Source Code Form to which the initial Contributor has attached
-    the notice in Exhibit A, the Executable Form of such Source Code
-    Form, and Modifications of such Source Code Form, in each case
-    including portions thereof.
-
-1.5. "Incompatible With Secondary Licenses"
-    means
-
-    (a) that the initial Contributor has attached the notice described
-        in Exhibit B to the Covered Software; or
-
-    (b) that the Covered Software was made available under the terms of
-        version 1.1 or earlier of the License, but not also under the
-        terms of a Secondary License.
-
-1.6. "Executable Form"
-    means any form of the work other than Source Code Form.
-
-1.7. "Larger Work"
-    means a work that combines Covered Software with other material, in 
-    a separate file or files, that is not Covered Software.
-
-1.8. "License"
-    means this document.
-
-1.9. "Licensable"
-    means having the right to grant, to the maximum extent possible,
-    whether at the time of the initial grant or subsequently, any and
-    all of the rights conveyed by this License.
-
-1.10. "Modifications"
-    means any of the following:
-
-    (a) any file in Source Code Form that results from an addition to,
-        deletion from, or modification of the contents of Covered
-        Software; or
-
-    (b) any new file in Source Code Form that contains any Covered
-        Software.
-
-1.11. "Patent Claims" of a Contributor
-    means any patent claim(s), including without limitation, method,
-    process, and apparatus claims, in any patent Licensable by such
-    Contributor that would be infringed, but for the grant of the
-    License, by the making, using, selling, offering for sale, having
-    made, import, or transfer of either its Contributions or its
-    Contributor Version.
-
-1.12. "Secondary License"
-    means either the GNU General Public License, Version 2.0, the GNU
-    Lesser General Public License, Version 2.1, the GNU Affero General
-    Public License, Version 3.0, or any later versions of those
-    licenses.
-
-1.13. "Source Code Form"
-    means the form of the work preferred for making modifications.
-
-1.14. "You" (or "Your")
-    means an individual or a legal entity exercising rights under this
-    License. For legal entities, "You" includes any entity that
-    controls, is controlled by, or is under common control with You. For
-    purposes of this definition, "control" means (a) the power, direct
-    or indirect, to cause the direction or management of such entity,
-    whether by contract or otherwise, or (b) ownership of more than
-    fifty percent (50%) of the outstanding shares or beneficial
-    ownership of such entity.
-
-2. License Grants and Conditions
---------------------------------
-
-2.1. Grants
-
-Each Contributor hereby grants You a world-wide, royalty-free,
-non-exclusive license:
-
-(a) under intellectual property rights (other than patent or trademark)
-    Licensable by such Contributor to use, reproduce, make available,
-    modify, display, perform, distribute, and otherwise exploit its
-    Contributions, either on an unmodified basis, with Modifications, or
-    as part of a Larger Work; and
-
-(b) under Patent Claims of such Contributor to make, use, sell, offer
-    for sale, have made, import, and otherwise transfer either its
-    Contributions or its Contributor Version.
-
-2.2. Effective Date
-
-The licenses granted in Section 2.1 with respect to any Contribution
-become effective for each Contribution on the date the Contributor first
-distributes such Contribution.
-
-2.3. Limitations on Grant Scope
-
-The licenses granted in this Section 2 are the only rights granted under
-this License. No additional rights or licenses will be implied from the
-distribution or licensing of Covered Software under this License.
-Notwithstanding Section 2.1(b) above, no patent license is granted by a
-Contributor:
-
-(a) for any code that a Contributor has removed from Covered Software;
-    or
-
-(b) for infringements caused by: (i) Your and any other third party's
-    modifications of Covered Software, or (ii) the combination of its
-    Contributions with other software (except as part of its Contributor
-    Version); or
-
-(c) under Patent Claims infringed by Covered Software in the absence of
-    its Contributions.
-
-This License does not grant any rights in the trademarks, service marks,
-or logos of any Contributor (except as may be necessary to comply with
-the notice requirements in Section 3.4).
-
-2.4. Subsequent Licenses
-
-No Contributor makes additional grants as a result of Your choice to
-distribute the Covered Software under a subsequent version of this
-License (see Section 10.2) or under the terms of a Secondary License (if
-permitted under the terms of Section 3.3).
-
-2.5. Representation
-
-Each Contributor represents that the Contributor believes its
-Contributions are its original creation(s) or it has sufficient rights
-to grant the rights to its Contributions conveyed by this License.
-
-2.6. Fair Use
-
-This License is not intended to limit any rights You have under
-applicable copyright doctrines of fair use, fair dealing, or other
-equivalents.
-
-2.7. Conditions
-
-Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
-in Section 2.1.
-
-3. Responsibilities
--------------------
-
-3.1. Distribution of Source Form
-
-All distribution of Covered Software in Source Code Form, including any
-Modifications that You create or to which You contribute, must be under
-the terms of this License. You must inform recipients that the Source
-Code Form of the Covered Software is governed by the terms of this
-License, and how they can obtain a copy of this License. You may not
-attempt to alter or restrict the recipients' rights in the Source Code
-Form.
-
-3.2. Distribution of Executable Form
-
-If You distribute Covered Software in Executable Form then:
-
-(a) such Covered Software must also be made available in Source Code
-    Form, as described in Section 3.1, and You must inform recipients of
-    the Executable Form how they can obtain a copy of such Source Code
-    Form by reasonable means in a timely manner, at a charge no more
-    than the cost of distribution to the recipient; and
-
-(b) You may distribute such Executable Form under the terms of this
-    License, or sublicense it under different terms, provided that the
-    license for the Executable Form does not attempt to limit or alter
-    the recipients' rights in the Source Code Form under this License.
-
-3.3. Distribution of a Larger Work
-
-You may create and distribute a Larger Work under terms of Your choice,
-provided that You also comply with the requirements of this License for
-the Covered Software. If the Larger Work is a combination of Covered
-Software with a work governed by one or more Secondary Licenses, and the
-Covered Software is not Incompatible With Secondary Licenses, this
-License permits You to additionally distribute such Covered Software
-under the terms of such Secondary License(s), so that the recipient of
-the Larger Work may, at their option, further distribute the Covered
-Software under the terms of either this License or such Secondary
-License(s).
-
-3.4. Notices
-
-You may not remove or alter the substance of any license notices
-(including copyright notices, patent notices, disclaimers of warranty,
-or limitations of liability) contained within the Source Code Form of
-the Covered Software, except that You may alter any license notices to
-the extent required to remedy known factual inaccuracies.
-
-3.5. Application of Additional Terms
-
-You may choose to offer, and to charge a fee for, warranty, support,
-indemnity or liability obligations to one or more recipients of Covered
-Software. However, You may do so only on Your own behalf, and not on
-behalf of any Contributor. You must make it absolutely clear that any
-such warranty, support, indemnity, or liability obligation is offered by
-You alone, and You hereby agree to indemnify every Contributor for any
-liability incurred by such Contributor as a result of warranty, support,
-indemnity or liability terms You offer. You may include additional
-disclaimers of warranty and limitations of liability specific to any
-jurisdiction.
-
-4. Inability to Comply Due to Statute or Regulation
----------------------------------------------------
-
-If it is impossible for You to comply with any of the terms of this
-License with respect to some or all of the Covered Software due to
-statute, judicial order, or regulation then You must: (a) comply with
-the terms of this License to the maximum extent possible; and (b)
-describe the limitations and the code they affect. Such description must
-be placed in a text file included with all distributions of the Covered
-Software under this License. Except to the extent prohibited by statute
-or regulation, such description must be sufficiently detailed for a
-recipient of ordinary skill to be able to understand it.
-
-5. Termination
---------------
-
-5.1. The rights granted under this License will terminate automatically
-if You fail to comply with any of its terms. However, if You become
-compliant, then the rights granted under this License from a particular
-Contributor are reinstated (a) provisionally, unless and until such
-Contributor explicitly and finally terminates Your grants, and (b) on an
-ongoing basis, if such Contributor fails to notify You of the
-non-compliance by some reasonable means prior to 60 days after You have
-come back into compliance. Moreover, Your grants from a particular
-Contributor are reinstated on an ongoing basis if such Contributor
-notifies You of the non-compliance by some reasonable means, this is the
-first time You have received notice of non-compliance with this License
-from such Contributor, and You become compliant prior to 30 days after
-Your receipt of the notice.
-
-5.2. If You initiate litigation against any entity by asserting a patent
-infringement claim (excluding declaratory judgment actions,
-counter-claims, and cross-claims) alleging that a Contributor Version
-directly or indirectly infringes any patent, then the rights granted to
-You by any and all Contributors for the Covered Software under Section
-2.1 of this License shall terminate.
-
-5.3. In the event of termination under Sections 5.1 or 5.2 above, all
-end user license agreements (excluding distributors and resellers) which
-have been validly granted by You or Your distributors under this License
-prior to termination shall survive termination.
-
-************************************************************************
-*                                                                      *
-*  6. Disclaimer of Warranty                                           *
-*  -------------------------                                           *
-*                                                                      *
-*  Covered Software is provided under this License on an "as is"       *
-*  basis, without warranty of any kind, either expressed, implied, or  *
-*  statutory, including, without limitation, warranties that the       *
-*  Covered Software is free of defects, merchantable, fit for a        *
-*  particular purpose or non-infringing. The entire risk as to the     *
-*  quality and performance of the Covered Software is with You.        *
-*  Should any Covered Software prove defective in any respect, You     *
-*  (not any Contributor) assume the cost of any necessary servicing,   *
-*  repair, or correction. This disclaimer of warranty constitutes an   *
-*  essential part of this License. No use of any Covered Software is   *
-*  authorized under this License except under this disclaimer.         *
-*                                                                      *
-************************************************************************
-
-************************************************************************
-*                                                                      *
-*  7. Limitation of Liability                                          *
-*  --------------------------                                          *
-*                                                                      *
-*  Under no circumstances and under no legal theory, whether tort      *
-*  (including negligence), contract, or otherwise, shall any           *
-*  Contributor, or anyone who distributes Covered Software as          *
-*  permitted above, be liable to You for any direct, indirect,         *
-*  special, incidental, or consequential damages of any character      *
-*  including, without limitation, damages for lost profits, loss of    *
-*  goodwill, work stoppage, computer failure or malfunction, or any    *
-*  and all other commercial damages or losses, even if such party      *
-*  shall have been informed of the possibility of such damages. This   *
-*  limitation of liability shall not apply to liability for death or   *
-*  personal injury resulting from such party's negligence to the       *
-*  extent applicable law prohibits such limitation. Some               *
-*  jurisdictions do not allow the exclusion or limitation of           *
-*  incidental or consequential damages, so this exclusion and          *
-*  limitation may not apply to You.                                    *
-*                                                                      *
-************************************************************************
-
-8. Litigation
--------------
-
-Any litigation relating to this License may be brought only in the
-courts of a jurisdiction where the defendant maintains its principal
-place of business and such litigation shall be governed by laws of that
-jurisdiction, without reference to its conflict-of-law provisions.
-Nothing in this Section shall prevent a party's ability to bring
-cross-claims or counter-claims.
-
-9. Miscellaneous
-----------------
-
-This License represents the complete agreement concerning the subject
-matter hereof. If any provision of this License is held to be
-unenforceable, such provision shall be reformed only to the extent
-necessary to make it enforceable. Any law or regulation which provides
-that the language of a contract shall be construed against the drafter
-shall not be used to construe this License against a Contributor.
-
-10. Versions of the License
----------------------------
-
-10.1. New Versions
-
-Mozilla Foundation is the license steward. Except as provided in Section
-10.3, no one other than the license steward has the right to modify or
-publish new versions of this License. Each version will be given a
-distinguishing version number.
-
-10.2. Effect of New Versions
-
-You may distribute the Covered Software under the terms of the version
-of the License under which You originally received the Covered Software,
-or under the terms of any subsequent version published by the license
-steward.
-
-10.3. Modified Versions
-
-If you create software not governed by this License, and you want to
-create a new license for such software, you may create and use a
-modified version of this License if you rename the license and remove
-any references to the name of the license steward (except to note that
-such modified license differs from this License).
-
-10.4. Distributing Source Code Form that is Incompatible With Secondary
-Licenses
-
-If You choose to distribute Source Code Form that is Incompatible With
-Secondary Licenses under the terms of this version of the License, the
-notice described in Exhibit B of this License must be attached.
-
-Exhibit A - Source Code Form License Notice
--------------------------------------------
-
-  This Source Code Form is subject to the terms of the Mozilla Public
-  License, v. 2.0. If a copy of the MPL was not distributed with this
-  file, You can obtain one at http://mozilla.org/MPL/2.0/.
-
-If it is not possible or desirable to put the notice in a particular
-file, then You may include the notice in a location (such as a LICENSE
-file in a relevant directory) where a recipient would be likely to look
-for such a notice.
-
-You may add additional accurate notices of copyright ownership.
-
-Exhibit B - "Incompatible With Secondary Licenses" Notice
----------------------------------------------------------
-
-  This Source Code Form is "Incompatible With Secondary Licenses", as
+Mozilla Public License Version 2.0
+==================================
+
+1. Definitions
+--------------
+
+1.1. "Contributor"
+    means each individual or legal entity that creates, contributes to
+    the creation of, or owns Covered Software.
+
+1.2. "Contributor Version"
+    means the combination of the Contributions of others (if any) used
+    by a Contributor and that particular Contributor's Contribution.
+
+1.3. "Contribution"
+    means Covered Software of a particular Contributor.
+
+1.4. "Covered Software"
+    means Source Code Form to which the initial Contributor has attached
+    the notice in Exhibit A, the Executable Form of such Source Code
+    Form, and Modifications of such Source Code Form, in each case
+    including portions thereof.
+
+1.5. "Incompatible With Secondary Licenses"
+    means
+
+    (a) that the initial Contributor has attached the notice described
+        in Exhibit B to the Covered Software; or
+
+    (b) that the Covered Software was made available under the terms of
+        version 1.1 or earlier of the License, but not also under the
+        terms of a Secondary License.
+
+1.6. "Executable Form"
+    means any form of the work other than Source Code Form.
+
+1.7. "Larger Work"
+    means a work that combines Covered Software with other material, in 
+    a separate file or files, that is not Covered Software.
+
+1.8. "License"
+    means this document.
+
+1.9. "Licensable"
+    means having the right to grant, to the maximum extent possible,
+    whether at the time of the initial grant or subsequently, any and
+    all of the rights conveyed by this License.
+
+1.10. "Modifications"
+    means any of the following:
+
+    (a) any file in Source Code Form that results from an addition to,
+        deletion from, or modification of the contents of Covered
+        Software; or
+
+    (b) any new file in Source Code Form that contains any Covered
+        Software.
+
+1.11. "Patent Claims" of a Contributor
+    means any patent claim(s), including without limitation, method,
+    process, and apparatus claims, in any patent Licensable by such
+    Contributor that would be infringed, but for the grant of the
+    License, by the making, using, selling, offering for sale, having
+    made, import, or transfer of either its Contributions or its
+    Contributor Version.
+
+1.12. "Secondary License"
+    means either the GNU General Public License, Version 2.0, the GNU
+    Lesser General Public License, Version 2.1, the GNU Affero General
+    Public License, Version 3.0, or any later versions of those
+    licenses.
+
+1.13. "Source Code Form"
+    means the form of the work preferred for making modifications.
+
+1.14. "You" (or "Your")
+    means an individual or a legal entity exercising rights under this
+    License. For legal entities, "You" includes any entity that
+    controls, is controlled by, or is under common control with You. For
+    purposes of this definition, "control" means (a) the power, direct
+    or indirect, to cause the direction or management of such entity,
+    whether by contract or otherwise, or (b) ownership of more than
+    fifty percent (50%) of the outstanding shares or beneficial
+    ownership of such entity.
+
+2. License Grants and Conditions
+--------------------------------
+
+2.1. Grants
+
+Each Contributor hereby grants You a world-wide, royalty-free,
+non-exclusive license:
+
+(a) under intellectual property rights (other than patent or trademark)
+    Licensable by such Contributor to use, reproduce, make available,
+    modify, display, perform, distribute, and otherwise exploit its
+    Contributions, either on an unmodified basis, with Modifications, or
+    as part of a Larger Work; and
+
+(b) under Patent Claims of such Contributor to make, use, sell, offer
+    for sale, have made, import, and otherwise transfer either its
+    Contributions or its Contributor Version.
+
+2.2. Effective Date
+
+The licenses granted in Section 2.1 with respect to any Contribution
+become effective for each Contribution on the date the Contributor first
+distributes such Contribution.
+
+2.3. Limitations on Grant Scope
+
+The licenses granted in this Section 2 are the only rights granted under
+this License. No additional rights or licenses will be implied from the
+distribution or licensing of Covered Software under this License.
+Notwithstanding Section 2.1(b) above, no patent license is granted by a
+Contributor:
+
+(a) for any code that a Contributor has removed from Covered Software;
+    or
+
+(b) for infringements caused by: (i) Your and any other third party's
+    modifications of Covered Software, or (ii) the combination of its
+    Contributions with other software (except as part of its Contributor
+    Version); or
+
+(c) under Patent Claims infringed by Covered Software in the absence of
+    its Contributions.
+
+This License does not grant any rights in the trademarks, service marks,
+or logos of any Contributor (except as may be necessary to comply with
+the notice requirements in Section 3.4).
+
+2.4. Subsequent Licenses
+
+No Contributor makes additional grants as a result of Your choice to
+distribute the Covered Software under a subsequent version of this
+License (see Section 10.2) or under the terms of a Secondary License (if
+permitted under the terms of Section 3.3).
+
+2.5. Representation
+
+Each Contributor represents that the Contributor believes its
+Contributions are its original creation(s) or it has sufficient rights
+to grant the rights to its Contributions conveyed by this License.
+
+2.6. Fair Use
+
+This License is not intended to limit any rights You have under
+applicable copyright doctrines of fair use, fair dealing, or other
+equivalents.
+
+2.7. Conditions
+
+Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
+in Section 2.1.
+
+3. Responsibilities
+-------------------
+
+3.1. Distribution of Source Form
+
+All distribution of Covered Software in Source Code Form, including any
+Modifications that You create or to which You contribute, must be under
+the terms of this License. You must inform recipients that the Source
+Code Form of the Covered Software is governed by the terms of this
+License, and how they can obtain a copy of this License. You may not
+attempt to alter or restrict the recipients' rights in the Source Code
+Form.
+
+3.2. Distribution of Executable Form
+
+If You distribute Covered Software in Executable Form then:
+
+(a) such Covered Software must also be made available in Source Code
+    Form, as described in Section 3.1, and You must inform recipients of
+    the Executable Form how they can obtain a copy of such Source Code
+    Form by reasonable means in a timely manner, at a charge no more
+    than the cost of distribution to the recipient; and
+
+(b) You may distribute such Executable Form under the terms of this
+    License, or sublicense it under different terms, provided that the
+    license for the Executable Form does not attempt to limit or alter
+    the recipients' rights in the Source Code Form under this License.
+
+3.3. Distribution of a Larger Work
+
+You may create and distribute a Larger Work under terms of Your choice,
+provided that You also comply with the requirements of this License for
+the Covered Software. If the Larger Work is a combination of Covered
+Software with a work governed by one or more Secondary Licenses, and the
+Covered Software is not Incompatible With Secondary Licenses, this
+License permits You to additionally distribute such Covered Software
+under the terms of such Secondary License(s), so that the recipient of
+the Larger Work may, at their option, further distribute the Covered
+Software under the terms of either this License or such Secondary
+License(s).
+
+3.4. Notices
+
+You may not remove or alter the substance of any license notices
+(including copyright notices, patent notices, disclaimers of warranty,
+or limitations of liability) contained within the Source Code Form of
+the Covered Software, except that You may alter any license notices to
+the extent required to remedy known factual inaccuracies.
+
+3.5. Application of Additional Terms
+
+You may choose to offer, and to charge a fee for, warranty, support,
+indemnity or liability obligations to one or more recipients of Covered
+Software. However, You may do so only on Your own behalf, and not on
+behalf of any Contributor. You must make it absolutely clear that any
+such warranty, support, indemnity, or liability obligation is offered by
+You alone, and You hereby agree to indemnify every Contributor for any
+liability incurred by such Contributor as a result of warranty, support,
+indemnity or liability terms You offer. You may include additional
+disclaimers of warranty and limitations of liability specific to any
+jurisdiction.
+
+4. Inability to Comply Due to Statute or Regulation
+---------------------------------------------------
+
+If it is impossible for You to comply with any of the terms of this
+License with respect to some or all of the Covered Software due to
+statute, judicial order, or regulation then You must: (a) comply with
+the terms of this License to the maximum extent possible; and (b)
+describe the limitations and the code they affect. Such description must
+be placed in a text file included with all distributions of the Covered
+Software under this License. Except to the extent prohibited by statute
+or regulation, such description must be sufficiently detailed for a
+recipient of ordinary skill to be able to understand it.
+
+5. Termination
+--------------
+
+5.1. The rights granted under this License will terminate automatically
+if You fail to comply with any of its terms. However, if You become
+compliant, then the rights granted under this License from a particular
+Contributor are reinstated (a) provisionally, unless and until such
+Contributor explicitly and finally terminates Your grants, and (b) on an
+ongoing basis, if such Contributor fails to notify You of the
+non-compliance by some reasonable means prior to 60 days after You have
+come back into compliance. Moreover, Your grants from a particular
+Contributor are reinstated on an ongoing basis if such Contributor
+notifies You of the non-compliance by some reasonable means, this is the
+first time You have received notice of non-compliance with this License
+from such Contributor, and You become compliant prior to 30 days after
+Your receipt of the notice.
+
+5.2. If You initiate litigation against any entity by asserting a patent
+infringement claim (excluding declaratory judgment actions,
+counter-claims, and cross-claims) alleging that a Contributor Version
+directly or indirectly infringes any patent, then the rights granted to
+You by any and all Contributors for the Covered Software under Section
+2.1 of this License shall terminate.
+
+5.3. In the event of termination under Sections 5.1 or 5.2 above, all
+end user license agreements (excluding distributors and resellers) which
+have been validly granted by You or Your distributors under this License
+prior to termination shall survive termination.
+
+************************************************************************
+*                                                                      *
+*  6. Disclaimer of Warranty                                           *
+*  -------------------------                                           *
+*                                                                      *
+*  Covered Software is provided under this License on an "as is"       *
+*  basis, without warranty of any kind, either expressed, implied, or  *
+*  statutory, including, without limitation, warranties that the       *
+*  Covered Software is free of defects, merchantable, fit for a        *
+*  particular purpose or non-infringing. The entire risk as to the     *
+*  quality and performance of the Covered Software is with You.        *
+*  Should any Covered Software prove defective in any respect, You     *
+*  (not any Contributor) assume the cost of any necessary servicing,   *
+*  repair, or correction. This disclaimer of warranty constitutes an   *
+*  essential part of this License. No use of any Covered Software is   *
+*  authorized under this License except under this disclaimer.         *
+*                                                                      *
+************************************************************************
+
+************************************************************************
+*                                                                      *
+*  7. Limitation of Liability                                          *
+*  --------------------------                                          *
+*                                                                      *
+*  Under no circumstances and under no legal theory, whether tort      *
+*  (including negligence), contract, or otherwise, shall any           *
+*  Contributor, or anyone who distributes Covered Software as          *
+*  permitted above, be liable to You for any direct, indirect,         *
+*  special, incidental, or consequential damages of any character      *
+*  including, without limitation, damages for lost profits, loss of    *
+*  goodwill, work stoppage, computer failure or malfunction, or any    *
+*  and all other commercial damages or losses, even if such party      *
+*  shall have been informed of the possibility of such damages. This   *
+*  limitation of liability shall not apply to liability for death or   *
+*  personal injury resulting from such party's negligence to the       *
+*  extent applicable law prohibits such limitation. Some               *
+*  jurisdictions do not allow the exclusion or limitation of           *
+*  incidental or consequential damages, so this exclusion and          *
+*  limitation may not apply to You.                                    *
+*                                                                      *
+************************************************************************
+
+8. Litigation
+-------------
+
+Any litigation relating to this License may be brought only in the
+courts of a jurisdiction where the defendant maintains its principal
+place of business and such litigation shall be governed by laws of that
+jurisdiction, without reference to its conflict-of-law provisions.
+Nothing in this Section shall prevent a party's ability to bring
+cross-claims or counter-claims.
+
+9. Miscellaneous
+----------------
+
+This License represents the complete agreement concerning the subject
+matter hereof. If any provision of this License is held to be
+unenforceable, such provision shall be reformed only to the extent
+necessary to make it enforceable. Any law or regulation which provides
+that the language of a contract shall be construed against the drafter
+shall not be used to construe this License against a Contributor.
+
+10. Versions of the License
+---------------------------
+
+10.1. New Versions
+
+Mozilla Foundation is the license steward. Except as provided in Section
+10.3, no one other than the license steward has the right to modify or
+publish new versions of this License. Each version will be given a
+distinguishing version number.
+
+10.2. Effect of New Versions
+
+You may distribute the Covered Software under the terms of the version
+of the License under which You originally received the Covered Software,
+or under the terms of any subsequent version published by the license
+steward.
+
+10.3. Modified Versions
+
+If you create software not governed by this License, and you want to
+create a new license for such software, you may create and use a
+modified version of this License if you rename the license and remove
+any references to the name of the license steward (except to note that
+such modified license differs from this License).
+
+10.4. Distributing Source Code Form that is Incompatible With Secondary
+Licenses
+
+If You choose to distribute Source Code Form that is Incompatible With
+Secondary Licenses under the terms of this version of the License, the
+notice described in Exhibit B of this License must be attached.
+
+Exhibit A - Source Code Form License Notice
+-------------------------------------------
+
+  This Source Code Form is subject to the terms of the Mozilla Public
+  License, v. 2.0. If a copy of the MPL was not distributed with this
+  file, You can obtain one at http://mozilla.org/MPL/2.0/.
+
+If it is not possible or desirable to put the notice in a particular
+file, then You may include the notice in a location (such as a LICENSE
+file in a relevant directory) where a recipient would be likely to look
+for such a notice.
+
+You may add additional accurate notices of copyright ownership.
+
+Exhibit B - "Incompatible With Secondary Licenses" Notice
+---------------------------------------------------------
+
+  This Source Code Form is "Incompatible With Secondary Licenses", as
   defined by the Mozilla Public License, v. 2.0.
```

### Comparing `VUnit-helpers-0.1.0/PKG-INFO` & `VUnit-helpers-2023.5.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,107 +1,119 @@
-Metadata-Version: 2.1
-Name: VUnit-helpers
-Version: 0.1.0
-Summary: Common tools and helpers to simplify the VUnit run scripts
-Author-email: Markus Leiter <leiter@p2l2.com>
-Project-URL: Homepage, https://github.com/p2l2/VUnit-helpers
-Project-URL: Bug Tracker, https://github.com/p2l2/VUnit-helpers/issues
-Keywords: VUnit,unit testing
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# VUnit-helpers
-
-This package contains project independent tools and helpers to simplify VUnit run scripts.
-Using this, the run script gets shorter, more readable and easier to maintain. 
-
-# Usage Examples
-
-
-## Get the root path of a git repository
-Working with relative paths in VUnit is dangerouse, since it depends on the working directory of python during execution. Instead, you can use your git repository as the root reference of all paths.
-``` Python
-import vunit_helpers
-git_repo_path = vunit_helpers.get_git_repo_root_path()
-```
-
-## Add UVVM to VUnit
-
-Use vunit_helpers.add_uvvm_sources() to add all UVVM source files to VUnit. VUnit will compile UVVM in the correct order.  
-
-``` Python
-from vunit import VUnit
-import vunit_helpers
-
-VU = VUnit.from_argv()
-# add all UVVM components
-vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM")
-
-# add some specific UVVM components only
-vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM", ["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"])
-```
-
-If you have precompiled UVVM using its compile_all.do TCL script, you can use vunit_helpers.add_precompiled_uvvm_libraries():
-``` Python
-VU = VUnit.from_argv()
-vunit_helpers.add_precompiled_uvvm_libraries(VU,["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"],"path/to/UVVM")
-```
-
-## Advanced add Source Files
-Vunit helpers allows including and excluding wildcard patterns. That way, it's easier to exclude specific files from VUnit. 
-``` Python
-from vunit import VUnit
-import vunit_helpers
-from vunit_helpers import File_pattern
-
-VU = VUnit.from_argv()
-lib = VU.add_library("lib") 
-
-include_patterns=[
-    File_pattern(git_repo_path  / "verification"/ "*" / "hdl" / "*.vhd"),
-    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "*.vhd"),
-]
-
-# The files that match the exclude patterns won't be added to the lib (these files are excluded from the include_patterns)
-exclude_patterns=[
-    # the SPI testbench uses external_names, that are not supported in GHDL yet
-    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "tb_Formal.vhd", when_simulator_is_not="ghdl"),
-    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "AnyFileIDontWant.vhd),
-    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "VerificationDefinitions-p.vhd", when_simulator_is="modelsim") 
-]
-vunit_helpers.advanced_add_source_files(VU,lib,include_patterns,exclude_patterns)
-```
-
-## UVVM with GHDL
-To run UVVM with GHDL, some additional compile and sim flags must be set. 
-``` Python
-VU = VUnit.from_argv()
-vunit_helpers.set_ghdl_flags_for_UVVM(VU)
-```
-
-## TOML File for RustHDL
-RustHDL is a free and open source VHDL language server. It's setup requires a TOML file, that lists all libraries and source files of a project. The fuction generate_rust_hdl_toml() will generate the TOML file for RustHDL based on all files that are included in the VUnit project. 
-Call this function after adding the files to VUnit. 
-
-``` Python
-VU = VUnit.from_argv()
-vunit_helpers.add_uvvm_sources(VU, "path/to/UVVM")
-
-vunit_helpers.generate_rust_hdl_toml(VU, str(git_repo_path / "vhdl_ls.toml"), str(git_repo_path))
-```
-
-
-
+Metadata-Version: 2.1
+Name: VUnit-helpers
+Version: 2023.5.7
+Summary: Common tools and helpers to simplify the VUnit run scripts
+Author-email: Markus Leiter <leiter@p2l2.com>
+Project-URL: Homepage, https://github.com/p2l2/VUnit-helpers
+Project-URL: Bug Tracker, https://github.com/p2l2/VUnit-helpers/issues
+Keywords: VUnit,unit testing
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# VUnit-helpers
+
+This package contains project independent tools and helpers to simplify VUnit run scripts.
+Using this, the run script gets shorter, more readable and easier to maintain. 
+
+# Installing VUnit_helpers
+You can install this package from source or via PyPi
+
+## Installing via PyPi
+
+    python -m pip install vunit_helpers
+
+## Installing from source:
+1. Clone or download the repository
+2. navigate to the directory and run ```python -m pip install .```
+
+Optionally add the ```-e``` flag to install the package in the editable mode.
+
+# Usage Examples
+
+## Get the root path of a git repository
+Working with relative paths in VUnit is dangerouse, since it depends on the working directory of python during execution. Instead, you can use your git repository as the root reference of all paths.
+``` Python
+import vunit_helpers
+git_repo_path = vunit_helpers.get_git_repo_root_path()
+```
+
+## Add UVVM to VUnit
+
+Use vunit_helpers.add_uvvm_sources() to add all UVVM source files to VUnit. VUnit will compile UVVM in the correct order.  
+
+``` Python
+from vunit import VUnit
+import vunit_helpers
+
+VU = VUnit.from_argv()
+# add all UVVM components
+vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM")
+
+# add some specific UVVM components only
+vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM", ["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"])
+```
+
+If you have precompiled UVVM using its compile_all.do TCL script, you can use vunit_helpers.add_precompiled_uvvm_libraries():
+``` Python
+VU = VUnit.from_argv()
+vunit_helpers.add_precompiled_uvvm_libraries(VU,["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"],"path/to/UVVM")
+```
+
+## Advanced add Source Files
+Vunit helpers allows including and excluding wildcard patterns. That way, it's easier to exclude specific files from VUnit. 
+``` Python
+from vunit import VUnit
+import vunit_helpers
+from vunit_helpers import File_pattern
+
+VU = VUnit.from_argv()
+lib = VU.add_library("lib") 
+
+include_patterns=[
+    File_pattern(git_repo_path  / "verification"/ "*" / "hdl" / "*.vhd"),
+    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "*.vhd"),
+]
+
+# The files that match the exclude patterns won't be added to the lib (these files are excluded from the include_patterns)
+exclude_patterns=[
+    # the SPI testbench uses external_names, that are not supported in GHDL yet
+    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "tb_Formal.vhd", when_simulator_is_not="ghdl"),
+    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "AnyFileIDontWant.vhd),
+    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "VerificationDefinitions-p.vhd", when_simulator_is="modelsim") 
+]
+vunit_helpers.advanced_add_source_files(VU,lib,include_patterns,exclude_patterns)
+```
+
+## UVVM with GHDL
+To run UVVM with GHDL, some additional compile and sim flags must be set. 
+``` Python
+VU = VUnit.from_argv()
+vunit_helpers.set_ghdl_flags_for_UVVM(VU)
+```
+
+## TOML File for RustHDL
+RustHDL is a free and open source VHDL language server. It's setup requires a TOML file, that lists all libraries and source files of a project. The fuction generate_rust_hdl_toml() will generate the TOML file for RustHDL based on all files that are included in the VUnit project. 
+Call this function after adding the files to VUnit. 
+
+``` Python
+VU = VUnit.from_argv()
+vunit_helpers.add_uvvm_sources(VU, "path/to/UVVM")
+
+vunit_helpers.generate_rust_hdl_toml(VU, str(git_repo_path / "vhdl_ls.toml"), str(git_repo_path))
+```
+
+
+
```

### Comparing `VUnit-helpers-0.1.0/README.md` & `VUnit-helpers-2023.5.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,94 @@
-# VUnit-helpers
-
-This package contains project independent tools and helpers to simplify VUnit run scripts.
-Using this, the run script gets shorter, more readable and easier to maintain. 
-
-# Usage Examples
-
-
-## Get the root path of a git repository
-Working with relative paths in VUnit is dangerouse, since it depends on the working directory of python during execution. Instead, you can use your git repository as the root reference of all paths.
-``` Python
-import vunit_helpers
-git_repo_path = vunit_helpers.get_git_repo_root_path()
-```
-
-## Add UVVM to VUnit
-
-Use vunit_helpers.add_uvvm_sources() to add all UVVM source files to VUnit. VUnit will compile UVVM in the correct order.  
-
-``` Python
-from vunit import VUnit
-import vunit_helpers
-
-VU = VUnit.from_argv()
-# add all UVVM components
-vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM")
-
-# add some specific UVVM components only
-vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM", ["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"])
-```
-
-If you have precompiled UVVM using its compile_all.do TCL script, you can use vunit_helpers.add_precompiled_uvvm_libraries():
-``` Python
-VU = VUnit.from_argv()
-vunit_helpers.add_precompiled_uvvm_libraries(VU,["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"],"path/to/UVVM")
-```
-
-## Advanced add Source Files
-Vunit helpers allows including and excluding wildcard patterns. That way, it's easier to exclude specific files from VUnit. 
-``` Python
-from vunit import VUnit
-import vunit_helpers
-from vunit_helpers import File_pattern
-
-VU = VUnit.from_argv()
-lib = VU.add_library("lib") 
-
-include_patterns=[
-    File_pattern(git_repo_path  / "verification"/ "*" / "hdl" / "*.vhd"),
-    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "*.vhd"),
-]
-
-# The files that match the exclude patterns won't be added to the lib (these files are excluded from the include_patterns)
-exclude_patterns=[
-    # the SPI testbench uses external_names, that are not supported in GHDL yet
-    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "tb_Formal.vhd", when_simulator_is_not="ghdl"),
-    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "AnyFileIDontWant.vhd),
-    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "VerificationDefinitions-p.vhd", when_simulator_is="modelsim") 
-]
-vunit_helpers.advanced_add_source_files(VU,lib,include_patterns,exclude_patterns)
-```
-
-## UVVM with GHDL
-To run UVVM with GHDL, some additional compile and sim flags must be set. 
-``` Python
-VU = VUnit.from_argv()
-vunit_helpers.set_ghdl_flags_for_UVVM(VU)
-```
-
-## TOML File for RustHDL
-RustHDL is a free and open source VHDL language server. It's setup requires a TOML file, that lists all libraries and source files of a project. The fuction generate_rust_hdl_toml() will generate the TOML file for RustHDL based on all files that are included in the VUnit project. 
-Call this function after adding the files to VUnit. 
-
-``` Python
-VU = VUnit.from_argv()
-vunit_helpers.add_uvvm_sources(VU, "path/to/UVVM")
-
-vunit_helpers.generate_rust_hdl_toml(VU, str(git_repo_path / "vhdl_ls.toml"), str(git_repo_path))
-```
-
-
-
+# VUnit-helpers
+
+This package contains project independent tools and helpers to simplify VUnit run scripts.
+Using this, the run script gets shorter, more readable and easier to maintain. 
+
+# Installing VUnit_helpers
+You can install this package from source or via PyPi
+
+## Installing via PyPi
+
+    python -m pip install vunit_helpers
+
+## Installing from source:
+1. Clone or download the repository
+2. navigate to the directory and run ```python -m pip install .```
+
+Optionally add the ```-e``` flag to install the package in the editable mode.
+
+# Usage Examples
+
+## Get the root path of a git repository
+Working with relative paths in VUnit is dangerouse, since it depends on the working directory of python during execution. Instead, you can use your git repository as the root reference of all paths.
+``` Python
+import vunit_helpers
+git_repo_path = vunit_helpers.get_git_repo_root_path()
+```
+
+## Add UVVM to VUnit
+
+Use vunit_helpers.add_uvvm_sources() to add all UVVM source files to VUnit. VUnit will compile UVVM in the correct order.  
+
+``` Python
+from vunit import VUnit
+import vunit_helpers
+
+VU = VUnit.from_argv()
+# add all UVVM components
+vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM")
+
+# add some specific UVVM components only
+vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM", ["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"])
+```
+
+If you have precompiled UVVM using its compile_all.do TCL script, you can use vunit_helpers.add_precompiled_uvvm_libraries():
+``` Python
+VU = VUnit.from_argv()
+vunit_helpers.add_precompiled_uvvm_libraries(VU,["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"],"path/to/UVVM")
+```
+
+## Advanced add Source Files
+Vunit helpers allows including and excluding wildcard patterns. That way, it's easier to exclude specific files from VUnit. 
+``` Python
+from vunit import VUnit
+import vunit_helpers
+from vunit_helpers import File_pattern
+
+VU = VUnit.from_argv()
+lib = VU.add_library("lib") 
+
+include_patterns=[
+    File_pattern(git_repo_path  / "verification"/ "*" / "hdl" / "*.vhd"),
+    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "*.vhd"),
+]
+
+# The files that match the exclude patterns won't be added to the lib (these files are excluded from the include_patterns)
+exclude_patterns=[
+    # the SPI testbench uses external_names, that are not supported in GHDL yet
+    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "tb_Formal.vhd", when_simulator_is_not="ghdl"),
+    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "AnyFileIDontWant.vhd),
+    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "VerificationDefinitions-p.vhd", when_simulator_is="modelsim") 
+]
+vunit_helpers.advanced_add_source_files(VU,lib,include_patterns,exclude_patterns)
+```
+
+## UVVM with GHDL
+To run UVVM with GHDL, some additional compile and sim flags must be set. 
+``` Python
+VU = VUnit.from_argv()
+vunit_helpers.set_ghdl_flags_for_UVVM(VU)
+```
+
+## TOML File for RustHDL
+RustHDL is a free and open source VHDL language server. It's setup requires a TOML file, that lists all libraries and source files of a project. The fuction generate_rust_hdl_toml() will generate the TOML file for RustHDL based on all files that are included in the VUnit project. 
+Call this function after adding the files to VUnit. 
+
+``` Python
+VU = VUnit.from_argv()
+vunit_helpers.add_uvvm_sources(VU, "path/to/UVVM")
+
+vunit_helpers.generate_rust_hdl_toml(VU, str(git_repo_path / "vhdl_ls.toml"), str(git_repo_path))
+```
+
+
+
```

### Comparing `VUnit-helpers-0.1.0/pyproject.toml` & `VUnit-helpers-2023.5.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-[build-system]
-requires = ["setuptools>=61.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-
-[project]
-version = "0.1.0"
-name = "VUnit-helpers"
-description = "Common tools and helpers to simplify the VUnit run scripts"
-authors = [
-  { name="Markus Leiter", email="leiter@p2l2.com" },
-]
-license = {file="LICENCE"}
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
-    "Natural Language :: English",
-    "Intended Audience :: Developers",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: MacOS :: MacOS X",
-    "Operating System :: POSIX :: Linux",
-    "Topic :: Software Development :: Testing",
-    "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
-]
-keywords = ["VUnit", "unit testing"]
-dependencies = [
-    "pathlib",
-    "logging",
-    "glob2",
-    "typing",
-    "toml>=0.10.2"
-]
-
-[project.urls]
-"Homepage" = "https://github.com/p2l2/VUnit-helpers"
-"Bug Tracker" = "https://github.com/p2l2/VUnit-helpers/issues"
+[build-system]
+requires = ["setuptools>=61.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+
+[project]
+version = "2023.5.7"
+name = "VUnit-helpers"
+description = "Common tools and helpers to simplify the VUnit run scripts"
+authors = [
+  { name="Markus Leiter", email="leiter@p2l2.com" },
+]
+license = {file="LICENCE"}
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
+    "Natural Language :: English",
+    "Intended Audience :: Developers",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: POSIX :: Linux",
+    "Topic :: Software Development :: Testing",
+    "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
+]
+keywords = ["VUnit", "unit testing"]
+dependencies = [
+    "pathlib",
+    "logging",
+    "glob2",
+    "typing",
+    "toml>=0.10.2"
+]
+
+[project.urls]
+"Homepage" = "https://github.com/p2l2/VUnit-helpers"
+"Bug Tracker" = "https://github.com/p2l2/VUnit-helpers/issues"
```

### Comparing `VUnit-helpers-0.1.0/src/VUnit_helpers.egg-info/PKG-INFO` & `VUnit-helpers-2023.5.7/src/VUnit_helpers.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,107 +1,119 @@
-Metadata-Version: 2.1
-Name: VUnit-helpers
-Version: 0.1.0
-Summary: Common tools and helpers to simplify the VUnit run scripts
-Author-email: Markus Leiter <leiter@p2l2.com>
-Project-URL: Homepage, https://github.com/p2l2/VUnit-helpers
-Project-URL: Bug Tracker, https://github.com/p2l2/VUnit-helpers/issues
-Keywords: VUnit,unit testing
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# VUnit-helpers
-
-This package contains project independent tools and helpers to simplify VUnit run scripts.
-Using this, the run script gets shorter, more readable and easier to maintain. 
-
-# Usage Examples
-
-
-## Get the root path of a git repository
-Working with relative paths in VUnit is dangerouse, since it depends on the working directory of python during execution. Instead, you can use your git repository as the root reference of all paths.
-``` Python
-import vunit_helpers
-git_repo_path = vunit_helpers.get_git_repo_root_path()
-```
-
-## Add UVVM to VUnit
-
-Use vunit_helpers.add_uvvm_sources() to add all UVVM source files to VUnit. VUnit will compile UVVM in the correct order.  
-
-``` Python
-from vunit import VUnit
-import vunit_helpers
-
-VU = VUnit.from_argv()
-# add all UVVM components
-vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM")
-
-# add some specific UVVM components only
-vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM", ["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"])
-```
-
-If you have precompiled UVVM using its compile_all.do TCL script, you can use vunit_helpers.add_precompiled_uvvm_libraries():
-``` Python
-VU = VUnit.from_argv()
-vunit_helpers.add_precompiled_uvvm_libraries(VU,["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"],"path/to/UVVM")
-```
-
-## Advanced add Source Files
-Vunit helpers allows including and excluding wildcard patterns. That way, it's easier to exclude specific files from VUnit. 
-``` Python
-from vunit import VUnit
-import vunit_helpers
-from vunit_helpers import File_pattern
-
-VU = VUnit.from_argv()
-lib = VU.add_library("lib") 
-
-include_patterns=[
-    File_pattern(git_repo_path  / "verification"/ "*" / "hdl" / "*.vhd"),
-    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "*.vhd"),
-]
-
-# The files that match the exclude patterns won't be added to the lib (these files are excluded from the include_patterns)
-exclude_patterns=[
-    # the SPI testbench uses external_names, that are not supported in GHDL yet
-    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "tb_Formal.vhd", when_simulator_is_not="ghdl"),
-    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "AnyFileIDontWant.vhd),
-    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "VerificationDefinitions-p.vhd", when_simulator_is="modelsim") 
-]
-vunit_helpers.advanced_add_source_files(VU,lib,include_patterns,exclude_patterns)
-```
-
-## UVVM with GHDL
-To run UVVM with GHDL, some additional compile and sim flags must be set. 
-``` Python
-VU = VUnit.from_argv()
-vunit_helpers.set_ghdl_flags_for_UVVM(VU)
-```
-
-## TOML File for RustHDL
-RustHDL is a free and open source VHDL language server. It's setup requires a TOML file, that lists all libraries and source files of a project. The fuction generate_rust_hdl_toml() will generate the TOML file for RustHDL based on all files that are included in the VUnit project. 
-Call this function after adding the files to VUnit. 
-
-``` Python
-VU = VUnit.from_argv()
-vunit_helpers.add_uvvm_sources(VU, "path/to/UVVM")
-
-vunit_helpers.generate_rust_hdl_toml(VU, str(git_repo_path / "vhdl_ls.toml"), str(git_repo_path))
-```
-
-
-
+Metadata-Version: 2.1
+Name: VUnit-helpers
+Version: 2023.5.7
+Summary: Common tools and helpers to simplify the VUnit run scripts
+Author-email: Markus Leiter <leiter@p2l2.com>
+Project-URL: Homepage, https://github.com/p2l2/VUnit-helpers
+Project-URL: Bug Tracker, https://github.com/p2l2/VUnit-helpers/issues
+Keywords: VUnit,unit testing
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# VUnit-helpers
+
+This package contains project independent tools and helpers to simplify VUnit run scripts.
+Using this, the run script gets shorter, more readable and easier to maintain. 
+
+# Installing VUnit_helpers
+You can install this package from source or via PyPi
+
+## Installing via PyPi
+
+    python -m pip install vunit_helpers
+
+## Installing from source:
+1. Clone or download the repository
+2. navigate to the directory and run ```python -m pip install .```
+
+Optionally add the ```-e``` flag to install the package in the editable mode.
+
+# Usage Examples
+
+## Get the root path of a git repository
+Working with relative paths in VUnit is dangerouse, since it depends on the working directory of python during execution. Instead, you can use your git repository as the root reference of all paths.
+``` Python
+import vunit_helpers
+git_repo_path = vunit_helpers.get_git_repo_root_path()
+```
+
+## Add UVVM to VUnit
+
+Use vunit_helpers.add_uvvm_sources() to add all UVVM source files to VUnit. VUnit will compile UVVM in the correct order.  
+
+``` Python
+from vunit import VUnit
+import vunit_helpers
+
+VU = VUnit.from_argv()
+# add all UVVM components
+vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM")
+
+# add some specific UVVM components only
+vunit_helpers.add_uvvm_sources(VU, git_repo_path / "UVVM", ["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"])
+```
+
+If you have precompiled UVVM using its compile_all.do TCL script, you can use vunit_helpers.add_precompiled_uvvm_libraries():
+``` Python
+VU = VUnit.from_argv()
+vunit_helpers.add_precompiled_uvvm_libraries(VU,["uvvm_util", "uvvm_vvc_framework", "bitvis_vip_scoreboard", "bitvis_vip_uart"],"path/to/UVVM")
+```
+
+## Advanced add Source Files
+Vunit helpers allows including and excluding wildcard patterns. That way, it's easier to exclude specific files from VUnit. 
+``` Python
+from vunit import VUnit
+import vunit_helpers
+from vunit_helpers import File_pattern
+
+VU = VUnit.from_argv()
+lib = VU.add_library("lib") 
+
+include_patterns=[
+    File_pattern(git_repo_path  / "verification"/ "*" / "hdl" / "*.vhd"),
+    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "*.vhd"),
+]
+
+# The files that match the exclude patterns won't be added to the lib (these files are excluded from the include_patterns)
+exclude_patterns=[
+    # the SPI testbench uses external_names, that are not supported in GHDL yet
+    File_pattern(git_repo_path  / "units" / "unit*" / "tb" / "tb_Formal.vhd", when_simulator_is_not="ghdl"),
+    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "AnyFileIDontWant.vhd),
+    File_pattern(git_repo_path  / "units" / "unitTop" / "tb" / "VerificationDefinitions-p.vhd", when_simulator_is="modelsim") 
+]
+vunit_helpers.advanced_add_source_files(VU,lib,include_patterns,exclude_patterns)
+```
+
+## UVVM with GHDL
+To run UVVM with GHDL, some additional compile and sim flags must be set. 
+``` Python
+VU = VUnit.from_argv()
+vunit_helpers.set_ghdl_flags_for_UVVM(VU)
+```
+
+## TOML File for RustHDL
+RustHDL is a free and open source VHDL language server. It's setup requires a TOML file, that lists all libraries and source files of a project. The fuction generate_rust_hdl_toml() will generate the TOML file for RustHDL based on all files that are included in the VUnit project. 
+Call this function after adding the files to VUnit. 
+
+``` Python
+VU = VUnit.from_argv()
+vunit_helpers.add_uvvm_sources(VU, "path/to/UVVM")
+
+vunit_helpers.generate_rust_hdl_toml(VU, str(git_repo_path / "vhdl_ls.toml"), str(git_repo_path))
+```
+
+
+
```

### Comparing `VUnit-helpers-0.1.0/src/vunit_helpers.py` & `VUnit-helpers-2023.5.7/src/vunit_helpers.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,288 +1,288 @@
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this file,
-# You can obtain one at http://mozilla.org/MPL/2.0/.
-#
-# Copyright (c) 2022-2023, Markus Leiter <leiter@p2l2.com> | www.p2l2.com
-
-import sys
-from pathlib import Path
-import subprocess
-from subprocess import call, STDOUT
-import os
-from os.path import dirname
-import logging
-from glob import glob
-from typing import Optional, List
-import toml
-
-logger = logging.getLogger('vunit_helpers')
-logger.setLevel(logging.WARNING)
-
-
-def enable_debug_logging():
-    """ 
-    Sets the logging level of the module internal logger to DEBUG.
-    """
-    logger.setLevel(logging.DEBUG)
-
-
-
-def get_git_repo_root_path():
-    """
-    Returns the absolute path to the git repository root
-    Returns None if the current directory is not within a git repository
-
-    Args:
-        path: 
-    """
-    if call(["git", "branch"], stderr=STDOUT, stdout=open(os.devnull, 'w')) != 0:
-        return None
-        logger.warning(f"This is not a git repository!")
-
-    else:
-        git_repo_dir = subprocess.Popen(
-        ['git', 'rev-parse', '--show-toplevel'], stdout=subprocess.PIPE).communicate()[0].rstrip().decode("utf-8") 
-        logger.debug(f"git repo path: {str(git_repo_dir)}")
-    return Path(git_repo_dir)
-
-
-def generate_rust_hdl_toml(VU, output_file, file_root_path):
-    """
-    Generate the toml file required by rust_hdl (vhdl_ls).
-
-    Call this function after all sources were added to VUnit. 
-    Precompiled libraries are cannot be handled by rust_hdl. 
-    Therefor, precompiled UVVM libraries won't be covered in the toml file.
-
-    Args:
-        VU: A VUnit object file.
-        output_file: A string containing the path to the output file.
-        file_root_path: root path for relative filenames. The path is used to convert them to absolute paths
-    """
-
-    # TODO: check if precompiled libraries were added
-
-    libs = VU.get_libraries()
-    vhdl_ls = {"libraries": {}}
-    for lib in libs:
-        files = []
-        for file in lib.get_source_files(allow_empty=True):
-            if os.path.isabs(file.name):
-                files.append(str(file.name))
-            else:
-                files.append(str(Path(file_root_path) / file.name))
-
-        vhdl_ls["libraries"].update(
-            {
-                lib.name: {
-                    "files": files
-                }
-            }
-        )
-    with open(output_file, "w") as f:
-        toml.dump(vhdl_ls, f)
-    logger.debug(f"rust_hdl configuration was written to {output_file}")
-
-
-def add_uvvm_sources(VU,uvvm_path,libraries=None):
-    """
-    UVVM https://github.com/UVVM/UVVM is a free and Open Source Methodology and Library which can be used in combination with VUnit.
-    Use add_uvvm to add the UVVM sources from a given path. 
-    Since UVVM is not included in VUnit, it must be cloned separately. 
-
-    Usage examples: 
-    VU.add_uvvm(uvvm_path="../UVVM") # To add all UVVM libraries
-
-    To decrease the compile duration, you can specify the libraries needed for simulation. 
-    The following example would compile  uvvm_util, uvvm_vvc_framework and bitvis_vip_clock_generator only:
-    VU.add_uvvm(uvvm_path="../UVVM", libraries=['uvvm_util', 'uvvm_vvc_framework','bitvis_vip_clock_generator'])
-
-    UVVM provides txt files with compile information. There is one txt file that lists all libraries of UVVM called component_list.txt.
-    Then, there is one file per component that lists all files of the library in compile order. This file is called compile_order.txt. 
-
-    :param uvvm_path: absolute or relative path pointing to the UVVM source directory e.g. '../UVVM'
-    :param libraries: List of UVVM libraries that are used. If libraries is None, all UVVM libraries are added to VUnit
-    """
-
-    # load the list of available UVVM components
-    component_list_file = Path(uvvm_path) / "script" / "component_list.txt"
-    if not Path(component_list_file).exists():
-        raise ValueError(f"Found no file named '{component_list_file!s}'. Probably, the UVVM path is incorrect (uvvm_path={uvvm_path}).")
-
-    uvvm_components = []
-    with open(component_list_file) as f:
-        uvvm_components = [s.strip() for s in f.readlines()] # read all components from component_list.txt
-        uvvm_components = [s for s in uvvm_components if (not s.startswith("#")) and s] # remove comments and empty lines
-
-    if libraries != None:
-        # check if all given libraries are available in UVVM
-        if not all(libname in uvvm_components for libname in libraries):
-            raise ValueError(f"some requested libraries are not available in UVVM. Requested: {libraries}, Available UVVM Components: {uvvm_components}")
-        uvvm_components = libraries 
-
-    # add source files of the components
-    for component in uvvm_components:
-        lib = VU.add_library(component)
-
-        script_dir = Path(uvvm_path) / component / "script"
-        source_files = []
-        with open(script_dir / "compile_order.txt") as f:
-            source_files = [s.strip() for s in f.readlines()] # read all lines including comments
-            source_files = [s for s in source_files if (not s.startswith("#")) and s] # remove comments and empty lines
-            #add the full path to the list of source files
-            source_files = [os.path.abspath(script_dir / Path(s)) for s in source_files]
-
-        # add the files
-        lib.add_source_files(source_files)
-
-
-def add_precompiled_uvvm_libraries(VU, used_libraries, UVVM_root_path):
-    """ 
-    Add the passed UVVM libraries to VUnit. 
-
-    To compile UVVM using modelsim, use the script compile_all.do located at UVVM/script
-    To compile UVVM using ghdl, use the script located at GHDL/src/scripts/vendors/compile-uvvm.ps1. 
-    Do not forget to setup the set the InstallationDirectory and the DestinationDirectory in config.ps1!
-
-    Args:
-        VU: A VUnit object file.
-        used_libraries: A list of uvvm libraries. E.g. ['uvvm_util','uvvm_vvc_framework','bitvis_vip_scoreboard','bitvis_vip_clock_generator']
-        UVVM_root_path: root path pointing to the UVVM directory. E.g. get_git_repo_root_path() / "verification" / "uvvm"
-    """
-    logger.debug(f"Active simulator={VU.get_simulator_name()}")
-
-    if VU.get_simulator_name() == "modelsim":
-        for libname in used_libraries:
-            location = UVVM_root_path / libname / "sim" / libname
-            VU.add_external_library(libname, location)
-            logger.debug(f"adding library {libname} from {str(location)}")
-    elif VU.get_simulator_name() == "ghdl":
-        for libname in used_libraries:
-            location = UVVM_root_path / libname / "v08"
-            VU.add_external_library(libname, location)
-            logger.debug(f"adding library {libname} from {str(location)}")
-    else:
-        logger.error(
-            f"Adding precompiled UVVM libraries for simulator {VU.get_simulator_name()} is not supported. You can use add_uvvm_sources() instead")
-
-
-def set_ghdl_flags_for_UVVM(VU):
-    """ 
-    Set all necessary flags to compile UVVM with GHDL
-
-    Args:
-        VU: A VUnit object file.
-
-    """
-    VU.add_compile_option("ghdl.a_flags", value=[
-        "-Wno-hide",
-        "-fexplicit",
-        "-Wbinding",
-        "-Wno-shared",
-        "--ieee=synopsys",
-        "--no-vital-checks",
-        "--std=08",
-        "-frelaxed",
-        "-frelaxed-rules",
-        # "-v"
-    ])
-
-    VU.set_sim_option("ghdl.elab_flags", value=[
-        "-Wno-hide",
-        "-fexplicit",
-        "-Wbinding",
-        "-Wno-shared",
-        "--ieee=synopsys",
-        "--no-vital-checks",
-        "--std=08",
-        "-frelaxed",
-        "-frelaxed-rules"
-    ])
-
-    VU.set_sim_option("ghdl.elab_e", overwrite=True, value=True)
-    logger.debug(f"GHDL flags for UVVM were set")
-
-
-class File_pattern:
-    def __init__(self, pattern, when_simulator_is=None, when_simulator_is_not=None):
-        self.pattern = str(pattern)
-
-        if isinstance(when_simulator_is, str):
-            self.include_simulators = [when_simulator_is]
-        else:
-            self.include_simulators = when_simulator_is
-
-        if isinstance(when_simulator_is_not, str):
-            self.exclude_simulators = [when_simulator_is_not]
-        else:
-            self.exclude_simulators = when_simulator_is_not
-
-
-def advanced_add_source_files(VU, lib, include_patterns, 
-                              exclude_patterns=None,
-                              preprocessors=None,
-                              include_dirs=None,
-                              defines=None,
-                              allow_empty=False,
-                              vhdl_standard: Optional[str] = None,
-                              no_parse=False,
-                              file_type=None,
-                              ):
-    """ 
-    Advanced method to include files in VUnit. This functions allows to specify include and exclude patterns for specific simulators. 
-    The function evaluates all include patterns first and removes all excluded files afterwards. 
-
-    Args:
-        VU: A VUnit object file.
-        lib: the lib where the files will be added
-        include_patterns: A list of File_patterns that shall be added to the lib
-        exclude_patterns: A list of File_patterns that shall be excluded from the include_patterns
-        All other Arguments are derived from VUnit.library.add_source_files() and directly passed through
-
-    """
-
-    include_files:List[str] = []
-    for file_pattern in include_patterns:
-        if ((file_pattern.include_simulators == None) or (VU.get_simulator_name() in file_pattern.include_simulators)) and ((file_pattern.exclude_simulators == None) or not (VU.get_simulator_name() in file_pattern.include_simulators)):
-            files = glob(file_pattern.pattern, recursive=True)
-            if not files:
-                logger.warning(
-                    f"Include file pattern {file_pattern.pattern} did not match any file!")
-            else:
-                include_files += files
-        else:
-            logger.debug(
-                f"include pattern {file_pattern.pattern} was not processed due to the used simulator ({VU.get_simulator_name()})")
-
-    exclude_files:List[str] = []
-    if exclude_patterns is not None:
-        for file_pattern in exclude_patterns:
-            if ((file_pattern.include_simulators == None) or (VU.get_simulator_name() in file_pattern.include_simulators)) and ((file_pattern.exclude_simulators == None) or not (VU.get_simulator_name() in file_pattern.include_simulators)):
-                files = glob(file_pattern.pattern, recursive=True)
-                if not files:
-                    logger.warning(
-                        f"Exclude file pattern {file_pattern.pattern} did not match any file!")
-                else:
-                    exclude_files += files
-            else:
-                logger.debug(
-                    f"exclude pattern {file_pattern.pattern} was not processed due to the used simulator ({VU.get_simulator_name()})")
-
-    file_names = [x for x in include_files if x not in exclude_files]
-
-
-    for incl in include_files:
-        logger.debug(f"including {incl}")
-    for excl in exclude_files:
-        logger.debug(f"excluding {excl}")
-    for remaining in file_names:
-        logger.debug(f"remaining {remaining}")
-
-    lib.add_source_files(file_names,
-                         preprocessors=preprocessors,
-                         include_dirs=include_dirs,
-                         defines=defines,
-                         allow_empty=allow_empty,
-                         vhdl_standard=vhdl_standard,
-                         no_parse=no_parse,
-                         file_type=file_type)
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this file,
+# You can obtain one at http://mozilla.org/MPL/2.0/.
+#
+# Copyright (c) 2022-2023, Markus Leiter <leiter@p2l2.com> | www.p2l2.com
+
+import sys
+from pathlib import Path
+import subprocess
+from subprocess import call, STDOUT
+import os
+from os.path import dirname
+import logging
+from glob import glob
+from typing import Optional, List
+import toml
+
+logger = logging.getLogger('vunit_helpers')
+logger.setLevel(logging.WARNING)
+
+
+def enable_debug_logging():
+    """ 
+    Sets the logging level of the module internal logger to DEBUG.
+    """
+    logger.setLevel(logging.DEBUG)
+
+
+
+def get_git_repo_root_path():
+    """
+    Returns the absolute path to the git repository root
+    Returns None if the current directory is not within a git repository
+
+    Args:
+        path: 
+    """
+    if call(["git", "branch"], stderr=STDOUT, stdout=open(os.devnull, 'w')) != 0:
+        return None
+        logger.warning(f"This is not a git repository!")
+
+    else:
+        git_repo_dir = subprocess.Popen(
+        ['git', 'rev-parse', '--show-toplevel'], stdout=subprocess.PIPE).communicate()[0].rstrip().decode("utf-8") 
+        logger.debug(f"git repo path: {str(git_repo_dir)}")
+    return Path(git_repo_dir)
+
+
+def generate_rust_hdl_toml(VU, output_file, file_root_path):
+    """
+    Generate the toml file required by rust_hdl (vhdl_ls).
+
+    Call this function after all sources were added to VUnit. 
+    Precompiled libraries are cannot be handled by rust_hdl. 
+    Therefor, precompiled UVVM libraries won't be covered in the toml file.
+
+    Args:
+        VU: A VUnit object file.
+        output_file: A string containing the path to the output file.
+        file_root_path: root path for relative filenames. The path is used to convert them to absolute paths
+    """
+
+    # TODO: check if precompiled libraries were added
+
+    libs = VU.get_libraries()
+    vhdl_ls = {"libraries": {}}
+    for lib in libs:
+        files = []
+        for file in lib.get_source_files(allow_empty=True):
+            if os.path.isabs(file.name):
+                files.append(str(file.name))
+            else:
+                files.append(str(Path(file_root_path) / file.name))
+
+        vhdl_ls["libraries"].update(
+            {
+                lib.name: {
+                    "files": files
+                }
+            }
+        )
+    with open(output_file, "w") as f:
+        toml.dump(vhdl_ls, f)
+    logger.debug(f"rust_hdl configuration was written to {output_file}")
+
+
+def add_uvvm_sources(VU,uvvm_path,libraries=None):
+    """
+    UVVM https://github.com/UVVM/UVVM is a free and Open Source Methodology and Library which can be used in combination with VUnit.
+    Use add_uvvm to add the UVVM sources from a given path. 
+    Since UVVM is not included in VUnit, it must be cloned separately. 
+
+    Usage examples: 
+    VU.add_uvvm(uvvm_path="../UVVM") # To add all UVVM libraries
+
+    To decrease the compile duration, you can specify the libraries needed for simulation. 
+    The following example would compile  uvvm_util, uvvm_vvc_framework and bitvis_vip_clock_generator only:
+    VU.add_uvvm(uvvm_path="../UVVM", libraries=['uvvm_util', 'uvvm_vvc_framework','bitvis_vip_clock_generator'])
+
+    UVVM provides txt files with compile information. There is one txt file that lists all libraries of UVVM called component_list.txt.
+    Then, there is one file per component that lists all files of the library in compile order. This file is called compile_order.txt. 
+
+    :param uvvm_path: absolute or relative path pointing to the UVVM source directory e.g. '../UVVM'
+    :param libraries: List of UVVM libraries that are used. If libraries is None, all UVVM libraries are added to VUnit
+    """
+
+    # load the list of available UVVM components
+    component_list_file = Path(uvvm_path) / "script" / "component_list.txt"
+    if not Path(component_list_file).exists():
+        raise ValueError(f"Found no file named '{component_list_file!s}'. Probably, the UVVM path is incorrect (uvvm_path={uvvm_path}).")
+
+    uvvm_components = []
+    with open(component_list_file) as f:
+        uvvm_components = [s.strip() for s in f.readlines()] # read all components from component_list.txt
+        uvvm_components = [s for s in uvvm_components if (not s.startswith("#")) and s] # remove comments and empty lines
+
+    if libraries != None:
+        # check if all given libraries are available in UVVM
+        if not all(libname in uvvm_components for libname in libraries):
+            raise ValueError(f"some requested libraries are not available in UVVM. Requested: {libraries}, Available UVVM Components: {uvvm_components}")
+        uvvm_components = libraries 
+
+    # add source files of the components
+    for component in uvvm_components:
+        lib = VU.add_library(component)
+
+        script_dir = Path(uvvm_path) / component / "script"
+        source_files = []
+        with open(script_dir / "compile_order.txt") as f:
+            source_files = [s.strip() for s in f.readlines()] # read all lines including comments
+            source_files = [s for s in source_files if (not s.startswith("#")) and s] # remove comments and empty lines
+            #add the full path to the list of source files
+            source_files = [os.path.abspath(script_dir / Path(s)) for s in source_files]
+
+        # add the files
+        lib.add_source_files(source_files)
+
+
+def add_precompiled_uvvm_libraries(VU, used_libraries, UVVM_root_path):
+    """ 
+    Add the passed UVVM libraries to VUnit. 
+
+    To compile UVVM using modelsim, use the script compile_all.do located at UVVM/script
+    To compile UVVM using ghdl, use the script located at GHDL/src/scripts/vendors/compile-uvvm.ps1. 
+    Do not forget to setup the set the InstallationDirectory and the DestinationDirectory in config.ps1!
+
+    Args:
+        VU: A VUnit object file.
+        used_libraries: A list of uvvm libraries. E.g. ['uvvm_util','uvvm_vvc_framework','bitvis_vip_scoreboard','bitvis_vip_clock_generator']
+        UVVM_root_path: root path pointing to the UVVM directory. E.g. get_git_repo_root_path() / "verification" / "uvvm"
+    """
+    logger.debug(f"Active simulator={VU.get_simulator_name()}")
+
+    if VU.get_simulator_name() == "modelsim":
+        for libname in used_libraries:
+            location = UVVM_root_path / libname / "sim" / libname
+            VU.add_external_library(libname, location)
+            logger.debug(f"adding library {libname} from {str(location)}")
+    elif VU.get_simulator_name() == "ghdl":
+        for libname in used_libraries:
+            location = UVVM_root_path / libname / "v08"
+            VU.add_external_library(libname, location)
+            logger.debug(f"adding library {libname} from {str(location)}")
+    else:
+        logger.error(
+            f"Adding precompiled UVVM libraries for simulator {VU.get_simulator_name()} is not supported. You can use add_uvvm_sources() instead")
+
+
+def set_ghdl_flags_for_UVVM(VU):
+    """ 
+    Set all necessary flags to compile UVVM with GHDL
+
+    Args:
+        VU: A VUnit object file.
+
+    """
+    VU.add_compile_option("ghdl.a_flags", value=[
+        "-Wno-hide",
+        "-fexplicit",
+        "-Wbinding",
+        "-Wno-shared",
+        "--ieee=synopsys",
+        "--no-vital-checks",
+        "--std=08",
+        "-frelaxed",
+        "-frelaxed-rules",
+        # "-v"
+    ])
+
+    VU.set_sim_option("ghdl.elab_flags", value=[
+        "-Wno-hide",
+        "-fexplicit",
+        "-Wbinding",
+        "-Wno-shared",
+        "--ieee=synopsys",
+        "--no-vital-checks",
+        "--std=08",
+        "-frelaxed",
+        "-frelaxed-rules"
+    ])
+
+    VU.set_sim_option("ghdl.elab_e", overwrite=True, value=True)
+    logger.debug(f"GHDL flags for UVVM were set")
+
+
+class File_pattern:
+    def __init__(self, pattern, when_simulator_is=None, when_simulator_is_not=None):
+        self.pattern = str(pattern)
+
+        if isinstance(when_simulator_is, str):
+            self.include_simulators = [when_simulator_is]
+        else:
+            self.include_simulators = when_simulator_is
+
+        if isinstance(when_simulator_is_not, str):
+            self.exclude_simulators = [when_simulator_is_not]
+        else:
+            self.exclude_simulators = when_simulator_is_not
+
+
+def advanced_add_source_files(VU, lib, include_patterns, 
+                              exclude_patterns=None,
+                              preprocessors=None,
+                              include_dirs=None,
+                              defines=None,
+                              allow_empty=False,
+                              vhdl_standard: Optional[str] = None,
+                              no_parse=False,
+                              file_type=None,
+                              ):
+    """ 
+    Advanced method to include files in VUnit. This functions allows to specify include and exclude patterns for specific simulators. 
+    The function evaluates all include patterns first and removes all excluded files afterwards. 
+
+    Args:
+        VU: A VUnit object file.
+        lib: the lib where the files will be added
+        include_patterns: A list of File_patterns that shall be added to the lib
+        exclude_patterns: A list of File_patterns that shall be excluded from the include_patterns
+        All other Arguments are derived from VUnit.library.add_source_files() and directly passed through
+
+    """
+
+    include_files:List[str] = []
+    for file_pattern in include_patterns:
+        if ((file_pattern.include_simulators == None) or (VU.get_simulator_name() in file_pattern.include_simulators)) and ((file_pattern.exclude_simulators == None) or not (VU.get_simulator_name() in file_pattern.include_simulators)):
+            files = glob(file_pattern.pattern, recursive=True)
+            if not files:
+                logger.warning(
+                    f"Include file pattern {file_pattern.pattern} did not match any file!")
+            else:
+                include_files += files
+        else:
+            logger.debug(
+                f"include pattern {file_pattern.pattern} was not processed due to the used simulator ({VU.get_simulator_name()})")
+
+    exclude_files:List[str] = []
+    if exclude_patterns is not None:
+        for file_pattern in exclude_patterns:
+            if ((file_pattern.include_simulators == None) or (VU.get_simulator_name() in file_pattern.include_simulators)) and ((file_pattern.exclude_simulators == None) or not (VU.get_simulator_name() in file_pattern.include_simulators)):
+                files = glob(file_pattern.pattern, recursive=True)
+                if not files:
+                    logger.warning(
+                        f"Exclude file pattern {file_pattern.pattern} did not match any file!")
+                else:
+                    exclude_files += files
+            else:
+                logger.debug(
+                    f"exclude pattern {file_pattern.pattern} was not processed due to the used simulator ({VU.get_simulator_name()})")
+
+    file_names = [x for x in include_files if x not in exclude_files]
+
+
+    for incl in include_files:
+        logger.debug(f"including {incl}")
+    for excl in exclude_files:
+        logger.debug(f"excluding {excl}")
+    for remaining in file_names:
+        logger.debug(f"remaining {remaining}")
+
+    lib.add_source_files(file_names,
+                         preprocessors=preprocessors,
+                         include_dirs=include_dirs,
+                         defines=defines,
+                         allow_empty=allow_empty,
+                         vhdl_standard=vhdl_standard,
+                         no_parse=no_parse,
+                         file_type=file_type)
```

