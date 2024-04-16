# Comparing `tmp/streamtape-1.0.1.tar.gz` & `tmp/streamtape-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamtape-1.0.1.tar", last modified: Tue Aug  8 11:47:37 2023, max compression
+gzip compressed data, was "streamtape-1.0.2.tar", last modified: Tue Apr 16 10:22:20 2024, max compression
```

## Comparing `streamtape-1.0.1.tar` & `streamtape-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 maximharder  (1000) maximharder  (1000)        0 2023-08-08 11:47:37.724367 streamtape-1.0.1/
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)    35148 2023-08-08 06:45:36.000000 streamtape-1.0.1/LICENSE
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     2268 2023-08-08 11:47:37.724367 streamtape-1.0.1/PKG-INFO
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     1873 2023-08-08 11:32:54.000000 streamtape-1.0.1/README.md
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)       38 2023-08-08 11:47:37.724367 streamtape-1.0.1/setup.cfg
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)      614 2023-08-08 11:13:57.000000 streamtape-1.0.1/setup.py
-drwxrwxr-x   0 maximharder  (1000) maximharder  (1000)        0 2023-08-08 11:47:37.712367 streamtape-1.0.1/streamtape/
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     1340 2023-08-08 06:26:51.000000 streamtape-1.0.1/streamtape/Account.py
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     1838 2023-08-08 06:26:51.000000 streamtape-1.0.1/streamtape/ApiResponse.py
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     4314 2023-08-08 06:26:51.000000 streamtape-1.0.1/streamtape/BaseConfig.py
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     2402 2023-08-08 11:07:47.000000 streamtape-1.0.1/streamtape/Convertation.py
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     7374 2023-08-08 11:08:13.000000 streamtape-1.0.1/streamtape/FileManager.py
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     3828 2023-08-08 11:09:08.000000 streamtape-1.0.1/streamtape/Remote.py
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     2643 2023-08-08 11:11:06.000000 streamtape-1.0.1/streamtape/Stream.py
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     2462 2023-08-08 11:37:36.000000 streamtape-1.0.1/streamtape/Upload.py
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)        0 2023-08-08 06:26:51.000000 streamtape-1.0.1/streamtape/__init__.py
-drwxrwxr-x   0 maximharder  (1000) maximharder  (1000)        0 2023-08-08 11:47:37.724367 streamtape-1.0.1/streamtape.egg-info/
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)     2268 2023-08-08 11:47:37.000000 streamtape-1.0.1/streamtape.egg-info/PKG-INFO
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)      440 2023-08-08 11:47:37.000000 streamtape-1.0.1/streamtape.egg-info/SOURCES.txt
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)        1 2023-08-08 11:47:37.000000 streamtape-1.0.1/streamtape.egg-info/dependency_links.txt
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)        1 2023-08-08 06:48:50.000000 streamtape-1.0.1/streamtape.egg-info/not-zip-safe
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)        9 2023-08-08 11:47:37.000000 streamtape-1.0.1/streamtape.egg-info/requires.txt
--rw-rw-r--   0 maximharder  (1000) maximharder  (1000)       11 2023-08-08 11:47:37.000000 streamtape-1.0.1/streamtape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 10:22:20.904936 streamtape-1.0.2/
+-rw-rw-rw-   0        0        0    35821 2024-04-16 08:31:59.000000 streamtape-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2735 2024-04-16 10:22:20.901952 streamtape-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2065 2024-04-16 08:38:22.000000 streamtape-1.0.2/README.md
+-rw-rw-rw-   0        0        0      595 2024-04-16 10:22:09.000000 streamtape-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 10:22:20.904936 streamtape-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      731 2024-04-16 08:43:14.000000 streamtape-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:22:20.885533 streamtape-1.0.2/streamtape/
+-rw-rw-rw-   0        0        0     1378 2024-04-16 08:31:59.000000 streamtape-1.0.2/streamtape/Account.py
+-rw-rw-rw-   0        0        0     1907 2024-04-16 08:31:59.000000 streamtape-1.0.2/streamtape/ApiResponse.py
+-rw-rw-rw-   0        0        0     4443 2024-04-16 08:31:59.000000 streamtape-1.0.2/streamtape/BaseConfig.py
+-rw-rw-rw-   0        0        0     2487 2024-04-16 08:31:59.000000 streamtape-1.0.2/streamtape/Convertation.py
+-rw-rw-rw-   0        0        0     7623 2024-04-16 08:31:59.000000 streamtape-1.0.2/streamtape/FileManager.py
+-rw-rw-rw-   0        0        0     3953 2024-04-16 08:31:59.000000 streamtape-1.0.2/streamtape/Remote.py
+-rw-rw-rw-   0        0        0     2734 2024-04-16 08:31:59.000000 streamtape-1.0.2/streamtape/Stream.py
+-rw-rw-rw-   0        0        0     2023 2024-04-16 08:31:59.000000 streamtape-1.0.2/streamtape/Upload.py
+-rw-rw-rw-   0        0        0        0 2024-04-16 08:31:59.000000 streamtape-1.0.2/streamtape/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 10:22:20.899535 streamtape-1.0.2/streamtape.egg-info/
+-rw-rw-rw-   0        0        0     2735 2024-04-16 10:22:20.000000 streamtape-1.0.2/streamtape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-04-16 10:22:20.000000 streamtape-1.0.2/streamtape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 10:22:20.000000 streamtape-1.0.2/streamtape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 08:33:33.000000 streamtape-1.0.2/streamtape.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-16 10:22:20.000000 streamtape-1.0.2/streamtape.egg-info/top_level.txt
```

### Comparing `streamtape-1.0.1/LICENSE` & `streamtape-1.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
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
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
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
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `streamtape-1.0.1/PKG-INFO` & `streamtape-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,122 @@
-Metadata-Version: 2.1
-Name: streamtape
-Version: 1.0.1
-Summary: Unofficial python api wrapper from https://streamtape.com
-Home-page: https://github.com/DevCraftClub/StreamTape
-Author: Maxim Harder
-Author-email: dev@devcraft.club
-Keywords: api streamtape stream video hosting unlimited
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Unofficial StreamTape API wrapper
-
-It is a simple API wrapper for the streaming service streamtape.com. The API documentation can be found on the [docs page](https://devcraftclub.github.io/StreamTape/). The whole structure of the API has been split into different classes for easy overview and usage.
-
-## Installation
-
-Install with
-
-```python3
-pip install streamtape
-```
-
-## Usage
-
-### General usage
-
-Every class starts with following initialization:
-
-```python3
-my_var = selectedClass(API_USER_KEY, API_PASSWORD)
-```
-
-API key and password you can get in your account in **[Account Settings](https://streamtape.com/accpanel#accsettings)**.
-
-### General response
-
-For the general purpose of any response, the ApiResponse class has been created to return a dict with this structure:
-
-```json
-{
-    "status": <status-code>,
-    "msg": "<informational message. might vary, use the status code in your code!>",
-    "result": <result of the request. varies depending on the request>
-}
-```
-
-### Account
-
-Example
-
-```python
-account = Account(API_USER_KEY, API_PASSWORD)
-print(account.get_info())
-```
-
-### Convertation
-
-Example
-
-```python
-converts = Convertation(API_USER_KEY, API_PASSWORD)
-print(converts.list_converts())
-```
-
-### FileManager
-
-Class for working with files and folders
-
-Example
-
-```python
-f_manager = FileManager(API_USER_KEY, API_PASSWORD)
-print(f_manager.list_data())
-```
-
-### Remote
-
-Example
-
-```python
-remote = Remote(API_USER_KEY, API_PASSWORD)
-print(remote.remote_upload("path_to_file", "folder_id"))
-```
-
-### Stream
-
-Example
-
-```python
-stream = Stream(API_USER_KEY, API_PASSWORD)
-print(stream.file_info("file_id"))
-```
-
-### Upload
-
-Example
-
-```python
-uploader = Upload(API_USER_KEY, API_PASSWORD)
-print(uploader.upload("path_to_file", "folder_id"))
-```
-
-## Changelog
-
-### 1.0.0
-
-- Initial release   
-
-### 1.0.1
-
-- Fixed variables
-- Fixed upload parameters
+Metadata-Version: 2.1
+Name: streamtape
+Version: 1.0.2
+Summary: Unofficial python api wrapper from https://streamtape.come
+Home-page: https://github.com/DevCraftClub/StreamTape
+Author-email: Maxim Harder <dev@devcraft.club>
+Project-URL: Homepage, https://github.com/DevCraftClub/StreamTape
+Project-URL: Issues, https://github.com/DevCraftClub/StreamTape/issues
+Project-URL: Docs, https://devcraftclub.github.io/StreamTape/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Unofficial StreamTape API wrapper
+
+It is a simple API wrapper for the streaming service streamtape.com. The API documentation can be found on the [docs page](https://devcraftclub.github.io/StreamTape/). The whole structure of the API has been split into different classes for easy overview and usage.
+
+## Installation
+
+Install with
+
+```python3
+pip install streamtape
+```
+
+## Usage
+
+### General usage
+
+Every class starts with following initialization:
+
+```python3
+my_var = selectedClass(API_USER_KEY, API_PASSWORD)
+```
+
+API key and password you can get in your account in **[Account Settings](https://streamtape.com/accpanel#accsettings)**.
+
+### General response
+
+For the general purpose of any response, the ApiResponse class has been created to return a dict with this structure:
+
+```json
+{
+    "status": <status-code>,
+    "msg": "<informational message. might vary, use the status code in your code!>",
+    "result": <result of the request. varies depending on the request>
+}
+```
+
+### Account
+
+Example
+
+```python
+account = Account(API_USER_KEY, API_PASSWORD)
+print(account.get_info())
+```
+
+### Convertation
+
+Example
+
+```python
+converts = Convertation(API_USER_KEY, API_PASSWORD)
+print(converts.list_converts())
+```
+
+### FileManager
+
+Class for working with files and folders
+
+Example
+
+```python
+f_manager = FileManager(API_USER_KEY, API_PASSWORD)
+print(f_manager.list_data())
+```
+
+### Remote
+
+Example
+
+```python
+remote = Remote(API_USER_KEY, API_PASSWORD)
+print(remote.remote_upload("path_to_file", "folder_id"))
+```
+
+### Stream
+
+Example
+
+```python
+stream = Stream(API_USER_KEY, API_PASSWORD)
+print(stream.file_info("file_id"))
+```
+
+### Upload
+
+Example
+
+```python
+uploader = Upload(API_USER_KEY, API_PASSWORD)
+print(uploader.upload("path_to_file", "folder_id"))
+```
+
+## Changelog
+
+### 1.0.0
+
+- Initial release
+
+### 1.0.1
+
+- Fixed variables
+- Fixed upload parameters
+
+### 1.0.2
+
+* Fixed API link (thx to @[Gairolarishav](https://github.com/Gairolarishav))
```

### Comparing `streamtape-1.0.1/README.md` & `streamtape-1.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,102 +1,106 @@
-# Unofficial StreamTape API wrapper
-
-It is a simple API wrapper for the streaming service streamtape.com. The API documentation can be found on the [docs page](https://devcraftclub.github.io/StreamTape/). The whole structure of the API has been split into different classes for easy overview and usage.
-
-## Installation
-
-Install with
-
-```python3
-pip install streamtape
-```
-
-## Usage
-
-### General usage
-
-Every class starts with following initialization:
-
-```python3
-my_var = selectedClass(API_USER_KEY, API_PASSWORD)
-```
-
-API key and password you can get in your account in **[Account Settings](https://streamtape.com/accpanel#accsettings)**.
-
-### General response
-
-For the general purpose of any response, the ApiResponse class has been created to return a dict with this structure:
-
-```json
-{
-    "status": <status-code>,
-    "msg": "<informational message. might vary, use the status code in your code!>",
-    "result": <result of the request. varies depending on the request>
-}
-```
-
-### Account
-
-Example
-
-```python
-account = Account(API_USER_KEY, API_PASSWORD)
-print(account.get_info())
-```
-
-### Convertation
-
-Example
-
-```python
-converts = Convertation(API_USER_KEY, API_PASSWORD)
-print(converts.list_converts())
-```
-
-### FileManager
-
-Class for working with files and folders
-
-Example
-
-```python
-f_manager = FileManager(API_USER_KEY, API_PASSWORD)
-print(f_manager.list_data())
-```
-
-### Remote
-
-Example
-
-```python
-remote = Remote(API_USER_KEY, API_PASSWORD)
-print(remote.remote_upload("path_to_file", "folder_id"))
-```
-
-### Stream
-
-Example
-
-```python
-stream = Stream(API_USER_KEY, API_PASSWORD)
-print(stream.file_info("file_id"))
-```
-
-### Upload
-
-Example
-
-```python
-uploader = Upload(API_USER_KEY, API_PASSWORD)
-print(uploader.upload("path_to_file", "folder_id"))
-```
-
-## Changelog
-
-### 1.0.0
-
-- Initial release   
-
-### 1.0.1
-
-- Fixed variables
-- Fixed upload parameters
+# Unofficial StreamTape API wrapper
+
+It is a simple API wrapper for the streaming service streamtape.com. The API documentation can be found on the [docs page](https://devcraftclub.github.io/StreamTape/). The whole structure of the API has been split into different classes for easy overview and usage.
+
+## Installation
+
+Install with
+
+```python3
+pip install streamtape
+```
+
+## Usage
+
+### General usage
+
+Every class starts with following initialization:
+
+```python3
+my_var = selectedClass(API_USER_KEY, API_PASSWORD)
+```
+
+API key and password you can get in your account in **[Account Settings](https://streamtape.com/accpanel#accsettings)**.
+
+### General response
+
+For the general purpose of any response, the ApiResponse class has been created to return a dict with this structure:
+
+```json
+{
+    "status": <status-code>,
+    "msg": "<informational message. might vary, use the status code in your code!>",
+    "result": <result of the request. varies depending on the request>
+}
+```
+
+### Account
+
+Example
+
+```python
+account = Account(API_USER_KEY, API_PASSWORD)
+print(account.get_info())
+```
+
+### Convertation
+
+Example
+
+```python
+converts = Convertation(API_USER_KEY, API_PASSWORD)
+print(converts.list_converts())
+```
+
+### FileManager
+
+Class for working with files and folders
+
+Example
+
+```python
+f_manager = FileManager(API_USER_KEY, API_PASSWORD)
+print(f_manager.list_data())
+```
+
+### Remote
+
+Example
+
+```python
+remote = Remote(API_USER_KEY, API_PASSWORD)
+print(remote.remote_upload("path_to_file", "folder_id"))
+```
+
+### Stream
+
+Example
+
+```python
+stream = Stream(API_USER_KEY, API_PASSWORD)
+print(stream.file_info("file_id"))
+```
+
+### Upload
+
+Example
+
+```python
+uploader = Upload(API_USER_KEY, API_PASSWORD)
+print(uploader.upload("path_to_file", "folder_id"))
+```
+
+## Changelog
+
+### 1.0.0
+
+- Initial release
+
+### 1.0.1
+
+- Fixed variables
+- Fixed upload parameters
+
+### 1.0.2
+
+* Fixed API link (thx to @[Gairolarishav](https://github.com/Gairolarishav))
```

### Comparing `streamtape-1.0.1/streamtape/Account.py` & `streamtape-1.0.2/streamtape/Account.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Any, Dict, Optional
-
-from streamtape.ApiResponse import ApiResponse
-from streamtape.BaseConfig import BaseConfig
-
-
-class Account(BaseConfig):
-	parameter: str = "parameter"
-
-	def __init__(self, user: str, password: str):
-		super().__init__(user, password)
-
-	def get_info(self) -> dict:
-		"""
-		Retrieves information about the user from the API.
-
-		Returns:
-		    A dictionary containing the user's information if the API response status is 200.
-		    The dictionary includes the following keys:
-		        - 'apiid': The user's API ID.
-		        - 'email': The user's email address.
-		        - 'signup_at': The user's signup date and time in datetime format.
-
-		    If the API response status is not 200, an error response dictionary is returned.
-		    The error response dictionary includes the following keys:
-		        - 'status': The API response status code.
-		        - 'msg': The error message returned by the API.
-		"""
-		url = self.url_query(f"{self.parameter}/info")
-		response = BaseConfig.send_request(url)
-		if response["status"] == 200:
-			return {
-				"apiid"    : response.result.get('apiid'),
-				"email"    : response.result.get('email'),
-				"signup_at": BaseConfig.str_to_datetime(response.result.get('signup_at'))
-			}
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
+from typing import Any, Dict, Optional
+
+from streamtape.ApiResponse import ApiResponse
+from streamtape.BaseConfig import BaseConfig
+
+
+class Account(BaseConfig):
+	parameter: str = "parameter"
+
+	def __init__(self, user: str, password: str):
+		super().__init__(user, password)
+
+	def get_info(self) -> dict:
+		"""
+		Retrieves information about the user from the API.
+
+		Returns:
+		    A dictionary containing the user's information if the API response status is 200.
+		    The dictionary includes the following keys:
+		        - 'apiid': The user's API ID.
+		        - 'email': The user's email address.
+		        - 'signup_at': The user's signup date and time in datetime format.
+
+		    If the API response status is not 200, an error response dictionary is returned.
+		    The error response dictionary includes the following keys:
+		        - 'status': The API response status code.
+		        - 'msg': The error message returned by the API.
+		"""
+		url = self.url_query(f"{self.parameter}/info")
+		response = BaseConfig.send_request(url)
+		if response["status"] == 200:
+			return {
+				"apiid"    : response.result.get('apiid'),
+				"email"    : response.result.get('email'),
+				"signup_at": BaseConfig.str_to_datetime(response.result.get('signup_at'))
+			}
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
```

### Comparing `streamtape-1.0.1/streamtape/ApiResponse.py` & `streamtape-1.0.2/streamtape/ApiResponse.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from typing import Optional, Union
-
-
-class ApiResponse:
-	status: Optional[int] = None
-	msg: Optional[str] = None
-	result: Optional[Union[list, bool, dict]] = None
-
-	@staticmethod
-	def message_info(status: int) -> str:
-		"""
-		Returns a message corresponding to the given status code.
-
-		Parameters:
-			- status (int): The status code to retrieve the message for.
-
-		Returns:
-			- str: The message corresponding to the given status code.
-
-		Raises:
-			- None
-
-		Examples:
-		>>> message_info(200)
-		'Everything is OK. Request succeeded'
-		>>> message_info(404)
-		'File not found'
-		>>> message_info(503)
-		'Some error occurred'
-		"""
-		msg = "Some error occurred"
-
-		if status == 200: msg = "Everything is OK. Request succeeded"
-		elif status == 400: msg = "Bad request (e.g. wrong parameters)"
-		elif status == 403: msg = "Permission denied (wrong api login/key, action on a file which does not belong to you, ...)"
-		elif status == 404: msg = "File not found"
-		elif status == 451: msg = "Unavailable For Legal Reasons"
-		elif status == 509: msg = "Bandwidth usage exceeded. Please try again later. (you might see this during peak hours)"
-		elif status != 509 and 500 <= status < 600: msg = "Server errors"
-
-		return msg
-
-	@staticmethod
-	def error_response(status: int, error_msg: str):
-		"""
-		Returns a dictionary representing an error response.
-
-		Parameters:
-		- status (int): The status code of the error.
-		- error_msg (str): The error message.
-
-		Returns:
-		- dict: A dictionary containing the error information.
-
-		Example:
-		>>> error_response(404, "Page not found")
-		{
-		    'error': True,
-		    'status_id': 404,
-		    'error_msg': 'Not Found',
-		    'api_msg': 'Page not found'
-		}
-		"""
-		return {
-			'error'    : True,
-			'status_id': status,
-			'error_msg': ApiResponse.message_info(status),
-			'api_msg'  : error_msg
-		}
+from typing import Optional, Union
+
+
+class ApiResponse:
+	status: Optional[int] = None
+	msg: Optional[str] = None
+	result: Optional[Union[list, bool, dict]] = None
+
+	@staticmethod
+	def message_info(status: int) -> str:
+		"""
+		Returns a message corresponding to the given status code.
+
+		Parameters:
+			- status (int): The status code to retrieve the message for.
+
+		Returns:
+			- str: The message corresponding to the given status code.
+
+		Raises:
+			- None
+
+		Examples:
+		>>> message_info(200)
+		'Everything is OK. Request succeeded'
+		>>> message_info(404)
+		'File not found'
+		>>> message_info(503)
+		'Some error occurred'
+		"""
+		msg = "Some error occurred"
+
+		if status == 200: msg = "Everything is OK. Request succeeded"
+		elif status == 400: msg = "Bad request (e.g. wrong parameters)"
+		elif status == 403: msg = "Permission denied (wrong api login/key, action on a file which does not belong to you, ...)"
+		elif status == 404: msg = "File not found"
+		elif status == 451: msg = "Unavailable For Legal Reasons"
+		elif status == 509: msg = "Bandwidth usage exceeded. Please try again later. (you might see this during peak hours)"
+		elif status != 509 and 500 <= status < 600: msg = "Server errors"
+
+		return msg
+
+	@staticmethod
+	def error_response(status: int, error_msg: str):
+		"""
+		Returns a dictionary representing an error response.
+
+		Parameters:
+		- status (int): The status code of the error.
+		- error_msg (str): The error message.
+
+		Returns:
+		- dict: A dictionary containing the error information.
+
+		Example:
+		>>> error_response(404, "Page not found")
+		{
+		    'error': True,
+		    'status_id': 404,
+		    'error_msg': 'Not Found',
+		    'api_msg': 'Page not found'
+		}
+		"""
+		return {
+			'error'    : True,
+			'status_id': status,
+			'error_msg': ApiResponse.message_info(status),
+			'api_msg'  : error_msg
+		}
```

### Comparing `streamtape-1.0.1/streamtape/BaseConfig.py` & `streamtape-1.0.2/streamtape/BaseConfig.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-from datetime import datetime
-from typing import Optional
-from urllib.parse import urlencode
-
-import requests
-
-from streamtape.ApiResponse import ApiResponse
-
-
-class BaseConfig:
-	url: str = 'https://api.streamtape.com'
-	api_user: Optional[str] = None
-	api_password: Optional[str] = None
-
-	def __init__(self, user: str, password: str):
-		"""
-		Initializes an instance of the class with the provided user and password.
-
-		Args:
-		    - user (str): The username for the API authentication.
-		    - password (str): The password for the API authentication.
-
-		Returns:
-		    - None
-		"""
-		self.api_user = user
-		self.api_password = password
-
-	def set_api_url(self, url: str):
-		"""
-		Sets the API URL for the object.
-
-		Parameters:
-		- self: The object itself.
-		- url (str): The URL to be set as the API URL.
-
-		Returns:
-		- None
-
-		Example:
-		>>> obj = MyClass()
-		>>> obj.set_api_url("https://api.example.com")
-		"""
-		self.url = url
-
-	def url_query(self, parameter: str, query: dict = {}, use_login: bool = True) -> str:
-		"""
-		Constructs a URL query string for making API requests.
-
-		Args:
-		    - self (object): The instance of the class.
-		    - parameter (str): The parameter to be appended to the base URL.
-		    - query (dict, optional): Additional query parameters to be included in the URL. Defaults to an empty dictionary.
-		    - use_login (bool, optional): Flag indicating whether to include login credentials in the query parameters. Defaults to True.
-
-		Returns:
-		    - str: The constructed URL query string.
-
-		Example:
-		    >>> obj = ClassName()
-		    >>> obj.url_query("endpoint", {"param1": "value1", "param2": "value2"}, False)
-		    'https://example.com/endpoint?param1=value1&param2=value2'
-		"""
-		api_url = f"{self.url}/{parameter}"
-		api_query = {"login": self.api_user, "key": self.api_password} if use_login else {}
-		api_query = {**api_query, **query}
-
-		return f"{api_url}?{urlencode(api_query)}"
-
-	@staticmethod
-	def send_request(url: str, type_request: str = 'GET', data: Optional[dict] = None, parameters: Optional[dict] = None, files: Optional[dict] = None) -> ApiResponse:
-		"""
-		Sends a HTTP request to the specified URL using the specified request type.
-
-		Args:
-			- url (str): The URL to send the request to.
-			- type_request (str, optional): The type of request to send. Defaults to 'GET'.
-			- data (dict, optional): The data to send with the request. Defaults to None.
-			- parameters (dict, optional): The parameters to include in the request. Defaults to None.
-			- files (dict, optional): The files to include in the request. Defaults to None.
-
-		Returns:
-			- ApiResponse: The response from the server.
-
-		Raises:
-			None
-
-		Examples:
-			>>> response = send_request('https://api.example.com/users', type_request='GET')
-			{
-				"status": <status-code>,
-				"msg": "<informational message. might vary, use the status code in your code!>",
-				"result": <result of the request. varies depending on the request>
-			}
-		"""
-		s = requests.Session()
-		response: Optional[ApiResponse] = None
-		if type_request.upper() == 'GET':
-			response = s.get(url, data=data, params=parameters, files=files).json()
-		elif type_request.upper() == 'POST':
-			response = s.post(url, data=data, params=parameters, files=files).json()
-
-		return response
-
-	@staticmethod
-	def str_to_datetime(date_string: str, format_string: str = '%y-%m-%d %H:%M:%S'):
-		"""
-		Converts a string representation of a date and time to a datetime object.
-
-		Args:
-			- date_string (str): The string representation of the date and time.
-			- format_string (str, optional): The format string specifying the expected format of the date and time string.
-				Defaults to '%y-%m-%d %H:%M:%S'.
-
-		Returns:
-			- datetime: A datetime object representing the parsed date and time.
-
-		Raises:
-			- ValueError: If the date_string does not match the format_string.
-
-		Examples:
-			>>> str_to_datetime('2022-01-01 12:00:00')
-			datetime.datetime(2022, 1, 1, 12, 0)
-
-			>>> str_to_datetime('01-01-2022 12:00:00', '%d-%m-%Y %H:%M:%S')
-			datetime.datetime(2022, 1, 1, 12, 0)
-
-		Note:
-			- The format_string follows the same conventions as the strftime() method of datetime objects.
-			- If the date_string does not match the format_string, a ValueError is raised.
-		"""
-		return datetime.strptime(date_string, format_string)
+from datetime import datetime
+from typing import Optional
+from urllib.parse import urlencode
+
+import requests
+
+from streamtape.ApiResponse import ApiResponse
+
+
+class BaseConfig:
+	url: str = 'https://api.strcloud.in'
+	api_user: Optional[str] = None
+	api_password: Optional[str] = None
+
+	def __init__(self, user: str, password: str):
+		"""
+		Initializes an instance of the class with the provided user and password.
+
+		Args:
+		    - user (str): The username for the API authentication.
+		    - password (str): The password for the API authentication.
+
+		Returns:
+		    - None
+		"""
+		self.api_user = user
+		self.api_password = password
+
+	def set_api_url(self, url: str):
+		"""
+		Sets the API URL for the object.
+
+		Parameters:
+		- self: The object itself.
+		- url (str): The URL to be set as the API URL.
+
+		Returns:
+		- None
+
+		Example:
+		>>> obj = MyClass()
+		>>> obj.set_api_url("https://api.example.com")
+		"""
+		self.url = url
+
+	def url_query(self, parameter: str, query: dict = {}, use_login: bool = True) -> str:
+		"""
+		Constructs a URL query string for making API requests.
+
+		Args:
+		    - self (object): The instance of the class.
+		    - parameter (str): The parameter to be appended to the base URL.
+		    - query (dict, optional): Additional query parameters to be included in the URL. Defaults to an empty dictionary.
+		    - use_login (bool, optional): Flag indicating whether to include login credentials in the query parameters. Defaults to True.
+
+		Returns:
+		    - str: The constructed URL query string.
+
+		Example:
+		    >>> obj = ClassName()
+		    >>> obj.url_query("endpoint", {"param1": "value1", "param2": "value2"}, False)
+		    'https://example.com/endpoint?param1=value1&param2=value2'
+		"""
+		api_url = f"{self.url}/{parameter}"
+		api_query = {"login": self.api_user, "key": self.api_password} if use_login else {}
+		api_query = {**api_query, **query}
+
+		return f"{api_url}?{urlencode(api_query)}"
+
+	@staticmethod
+	def send_request(url: str, type_request: str = 'GET', data: Optional[dict] = None, parameters: Optional[dict] = None, files: Optional[dict] = None) -> ApiResponse:
+		"""
+		Sends a HTTP request to the specified URL using the specified request type.
+
+		Args:
+			- url (str): The URL to send the request to.
+			- type_request (str, optional): The type of request to send. Defaults to 'GET'.
+			- data (dict, optional): The data to send with the request. Defaults to None.
+			- parameters (dict, optional): The parameters to include in the request. Defaults to None.
+			- files (dict, optional): The files to include in the request. Defaults to None.
+
+		Returns:
+			- ApiResponse: The response from the server.
+
+		Raises:
+			None
+
+		Examples:
+			>>> response = send_request('https://api.example.com/users', type_request='GET')
+			{
+				"status": <status-code>,
+				"msg": "<informational message. might vary, use the status code in your code!>",
+				"result": <result of the request. varies depending on the request>
+			}
+		"""
+		s = requests.Session()
+		response: Optional[ApiResponse] = None
+		if type_request.upper() == 'GET':
+			response = s.get(url, data=data, params=parameters, files=files).json()
+		elif type_request.upper() == 'POST':
+			response = s.post(url, data=data, params=parameters, files=files).json()
+
+		return response
+
+	@staticmethod
+	def str_to_datetime(date_string: str, format_string: str = '%y-%m-%d %H:%M:%S'):
+		"""
+		Converts a string representation of a date and time to a datetime object.
+
+		Args:
+			- date_string (str): The string representation of the date and time.
+			- format_string (str, optional): The format string specifying the expected format of the date and time string.
+				Defaults to '%y-%m-%d %H:%M:%S'.
+
+		Returns:
+			- datetime: A datetime object representing the parsed date and time.
+
+		Raises:
+			- ValueError: If the date_string does not match the format_string.
+
+		Examples:
+			>>> str_to_datetime('2022-01-01 12:00:00')
+			datetime.datetime(2022, 1, 1, 12, 0)
+
+			>>> str_to_datetime('01-01-2022 12:00:00', '%d-%m-%Y %H:%M:%S')
+			datetime.datetime(2022, 1, 1, 12, 0)
+
+		Note:
+			- The format_string follows the same conventions as the strftime() method of datetime objects.
+			- If the date_string does not match the format_string, a ValueError is raised.
+		"""
+		return datetime.strptime(date_string, format_string)
```

### Comparing `streamtape-1.0.1/streamtape/Convertation.py` & `streamtape-1.0.2/streamtape/Convertation.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-from typing import Union
-
-from streamtape.ApiResponse import ApiResponse
-from streamtape.BaseConfig import BaseConfig
-
-
-class Convertation(BaseConfig):
-	parameter: str = "file"
-
-	def __init__(self, user: str, password: str):
-		super().__init__(user, password)
-
-	def list_converts(self) -> Union[dict, list]:
-		"""
-		Retrieves a list of running converts from the specified URL.
-
-		Returns:
-			- Union[Dict, List]: A dictionary or a list containing the running converts.
-
-		Raises:
-			- ApiResponse: If the API response status is not 200, an error response is returned.
-		"""
-
-		url = self.url_query(f"{self.parameter}/runningconverts")
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return response["result"]
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def list_failed_converts(self) -> Union[dict, list]:
-		"""
-		Retrieves a list of failed conversions from the specified URL.
-
-		Returns:
-		    - Union[Dict, List]: A dictionary or a list containing the failed conversions.
-
-		Raises:
-		    - ApiResponseError: If the API response status is not 200.
-
-		Example:
-		    >>> obj = YourClassName()
-		    >>> obj.list_failed_converts()
-		    {'status': 200, 'result': ['conversion1', 'conversion2']}
-		"""
-		url = self.url_query(f"{self.parameter}/failedconverts")
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return response["result"]
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def get_thumbnail(self, file_id: str) -> Union[dict, list]:
-		"""
-		Retrieves the thumbnail for a given file ID.
-
-		Args:
-		    - self (object): The instance of the class.
-		    - file_id (str): The ID of the file for which the thumbnail is requested.
-
-		Returns:
-		    - Union[dict, list]: The thumbnail information as a dictionary or a list.
-
-		Raises:
-		    - ApiResponseError: If the API response status is not 200.
-
-		Example:
-		    >>> thumbnail = get_thumbnail("file123")
-		    {
-				"status": 200,
-				"msg": "OK",
-				"result": "https://thumb.tapecontent.net/thumb/wg8ad12d3QiJRXG/thumb.jpg"
-			}
-		"""
-		url = self.url_query(f"{self.parameter}/getsplash", query={
-			"file": file_id
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return response["result"]
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
+from typing import Union
+
+from streamtape.ApiResponse import ApiResponse
+from streamtape.BaseConfig import BaseConfig
+
+
+class Convertation(BaseConfig):
+	parameter: str = "file"
+
+	def __init__(self, user: str, password: str):
+		super().__init__(user, password)
+
+	def list_converts(self) -> Union[dict, list]:
+		"""
+		Retrieves a list of running converts from the specified URL.
+
+		Returns:
+			- Union[Dict, List]: A dictionary or a list containing the running converts.
+
+		Raises:
+			- ApiResponse: If the API response status is not 200, an error response is returned.
+		"""
+
+		url = self.url_query(f"{self.parameter}/runningconverts")
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return response["result"]
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def list_failed_converts(self) -> Union[dict, list]:
+		"""
+		Retrieves a list of failed conversions from the specified URL.
+
+		Returns:
+		    - Union[Dict, List]: A dictionary or a list containing the failed conversions.
+
+		Raises:
+		    - ApiResponseError: If the API response status is not 200.
+
+		Example:
+		    >>> obj = YourClassName()
+		    >>> obj.list_failed_converts()
+		    {'status': 200, 'result': ['conversion1', 'conversion2']}
+		"""
+		url = self.url_query(f"{self.parameter}/failedconverts")
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return response["result"]
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def get_thumbnail(self, file_id: str) -> Union[dict, list]:
+		"""
+		Retrieves the thumbnail for a given file ID.
+
+		Args:
+		    - self (object): The instance of the class.
+		    - file_id (str): The ID of the file for which the thumbnail is requested.
+
+		Returns:
+		    - Union[dict, list]: The thumbnail information as a dictionary or a list.
+
+		Raises:
+		    - ApiResponseError: If the API response status is not 200.
+
+		Example:
+		    >>> thumbnail = get_thumbnail("file123")
+		    {
+				"status": 200,
+				"msg": "OK",
+				"result": "https://thumb.tapecontent.net/thumb/wg8ad12d3QiJRXG/thumb.jpg"
+			}
+		"""
+		url = self.url_query(f"{self.parameter}/getsplash", query={
+			"file": file_id
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return response["result"]
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
```

### Comparing `streamtape-1.0.1/streamtape/FileManager.py` & `streamtape-1.0.2/streamtape/FileManager.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-from typing import Optional, Union
-
-from streamtape.ApiResponse import ApiResponse
-from streamtape.BaseConfig import BaseConfig
-
-
-class FileManager(BaseConfig):
-	parameter: str = "file"
-
-	def __init__(self, user: str, password: str):
-		super().__init__(user, password)
-
-	def list_data(self, folder_id: Optional[str] = None) -> Union[dict, list]:
-		"""
-		Retrieves a list of data from a specified folder.
-
-		Args:
-		    - folder_id (Optional[str]): The ID of the folder to retrieve data from. Defaults to None.
-
-		Returns:
-		    - Union[dict, list]: A dictionary or list containing the retrieved data.
-
-		Raises:
-		    - ApiResponseError: If the API response status is not 200.
-
-		Example:
-		    >>> list_data("folder123")
-		    {
-				"status": 200,
-				"msg": "OK",
-				"result": {
-					"folders": [
-					    {
-						    "id": "B-qlJkdHFeo",
-						    "name": "Subfolder"
-					    }
-					],
-					"files": [
-					    {
-						    "name": "MyMinecraftLetsPlay.mp4",
-							"size": 7040842,
-							"link": "https://streamtape.com/v/rbAarvRPXdYbaxY/MyMinecraftLetsPlay.mp4",
-							"created_at": 1585532987430,
-							"downloads": 0,
-							"linkid": "rbAarvRPXdYbaxY",
-							"convert": "converted"
-					    }
-					]
-				}
-			}
-		"""
-		url = self.url_query(f"{self.parameter}/listfolder", query={
-			"folder": folder_id,
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return response["result"]
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def create_folder(self, folder_name: str, parent_folder: Optional[str] = None) -> dict:
-		"""
-		Creates a new folder with the given folder name and parent folder.
-
-		Args:
-		    - folder_name (str): The name of the folder to be created.
-		    - parent_folder (str, optional): The ID of the parent folder. Defaults to None.
-
-		Returns:
-		    - dict: A dictionary containing the folder ID if the folder is created successfully.
-		          If an error occurs, an error response dictionary is returned.
-
-		Raises:
-		    - ApiResponseError: If the API response status is not 200.
-
-		Example:
-		    >>> create_folder("New Folder", "12345")
-			{
-				"status": 200,
-				"msg": "OK",
-				"result": {
-				    "folderid": "LnvnE51P5gc"
-				}
-			}
-		"""
-		url = self.url_query(f"{self.parameter}/createfolder", query={
-			"name": folder_name,
-			"pid" : parent_folder,
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return {
-				"folderid": response["result"].get("folderid")
-			}
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def rename_folder(self, folder_name: str, parent_folder: str) -> Union[dict, bool]:
-		"""
-		Renames a folder with the given folder_name and moves it to the specified parent_folder.
-
-		Args:
-		    - folder_name (str): The name of the folder to be renamed.
-		    - parent_folder (str): The name of the parent folder where the renamed folder will be moved.
-
-		Returns:
-		    - Union[dict, bool]: Returns a boolean value indicating the success of the renaming operation if the response status is 200.
-		                       Otherwise, returns an error response as a dictionary using the ApiResponse.error_response method.
-
-		Raises:
-		    - ApiResponseError: If the API response status is not 200.
-		"""
-		url = self.url_query(f"{self.parameter}/renamefolder", query={
-			"name"  : folder_name,
-			"folder": parent_folder,
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return bool(response["result"])
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def delete_folder(self, folder_id: str) -> Union[dict, bool]:
-		"""
-		Deletes a folder with the given folder_id.
-
-		Args:
-		    - folder_id (str): The ID of the folder to be deleted.
-
-		Returns:
-		    - Union[dict, bool]: Returns a boolean value indicating the success of the deletion operation if the response status is 200.
-		                       If the response status is not 200, returns an error response dictionary.
-
-		Raises:
-		    - ApiResponseError: If the API response status is not 200.
-
-		Example:
-		    >>> delete_folder("folder123")
-		    {
-				"status": 200,
-				"msg": "OK",
-				"result": true
-			}
-		"""
-		url = self.url_query(f"{self.parameter}/deletefolder", query={
-			"folder": folder_id,
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return bool(response["result"])
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def rename_file(self, file: str, name: str) -> Union[dict, bool]:
-		"""
-		Renames a file with the given name.
-
-		Args:
-		    - file (str): The name of the file to be renamed.
-		    - name (str): The new name for the file.
-
-		Returns:
-		    - Union[dict, bool]: Returns a dictionary containing the response result if the request is successful,
-		    otherwise returns a boolean value indicating the success of the request.
-
-		Raises:
-		    - ApiResponse: If the response status is not 200, an ApiResponse error response is raised.
-
-		Example:
-		    >>> obj = MyClass()
-		    >>> obj.rename_file("old_file.txt", "new_file.txt")
-		    {
-				"status": 200,
-				"msg": "OK",
-				"result": true
-			}
-		"""
-		url = self.url_query(f"{self.parameter}/deletefolder", query={
-			"file": file,
-			"name": name
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return bool(response["result"])
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def move_file(self, file_id: str, folder_id: str) -> Union[dict, bool]:
-		"""
-		Moves a file to a specified folder.
-
-		Args:
-		    - file_id (str): The ID of the file to be moved.
-		    - folder_id (str): The ID of the folder to which the file will be moved.
-
-		Returns:
-		    - Union[dict, bool]: Returns a boolean value indicating the success of the operation if the response status is 200.
-		                       Otherwise, returns an error response as a dictionary containing the status code and error message.
-
-		Raises:
-		    - ApiResponse: If the response status is not 200, an ApiResponse error response is raised.
-		"""
-		url = self.url_query(f"{self.parameter}/move", query={
-			"file"  : file_id,
-			"folder": folder_id
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return bool(response["result"])
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def delete_file(self, file_id: str) -> Union[dict, bool]:
-		"""
-		Deletes a file with the given file_id.
-
-		Args:
-		    - file_id (str): The ID of the file to be deleted.
-
-		Returns:
-		    - Union[dict, bool]: Returns a boolean value indicating the success of the deletion operation if the response status is 200.
-		                       If the response status is not 200, returns an error response dictionary.
-
-		Raises:
-		    - ApiResponse: If the response status is not 200, an ApiResponse error response is raised.
-
-		Example:
-		    >>> delete_file("file123")
-		    {
-				"status": 200,
-				"msg": "OK",
-				"result": true
-			}
-		"""
-		url = self.url_query(f"{self.parameter}/delete", query={
-			"file": file_id
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return bool(response["result"])
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
+from typing import Optional, Union
+
+from streamtape.ApiResponse import ApiResponse
+from streamtape.BaseConfig import BaseConfig
+
+
+class FileManager(BaseConfig):
+	parameter: str = "file"
+
+	def __init__(self, user: str, password: str):
+		super().__init__(user, password)
+
+	def list_data(self, folder_id: Optional[str] = None) -> Union[dict, list]:
+		"""
+		Retrieves a list of data from a specified folder.
+
+		Args:
+		    - folder_id (Optional[str]): The ID of the folder to retrieve data from. Defaults to None.
+
+		Returns:
+		    - Union[dict, list]: A dictionary or list containing the retrieved data.
+
+		Raises:
+		    - ApiResponseError: If the API response status is not 200.
+
+		Example:
+		    >>> list_data("folder123")
+		    {
+				"status": 200,
+				"msg": "OK",
+				"result": {
+					"folders": [
+					    {
+						    "id": "B-qlJkdHFeo",
+						    "name": "Subfolder"
+					    }
+					],
+					"files": [
+					    {
+						    "name": "MyMinecraftLetsPlay.mp4",
+							"size": 7040842,
+							"link": "https://streamtape.com/v/rbAarvRPXdYbaxY/MyMinecraftLetsPlay.mp4",
+							"created_at": 1585532987430,
+							"downloads": 0,
+							"linkid": "rbAarvRPXdYbaxY",
+							"convert": "converted"
+					    }
+					]
+				}
+			}
+		"""
+		url = self.url_query(f"{self.parameter}/listfolder", query={
+			"folder": folder_id,
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return response["result"]
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def create_folder(self, folder_name: str, parent_folder: Optional[str] = None) -> dict:
+		"""
+		Creates a new folder with the given folder name and parent folder.
+
+		Args:
+		    - folder_name (str): The name of the folder to be created.
+		    - parent_folder (str, optional): The ID of the parent folder. Defaults to None.
+
+		Returns:
+		    - dict: A dictionary containing the folder ID if the folder is created successfully.
+		          If an error occurs, an error response dictionary is returned.
+
+		Raises:
+		    - ApiResponseError: If the API response status is not 200.
+
+		Example:
+		    >>> create_folder("New Folder", "12345")
+			{
+				"status": 200,
+				"msg": "OK",
+				"result": {
+				    "folderid": "LnvnE51P5gc"
+				}
+			}
+		"""
+		url = self.url_query(f"{self.parameter}/createfolder", query={
+			"name": folder_name,
+			"pid" : parent_folder,
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return {
+				"folderid": response["result"].get("folderid")
+			}
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def rename_folder(self, folder_name: str, parent_folder: str) -> Union[dict, bool]:
+		"""
+		Renames a folder with the given folder_name and moves it to the specified parent_folder.
+
+		Args:
+		    - folder_name (str): The name of the folder to be renamed.
+		    - parent_folder (str): The name of the parent folder where the renamed folder will be moved.
+
+		Returns:
+		    - Union[dict, bool]: Returns a boolean value indicating the success of the renaming operation if the response status is 200.
+		                       Otherwise, returns an error response as a dictionary using the ApiResponse.error_response method.
+
+		Raises:
+		    - ApiResponseError: If the API response status is not 200.
+		"""
+		url = self.url_query(f"{self.parameter}/renamefolder", query={
+			"name"  : folder_name,
+			"folder": parent_folder,
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return bool(response["result"])
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def delete_folder(self, folder_id: str) -> Union[dict, bool]:
+		"""
+		Deletes a folder with the given folder_id.
+
+		Args:
+		    - folder_id (str): The ID of the folder to be deleted.
+
+		Returns:
+		    - Union[dict, bool]: Returns a boolean value indicating the success of the deletion operation if the response status is 200.
+		                       If the response status is not 200, returns an error response dictionary.
+
+		Raises:
+		    - ApiResponseError: If the API response status is not 200.
+
+		Example:
+		    >>> delete_folder("folder123")
+		    {
+				"status": 200,
+				"msg": "OK",
+				"result": true
+			}
+		"""
+		url = self.url_query(f"{self.parameter}/deletefolder", query={
+			"folder": folder_id,
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return bool(response["result"])
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def rename_file(self, file: str, name: str) -> Union[dict, bool]:
+		"""
+		Renames a file with the given name.
+
+		Args:
+		    - file (str): The name of the file to be renamed.
+		    - name (str): The new name for the file.
+
+		Returns:
+		    - Union[dict, bool]: Returns a dictionary containing the response result if the request is successful,
+		    otherwise returns a boolean value indicating the success of the request.
+
+		Raises:
+		    - ApiResponse: If the response status is not 200, an ApiResponse error response is raised.
+
+		Example:
+		    >>> obj = MyClass()
+		    >>> obj.rename_file("old_file.txt", "new_file.txt")
+		    {
+				"status": 200,
+				"msg": "OK",
+				"result": true
+			}
+		"""
+		url = self.url_query(f"{self.parameter}/deletefolder", query={
+			"file": file,
+			"name": name
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return bool(response["result"])
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def move_file(self, file_id: str, folder_id: str) -> Union[dict, bool]:
+		"""
+		Moves a file to a specified folder.
+
+		Args:
+		    - file_id (str): The ID of the file to be moved.
+		    - folder_id (str): The ID of the folder to which the file will be moved.
+
+		Returns:
+		    - Union[dict, bool]: Returns a boolean value indicating the success of the operation if the response status is 200.
+		                       Otherwise, returns an error response as a dictionary containing the status code and error message.
+
+		Raises:
+		    - ApiResponse: If the response status is not 200, an ApiResponse error response is raised.
+		"""
+		url = self.url_query(f"{self.parameter}/move", query={
+			"file"  : file_id,
+			"folder": folder_id
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return bool(response["result"])
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def delete_file(self, file_id: str) -> Union[dict, bool]:
+		"""
+		Deletes a file with the given file_id.
+
+		Args:
+		    - file_id (str): The ID of the file to be deleted.
+
+		Returns:
+		    - Union[dict, bool]: Returns a boolean value indicating the success of the deletion operation if the response status is 200.
+		                       If the response status is not 200, returns an error response dictionary.
+
+		Raises:
+		    - ApiResponse: If the response status is not 200, an ApiResponse error response is raised.
+
+		Example:
+		    >>> delete_file("file123")
+		    {
+				"status": 200,
+				"msg": "OK",
+				"result": true
+			}
+		"""
+		url = self.url_query(f"{self.parameter}/delete", query={
+			"file": file_id
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return bool(response["result"])
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
```

### Comparing `streamtape-1.0.1/streamtape/Remote.py` & `streamtape-1.0.2/streamtape/Remote.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-from typing import Optional, Union
-
-from streamtape.ApiResponse import ApiResponse
-from streamtape.BaseConfig import BaseConfig
-from streamtape.Stream import Stream
-
-
-class Remote(BaseConfig):
-	parameter: str = "remotedl"
-
-	def __init__(self, user: str, password: str):
-		super().__init__(user, password)
-
-	def remote_upload(self, file_url: str, folder: Optional[str], headers: Optional[dict], name: Optional[str]) -> dict:
-		"""
-		Uploads a file to a remote server.
-
-		Args:
-		    - file_url (str): The URL of the file to be uploaded.
-		    - folder (Optional[str]): The folder in which the file should be uploaded. Defaults to None.
-		    - headers (Optional[dict]): Additional headers to be included in the request. Defaults to an empty dictionary.
-		    - name (Optional[str]): The name of the file. Defaults to None.
-
-		Returns:
-		    - dict: A dictionary containing the ID of the uploaded file, the ID of the folder it belongs to, and the file information.
-
-		Raises:
-		    - ApiResponse: If the response status is not 200, an error response is returned.
-
-		"""
-		url = self.url_query(f"{self.parameter}/add", {
-			"url"    : file_url,
-			"folder" : folder or None,
-			"headers": headers or {},
-			"name"   : name or None
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			stream = Stream(self.api_user, self.api_password)
-			file_info = stream.file_info(response["result"].get('id'))
-			return {
-				"id"       : response["result"].get('id'),
-				"folderid" : response["result"].get('folderid'),
-				"file_info": file_info
-			}
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def remove(self, file_id: str) -> Union[bool, dict]:
-		"""
-		Removes a file with the given file_id from the server.
-
-		Args:
-		    - file_id (str): The ID of the file to be removed.
-
-		Returns:
-		    - Union[bool, dict]: Returns a boolean value indicating the success of the operation if the status code is 200.
-		                       Otherwise, returns an error response dictionary.
-
-		Raises:
-		    - ApiResponse: If the response status is not 200, an error response is returned.
-
-		Example:
-		    >>> remove("file123")  # Returns True if the file is successfully removed, otherwise returns an error response dictionary.
-		    {
-				"status": 200,
-				"msg": "OK",
-				"result": true
-			}
-		"""
-		url = self.url_query(f"{self.parameter}/remove", {
-			"id": file_id,
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return bool(response["result"])
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def check_remote_status(self, file_id: str) -> Union[dict, list]:
-		"""
-		Retrieves the status of a remote file with the given file ID.
-
-		Args:
-		    - self (object): The instance of the class.
-		    - file_id (str): The ID of the file to check the status for.
-
-		Returns:
-		    - Union[dict, list]: The status of the remote file. It can be either a dictionary or a list.
-
-		Raises:
-		    - ApiResponseError: If the API response status is not 200.
-
-		Example:
-		    >>> check_remote_status("12345")
-		    {
-				"status": 200,
-				"msg": "OK",
-				"result": {
-					"LnvnE51P5gc": {
-					    "id": "LnvnE51P5gc",
-					    "remoteurl": "https://vid.me/myvideo123",
-					    "status": "new",
-					    "bytes_loaded": null,
-					    "bytes_total": null,
-					    "folderid": "LnvnE51P5gc",
-					    "added": "2019-12-31 23:59:59",
-					    "last_update": "2019-12-31 23:59:59",
-					    "extid": false,
-					    "url": false
-					},
-				}
-			}
-		"""
-		url = self.url_query(f"{self.parameter}/status", {
-			"id": file_id,
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return response["result"]
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
+from typing import Optional, Union
+
+from streamtape.ApiResponse import ApiResponse
+from streamtape.BaseConfig import BaseConfig
+from streamtape.Stream import Stream
+
+
+class Remote(BaseConfig):
+	parameter: str = "remotedl"
+
+	def __init__(self, user: str, password: str):
+		super().__init__(user, password)
+
+	def remote_upload(self, file_url: str, folder: Optional[str], headers: Optional[dict], name: Optional[str]) -> dict:
+		"""
+		Uploads a file to a remote server.
+
+		Args:
+		    - file_url (str): The URL of the file to be uploaded.
+		    - folder (Optional[str]): The folder in which the file should be uploaded. Defaults to None.
+		    - headers (Optional[dict]): Additional headers to be included in the request. Defaults to an empty dictionary.
+		    - name (Optional[str]): The name of the file. Defaults to None.
+
+		Returns:
+		    - dict: A dictionary containing the ID of the uploaded file, the ID of the folder it belongs to, and the file information.
+
+		Raises:
+		    - ApiResponse: If the response status is not 200, an error response is returned.
+
+		"""
+		url = self.url_query(f"{self.parameter}/add", {
+			"url"    : file_url,
+			"folder" : folder or None,
+			"headers": headers or {},
+			"name"   : name or None
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			stream = Stream(self.api_user, self.api_password)
+			file_info = stream.file_info(response["result"].get('id'))
+			return {
+				"id"       : response["result"].get('id'),
+				"folderid" : response["result"].get('folderid'),
+				"file_info": file_info
+			}
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def remove(self, file_id: str) -> Union[bool, dict]:
+		"""
+		Removes a file with the given file_id from the server.
+
+		Args:
+		    - file_id (str): The ID of the file to be removed.
+
+		Returns:
+		    - Union[bool, dict]: Returns a boolean value indicating the success of the operation if the status code is 200.
+		                       Otherwise, returns an error response dictionary.
+
+		Raises:
+		    - ApiResponse: If the response status is not 200, an error response is returned.
+
+		Example:
+		    >>> remove("file123")  # Returns True if the file is successfully removed, otherwise returns an error response dictionary.
+		    {
+				"status": 200,
+				"msg": "OK",
+				"result": true
+			}
+		"""
+		url = self.url_query(f"{self.parameter}/remove", {
+			"id": file_id,
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return bool(response["result"])
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def check_remote_status(self, file_id: str) -> Union[dict, list]:
+		"""
+		Retrieves the status of a remote file with the given file ID.
+
+		Args:
+		    - self (object): The instance of the class.
+		    - file_id (str): The ID of the file to check the status for.
+
+		Returns:
+		    - Union[dict, list]: The status of the remote file. It can be either a dictionary or a list.
+
+		Raises:
+		    - ApiResponseError: If the API response status is not 200.
+
+		Example:
+		    >>> check_remote_status("12345")
+		    {
+				"status": 200,
+				"msg": "OK",
+				"result": {
+					"LnvnE51P5gc": {
+					    "id": "LnvnE51P5gc",
+					    "remoteurl": "https://vid.me/myvideo123",
+					    "status": "new",
+					    "bytes_loaded": null,
+					    "bytes_total": null,
+					    "folderid": "LnvnE51P5gc",
+					    "added": "2019-12-31 23:59:59",
+					    "last_update": "2019-12-31 23:59:59",
+					    "extid": false,
+					    "url": false
+					},
+				}
+			}
+		"""
+		url = self.url_query(f"{self.parameter}/status", {
+			"id": file_id,
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return response["result"]
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
```

### Comparing `streamtape-1.0.1/streamtape/Stream.py` & `streamtape-1.0.2/streamtape/Stream.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from streamtape.ApiResponse import ApiResponse
-from streamtape.BaseConfig import BaseConfig
-
-
-class Stream(BaseConfig):
-	parameter: str = "file"
-
-	def __init__(self, user: str, password: str):
-		super().__init__(user, password)
-
-	def dlticket(self, file_id: str) -> dict:
-		"""
-		Retrieves a download ticket for a given file ID.
-
-		Args:
-		    - file_id (str): The ID of the file for which to retrieve the download ticket.
-
-		Returns:
-		    - dict: A dictionary containing the download ticket information, including the ticket itself,
-		          the wait time in seconds, and the expiration date and time.
-
-		Raises:
-		    - ApiResponseError: If the API response status is not 200, indicating an error occurred.
-
-		"""
-		url = self.url_query(f"{self.parameter}/dlticket", {
-			"file": file_id
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return {
-				"ticket"     : response["result"].get('ticket'),
-				"wait_time"  : int(response["result"].get('wait_time')),
-				"valid_until": BaseConfig.str_to_datetime(response["result"].get('valid_until')),
-			}
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def download_link(self, file_id: str) -> dict:
-		"""
-		Downloads a file from the server using the provided file ID.
-
-		Args:
-		    - file_id (str): The ID of the file to be downloaded.
-
-		Returns:
-		    - dict: A dictionary containing the name, size, and URL of the downloaded file.
-
-		Raises:
-		    - ApiResponseError: If the server returns an error response.
-
-		"""
-		dl_ticket = self.dlticket(file_id)
-		url = self.url_query(f"{self.parameter}/dl", {
-			"file"  : file_id,
-			"ticket": dl_ticket
-		}, use_login=False)
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return {
-				"name": response["result"].get('name'),
-				"size": int(response["result"].get('size')),
-				"url" : response["result"].get('url'),
-			}
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
-
-	def file_info(self, file_id: list) -> dict:
-		"""
-		Retrieves information about the specified files.
-
-		Args:
-		    - file_id (list): A list of file IDs for which information needs to be retrieved.
-
-		Returns:
-		    - dict: A dictionary containing the information about the files.
-
-		Raises:
-		    - ApiResponseError: If the API response status is not 200.
-		"""
-		url = self.url_query(f"{self.parameter}/info", {
-			"file": ','.join(file_id),
-		})
-		response = BaseConfig.send_request(url)
-
-		if response["status"] == 200:
-			return response["result"]
-		else:
-			return ApiResponse.error_response(response["status"], response["msg"])
+from streamtape.ApiResponse import ApiResponse
+from streamtape.BaseConfig import BaseConfig
+
+
+class Stream(BaseConfig):
+	parameter: str = "file"
+
+	def __init__(self, user: str, password: str):
+		super().__init__(user, password)
+
+	def dlticket(self, file_id: str) -> dict:
+		"""
+		Retrieves a download ticket for a given file ID.
+
+		Args:
+		    - file_id (str): The ID of the file for which to retrieve the download ticket.
+
+		Returns:
+		    - dict: A dictionary containing the download ticket information, including the ticket itself,
+		          the wait time in seconds, and the expiration date and time.
+
+		Raises:
+		    - ApiResponseError: If the API response status is not 200, indicating an error occurred.
+
+		"""
+		url = self.url_query(f"{self.parameter}/dlticket", {
+			"file": file_id
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return {
+				"ticket"     : response["result"].get('ticket'),
+				"wait_time"  : int(response["result"].get('wait_time')),
+				"valid_until": BaseConfig.str_to_datetime(response["result"].get('valid_until')),
+			}
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def download_link(self, file_id: str) -> dict:
+		"""
+		Downloads a file from the server using the provided file ID.
+
+		Args:
+		    - file_id (str): The ID of the file to be downloaded.
+
+		Returns:
+		    - dict: A dictionary containing the name, size, and URL of the downloaded file.
+
+		Raises:
+		    - ApiResponseError: If the server returns an error response.
+
+		"""
+		dl_ticket = self.dlticket(file_id)
+		url = self.url_query(f"{self.parameter}/dl", {
+			"file"  : file_id,
+			"ticket": dl_ticket
+		}, use_login=False)
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return {
+				"name": response["result"].get('name'),
+				"size": int(response["result"].get('size')),
+				"url" : response["result"].get('url'),
+			}
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
+
+	def file_info(self, file_id: list) -> dict:
+		"""
+		Retrieves information about the specified files.
+
+		Args:
+		    - file_id (list): A list of file IDs for which information needs to be retrieved.
+
+		Returns:
+		    - dict: A dictionary containing the information about the files.
+
+		Raises:
+		    - ApiResponseError: If the API response status is not 200.
+		"""
+		url = self.url_query(f"{self.parameter}/info", {
+			"file": ','.join(file_id),
+		})
+		response = BaseConfig.send_request(url)
+
+		if response["status"] == 200:
+			return response["result"]
+		else:
+			return ApiResponse.error_response(response["status"], response["msg"])
```

### Comparing `streamtape-1.0.1/streamtape.egg-info/PKG-INFO` & `streamtape-1.0.2/streamtape.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,122 @@
-Metadata-Version: 2.1
-Name: streamtape
-Version: 1.0.1
-Summary: Unofficial python api wrapper from https://streamtape.com
-Home-page: https://github.com/DevCraftClub/StreamTape
-Author: Maxim Harder
-Author-email: dev@devcraft.club
-Keywords: api streamtape stream video hosting unlimited
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Unofficial StreamTape API wrapper
-
-It is a simple API wrapper for the streaming service streamtape.com. The API documentation can be found on the [docs page](https://devcraftclub.github.io/StreamTape/). The whole structure of the API has been split into different classes for easy overview and usage.
-
-## Installation
-
-Install with
-
-```python3
-pip install streamtape
-```
-
-## Usage
-
-### General usage
-
-Every class starts with following initialization:
-
-```python3
-my_var = selectedClass(API_USER_KEY, API_PASSWORD)
-```
-
-API key and password you can get in your account in **[Account Settings](https://streamtape.com/accpanel#accsettings)**.
-
-### General response
-
-For the general purpose of any response, the ApiResponse class has been created to return a dict with this structure:
-
-```json
-{
-    "status": <status-code>,
-    "msg": "<informational message. might vary, use the status code in your code!>",
-    "result": <result of the request. varies depending on the request>
-}
-```
-
-### Account
-
-Example
-
-```python
-account = Account(API_USER_KEY, API_PASSWORD)
-print(account.get_info())
-```
-
-### Convertation
-
-Example
-
-```python
-converts = Convertation(API_USER_KEY, API_PASSWORD)
-print(converts.list_converts())
-```
-
-### FileManager
-
-Class for working with files and folders
-
-Example
-
-```python
-f_manager = FileManager(API_USER_KEY, API_PASSWORD)
-print(f_manager.list_data())
-```
-
-### Remote
-
-Example
-
-```python
-remote = Remote(API_USER_KEY, API_PASSWORD)
-print(remote.remote_upload("path_to_file", "folder_id"))
-```
-
-### Stream
-
-Example
-
-```python
-stream = Stream(API_USER_KEY, API_PASSWORD)
-print(stream.file_info("file_id"))
-```
-
-### Upload
-
-Example
-
-```python
-uploader = Upload(API_USER_KEY, API_PASSWORD)
-print(uploader.upload("path_to_file", "folder_id"))
-```
-
-## Changelog
-
-### 1.0.0
-
-- Initial release   
-
-### 1.0.1
-
-- Fixed variables
-- Fixed upload parameters
+Metadata-Version: 2.1
+Name: streamtape
+Version: 1.0.2
+Summary: Unofficial python api wrapper from https://streamtape.come
+Home-page: https://github.com/DevCraftClub/StreamTape
+Author-email: Maxim Harder <dev@devcraft.club>
+Project-URL: Homepage, https://github.com/DevCraftClub/StreamTape
+Project-URL: Issues, https://github.com/DevCraftClub/StreamTape/issues
+Project-URL: Docs, https://devcraftclub.github.io/StreamTape/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Unofficial StreamTape API wrapper
+
+It is a simple API wrapper for the streaming service streamtape.com. The API documentation can be found on the [docs page](https://devcraftclub.github.io/StreamTape/). The whole structure of the API has been split into different classes for easy overview and usage.
+
+## Installation
+
+Install with
+
+```python3
+pip install streamtape
+```
+
+## Usage
+
+### General usage
+
+Every class starts with following initialization:
+
+```python3
+my_var = selectedClass(API_USER_KEY, API_PASSWORD)
+```
+
+API key and password you can get in your account in **[Account Settings](https://streamtape.com/accpanel#accsettings)**.
+
+### General response
+
+For the general purpose of any response, the ApiResponse class has been created to return a dict with this structure:
+
+```json
+{
+    "status": <status-code>,
+    "msg": "<informational message. might vary, use the status code in your code!>",
+    "result": <result of the request. varies depending on the request>
+}
+```
+
+### Account
+
+Example
+
+```python
+account = Account(API_USER_KEY, API_PASSWORD)
+print(account.get_info())
+```
+
+### Convertation
+
+Example
+
+```python
+converts = Convertation(API_USER_KEY, API_PASSWORD)
+print(converts.list_converts())
+```
+
+### FileManager
+
+Class for working with files and folders
+
+Example
+
+```python
+f_manager = FileManager(API_USER_KEY, API_PASSWORD)
+print(f_manager.list_data())
+```
+
+### Remote
+
+Example
+
+```python
+remote = Remote(API_USER_KEY, API_PASSWORD)
+print(remote.remote_upload("path_to_file", "folder_id"))
+```
+
+### Stream
+
+Example
+
+```python
+stream = Stream(API_USER_KEY, API_PASSWORD)
+print(stream.file_info("file_id"))
+```
+
+### Upload
+
+Example
+
+```python
+uploader = Upload(API_USER_KEY, API_PASSWORD)
+print(uploader.upload("path_to_file", "folder_id"))
+```
+
+## Changelog
+
+### 1.0.0
+
+- Initial release
+
+### 1.0.1
+
+- Fixed variables
+- Fixed upload parameters
+
+### 1.0.2
+
+* Fixed API link (thx to @[Gairolarishav](https://github.com/Gairolarishav))
```

