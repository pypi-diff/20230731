# Comparing `tmp/decentralizedroutines-2.0.7.tar.gz` & `tmp/decentralizedroutines-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decentralizedroutines-2.0.7.tar", last modified: Tue May  9 10:45:36 2023, max compression
+gzip compressed data, was "decentralizedroutines-2.2.0.tar", last modified: Mon Jul 31 11:20:48 2023, max compression
```

## Comparing `decentralizedroutines-2.0.7.tar` & `decentralizedroutines-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 10:45:36.382523 decentralizedroutines-2.0.7/
--rw-rw-rw-   0        0        0    35823 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.7/LICENSE
--rw-rw-rw-   0        0        0     1159 2023-05-09 10:45:36.383523 decentralizedroutines-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      505 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.7/README.md
--rw-rw-rw-   0        0        0      108 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      865 2023-05-09 10:45:36.384523 decentralizedroutines-2.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 10:45:36.363523 decentralizedroutines-2.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 10:45:36.373522 decentralizedroutines-2.0.7/src/decentralizedroutines/
--rw-rw-rw-   0        0        0    10305 2023-05-03 16:35:19.000000 decentralizedroutines-2.0.7/src/decentralizedroutines/RoutineScheduler.py
--rw-rw-rw-   0        0        0        0 2022-08-08 20:26:59.000000 decentralizedroutines-2.0.7/src/decentralizedroutines/__init__.py
--rw-rw-rw-   0        0        0      648 2022-12-19 22:11:23.000000 decentralizedroutines-2.0.7/src/decentralizedroutines/defaults.py
--rw-rw-rw-   0        0        0     1301 2023-01-16 18:07:39.000000 decentralizedroutines-2.0.7/src/decentralizedroutines/master.py
--rw-rw-rw-   0        0        0     1352 2023-02-28 18:56:12.000000 decentralizedroutines-2.0.7/src/decentralizedroutines/runroutines.py
--rw-rw-rw-   0        0        0     3367 2023-01-14 21:08:08.000000 decentralizedroutines-2.0.7/src/decentralizedroutines/schedule_sequence.py
--rw-rw-rw-   0        0        0     1982 2022-12-11 09:13:36.000000 decentralizedroutines-2.0.7/src/decentralizedroutines/update_version_requirements.py
--rw-rw-rw-   0        0        0     8934 2023-02-28 12:30:21.000000 decentralizedroutines-2.0.7/src/decentralizedroutines/worker.py
--rw-rw-rw-   0        0        0     9542 2023-02-27 10:18:30.000000 decentralizedroutines-2.0.7/src/decentralizedroutines/worker_lib.py
-drwxrwxrwx   0        0        0        0 2023-05-09 10:45:36.382523 decentralizedroutines-2.0.7/src/decentralizedroutines.egg-info/
--rw-rw-rw-   0        0        0     1159 2023-05-09 10:45:36.000000 decentralizedroutines-2.0.7/src/decentralizedroutines.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-05-09 10:45:36.000000 decentralizedroutines-2.0.7/src/decentralizedroutines.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 10:45:36.000000 decentralizedroutines-2.0.7/src/decentralizedroutines.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-09 10:45:36.000000 decentralizedroutines-2.0.7/src/decentralizedroutines.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-09 10:45:36.000000 decentralizedroutines-2.0.7/src/decentralizedroutines.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:20:48.365207 decentralizedroutines-2.2.0/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:20:48.365207 decentralizedroutines-2.2.0/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      487 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 11:20:48.365207 decentralizedroutines-2.2.0/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:20:48.361207 decentralizedroutines-2.2.0/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:20:48.361207 decentralizedroutines-2.2.0/src/decentralizedroutines/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10073 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/RoutineScheduler.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/__init__.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      625 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      623 2023-07-08 20:05:47.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/master.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1312 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/runroutines.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3281 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/schedule_sequence.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2149 2023-07-18 18:19:13.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/update_version_requirements.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8743 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/worker.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10328 2023-06-30 14:17:28.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/worker_lib.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:20:48.365207 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      665 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       45 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       22 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/top_level.txt
```

### Comparing `decentralizedroutines-2.0.7/LICENSE` & `decentralizedroutines-2.2.0/LICENSE`

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
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
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
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `decentralizedroutines-2.0.7/PKG-INFO` & `decentralizedroutines-2.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: decentralizedroutines
-Version: 2.0.7
-Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
-Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
-Author: Jose Carlito de Oliveira Filho
-Author-email: jcarlitooliveira@gmail.com
-Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# DecentralizedRoutines
-Decentralized routines orquestration through Kinesis working pool 
-
-### create virtual environment
-<ul>
-<li>enter command: pip -m venv venv</li>
-<li>activate virtual environnment (venv\Scripts\activate.bat)</li>
-</ul>
-
-## Create .env file in root folder Ie:
-<ul>
-<li>LOG_LEVEL=[DEBUG]</li>
-<li>GIT_USER=[GIT_USER]</li>
-<li>GIT_TOKEN=[GIT_TOKEN]</li>
-<li>GIT_ACRONYM=[GIT_ACRONYM]</li>
-<li>GIT_SERVER=[GIT_SERVER]</li>
-<li>SOURCE_FOLDER=[SOURCE_FOLDER]</li>
-</ul>
+Metadata-Version: 2.1
+Name: decentralizedroutines
+Version: 2.2.0
+Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
+Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
+Author: Jose Carlito de Oliveira Filho
+Author-email: jcarlitooliveira@gmail.com
+Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DecentralizedRoutines
+Decentralized routines orquestration through Kinesis working pool 
+
+### create virtual environment
+<ul>
+<li>enter command: pip -m venv venv</li>
+<li>activate virtual environnment (venv\Scripts\activate.bat)</li>
+</ul>
+
+## Create .env file in root folder Ie:
+<ul>
+<li>LOG_LEVEL=[DEBUG]</li>
+<li>GIT_USER=[GIT_USER]</li>
+<li>GIT_TOKEN=[GIT_TOKEN]</li>
+<li>GIT_ACRONYM=[GIT_ACRONYM]</li>
+<li>GIT_SERVER=[GIT_SERVER]</li>
+<li>SOURCE_FOLDER=[SOURCE_FOLDER]</li>
+</ul>
```

### Comparing `decentralizedroutines-2.0.7/setup.cfg` & `decentralizedroutines-2.2.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,52 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2064 6563 656e 7472 616c 697a 6564   = decentralized
-00000020: 726f 7574 696e 6573 0d0a 7665 7273 696f  routines..versio
-00000030: 6e20 3d20 322e 302e 370d 0a61 7574 686f  n = 2.0.7..autho
-00000040: 7220 3d20 4a6f 7365 2043 6172 6c69 746f  r = Jose Carlito
-00000050: 2064 6520 4f6c 6976 6569 7261 2046 696c   de Oliveira Fil
-00000060: 686f 0d0a 6175 7468 6f72 5f65 6d61 696c  ho..author_email
-00000070: 203d 206a 6361 726c 6974 6f6f 6c69 7665   = jcarlitoolive
-00000080: 6972 6140 676d 6169 6c2e 636f 6d0d 0a64  ira@gmail.com..d
-00000090: 6573 6372 6970 7469 6f6e 203d 204d 6173  escription = Mas
-000000a0: 7465 722f 576f 726b 6572 2069 6d70 6c65  ter/Worker imple
-000000b0: 6d65 6e74 6174 696f 6e20 6f66 2064 6563  mentation of dec
-000000c0: 656e 7472 616c 697a 6564 2067 6974 2070  entralized git p
-000000d0: 7562 6c69 7368 6564 2072 6f75 7469 6e65  ublished routine
-000000e0: 7320 616e 6420 6b69 6e65 7369 7320 776f  s and kinesis wo
-000000f0: 726b 6572 2070 6f6f 6c0d 0a6c 6f6e 675f  rker pool..long_
-00000100: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-00000110: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-00000120: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00000130: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000140: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
-00000150: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
-00000160: 7562 2e63 6f6d 2f6a 6361 726c 6974 6f6f  ub.com/jcarlitoo
-00000170: 6c69 7665 6972 612f 4465 6365 6e74 7261  liveira/Decentra
-00000180: 6c69 7a65 6452 6f75 7469 6e65 730d 0a70  lizedRoutines..p
-00000190: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-000001a0: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
-000001b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001c0: 6d2f 6a63 6172 6c69 746f 6f6c 6976 6569  m/jcarlitoolivei
-000001d0: 7261 2f44 6563 656e 7472 616c 697a 6564  ra/Decentralized
-000001e0: 526f 7574 696e 6573 2f69 7373 7565 730d  Routines/issues.
-000001f0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-00000200: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000220: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
-00000230: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000240: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-00000250: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-00000260: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000270: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
-00000280: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-00000290: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
-000002a0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-000002b0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-000002c0: 332e 390d 0a69 6e73 7461 6c6c 5f72 6571  3.9..install_req
-000002d0: 7569 7265 7320 3d20 0d0a 0973 6861 7265  uires = ...share
-000002e0: 6464 6174 613d 3d32 2e30 2e37 0d0a 0970  ddata==2.0.7...p
-000002f0: 7375 7469 6c3d 3d35 2e39 2e30 0d0a 0974  sutil==5.9.0...t
-00000300: 7a6c 6f63 616c 3d3d 342e 310d 0a0d 0a5b  zlocal==4.1....[
-00000310: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000320: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000330: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
-00000340: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000350: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000360: 0a                                       .
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6465 6365 6e74 7261 6c69 7a65 6472  = decentralizedr
+00000020: 6f75 7469 6e65 730a 7665 7273 696f 6e20  outines.version 
+00000030: 3d20 322e 322e 300a 6175 7468 6f72 203d  = 2.2.0.author =
+00000040: 204a 6f73 6520 4361 726c 6974 6f20 6465   Jose Carlito de
+00000050: 204f 6c69 7665 6972 6120 4669 6c68 6f0a   Oliveira Filho.
+00000060: 6175 7468 6f72 5f65 6d61 696c 203d 206a  author_email = j
+00000070: 6361 726c 6974 6f6f 6c69 7665 6972 6140  carlitooliveira@
+00000080: 676d 6169 6c2e 636f 6d0a 6465 7363 7269  gmail.com.descri
+00000090: 7074 696f 6e20 3d20 4d61 7374 6572 2f57  ption = Master/W
+000000a0: 6f72 6b65 7220 696d 706c 656d 656e 7461  orker implementa
+000000b0: 7469 6f6e 206f 6620 6465 6365 6e74 7261  tion of decentra
+000000c0: 6c69 7a65 6420 6769 7420 7075 626c 6973  lized git publis
+000000d0: 6865 6420 726f 7574 696e 6573 2061 6e64  hed routines and
+000000e0: 206b 696e 6573 6973 2077 6f72 6b65 7220   kinesis worker 
+000000f0: 706f 6f6c 0a6c 6f6e 675f 6465 7363 7269  pool.long_descri
+00000100: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
+00000110: 4144 4d45 2e6d 640a 6c6f 6e67 5f64 6573  ADME.md.long_des
+00000120: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+00000130: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+00000140: 6b64 6f77 6e0a 7572 6c20 3d20 6874 7470  kdown.url = http
+00000150: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00000160: 6361 726c 6974 6f6f 6c69 7665 6972 612f  carlitooliveira/
+00000170: 4465 6365 6e74 7261 6c69 7a65 6452 6f75  DecentralizedRou
+00000180: 7469 6e65 730a 7072 6f6a 6563 745f 7572  tines.project_ur
+00000190: 6c73 203d 200a 0942 7567 2054 7261 636b  ls = ..Bug Track
+000001a0: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
+000001b0: 6875 622e 636f 6d2f 6a63 6172 6c69 746f  hub.com/jcarlito
+000001c0: 6f6c 6976 6569 7261 2f44 6563 656e 7472  oliveira/Decentr
+000001d0: 616c 697a 6564 526f 7574 696e 6573 2f69  alizedRoutines/i
+000001e0: 7373 7565 730a 636c 6173 7369 6669 6572  ssues.classifier
+000001f0: 7320 3d20 0a09 5072 6f67 7261 6d6d 696e  s = ..Programmin
+00000200: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000210: 7468 6f6e 203a 3a20 330a 094c 6963 656e  thon :: 3..Licen
+00000220: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000230: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000240: 650a 094f 7065 7261 7469 6e67 2053 7973  e..Operating Sys
+00000250: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000260: 6e64 656e 740a 0a5b 6f70 7469 6f6e 735d  ndent..[options]
+00000270: 0a70 6163 6b61 6765 5f64 6972 203d 200a  .package_dir = .
+00000280: 093d 2073 7263 0a70 6163 6b61 6765 7320  .= src.packages 
+00000290: 3d20 6669 6e64 3a0a 7079 7468 6f6e 5f72  = find:.python_r
+000002a0: 6571 7569 7265 7320 3d20 3e3d 332e 390a  equires = >=3.9.
+000002b0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+000002c0: 203d 200a 0973 6861 7265 6464 6174 613d   = ..shareddata=
+000002d0: 3d32 2e32 2e30 0a09 7073 7574 696c 3d3d  =2.2.0..psutil==
+000002e0: 352e 392e 350a 0974 7a6c 6f63 616c 3d3d  5.9.5..tzlocal==
+000002f0: 342e 310a 0a5b 6f70 7469 6f6e 732e 7061  4.1..[options.pa
+00000300: 636b 6167 6573 2e66 696e 645d 0a77 6865  ckages.find].whe
+00000310: 7265 203d 2073 7263 0a0a 5b65 6767 5f69  re = src..[egg_i
+00000320: 6e66 6f5d 0a74 6167 5f62 7569 6c64 203d  nfo].tag_build =
+00000330: 200a 7461 675f 6461 7465 203d 2030 0a0a   .tag_date = 0..
```

### Comparing `decentralizedroutines-2.0.7/src/decentralizedroutines/RoutineScheduler.py` & `decentralizedroutines-2.2.0/src/decentralizedroutines/RoutineScheduler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-import os,glob,subprocess,pytz
-from pathlib import Path
-import pandas as pd
-import numpy as np
-from datetime import datetime
-from tzlocal import get_localzone 
-local_tz = pytz.timezone(str(get_localzone()))
-
-from SharedData.Metadata import Metadata
-from SharedData.Logger import Logger
-from SharedData.SharedDataAWSKinesis import KinesisLogStreamConsumer,KinesisStreamProducer
-
-class RoutineScheduler:
-
-    def __init__(self,stream_name):
-        self.consumer = KinesisLogStreamConsumer()
-        self.producer = KinesisStreamProducer(stream_name)
-
-    def LoadSchedule(self,schedule_name):
-        self.schedule=[]        
-
-        today = datetime.now().date()
-        year = today.timetuple()[0]
-        month = today.timetuple()[1]
-        day = today.timetuple()[2]        
-
-        _sched = Metadata('SCHEDULES/'+schedule_name).static.reset_index()
-        sched = pd.DataFrame()
-        for i,s in _sched.iterrows():
-            runtimes = s['Run Times'].split(',')
-            for t in runtimes:
-                hour = int(t.split(':')[0])
-                minute = int(t.split(':')[1])
-                dttm = local_tz.localize(datetime(year,month,day,hour,minute))
-                s['Run Times'] = dttm
-                sched = sched.reindex(columns=s.index.union(sched.columns))
-                sched = pd.concat([sched, pd.DataFrame(s).T])
-
-        sched = sched.sort_values(by=['Run Times','Name']).reset_index(drop=True)
-        sched['Status'] = np.nan
-        sched['Last Message'] = np.nan
-        sched['index'] = [s.lower().replace('\\','/') for s in sched['index']]
-        sched.loc[sched['Dependencies'].isnull(),'Dependencies'] = ''
-        sched['Dependencies'] = [s.lower().replace('\\','/') for s in sched['Dependencies']]
-
-
-        uruntimes = sched['Run Times'].unique()
-        runtime = uruntimes[0]
-        sched_sort = pd.DataFrame(columns=sched.columns)
-        for runtime in uruntimes:
-            # mark pending routines
-            while True:
-                idx = runtime.astimezone(tz=local_tz)>=sched['Run Times']
-                idx = (idx) & ((sched['Status'].isnull()) | (sched['Status']=='WAITING DEPENDENCIES'))
-
-                dfpending = sched[idx]
-                expiredidx = dfpending.duplicated(['Computer','Script'],keep='last')
-                if expiredidx.any():
-                    expiredids = expiredidx.index[expiredidx]
-                    sched.loc[expiredids,'Status'] = 'EXPIRED'
-                dfpending = dfpending[~expiredidx]
-                i=0
-                for i in dfpending.index:
-                    r = dfpending.loc[i]
-                    if (not str(r['Dependencies'])=='') & (not str(r['Dependencies'])=='nan'):
-                        run=True
-                        sched.loc[i,'Status'] = 'WAITING DEPENDENCIES'
-                        dependencies = r['Dependencies'].replace('\n','').split(',')                
-                        for dep in dependencies:                            
-                            idx = sched['index']==dep
-                            idx = (idx) & (sched['Run Times']<=runtime.astimezone(tz=local_tz))                            
-                            ids = sched.index[idx]
-                            if len(ids)==0:
-                                # Logger.log.info('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
-                                Logger.log.error('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
-                                raise Exception('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
-                            else:
-                                if not str(sched.loc[ids[-1],'Status']) == 'COMPLETED':
-                                    run=False
-                        if run:
-                            sched.loc[i,'Status'] = 'PENDING'
-                    else:
-                        sched.loc[i,'Status'] = 'PENDING'
-
-                idx = sched['Status']=='PENDING'
-                if idx.any():
-                    sched_sort = pd.concat([sched_sort, sched[idx]])
-                    sched_sort['Status'] = np.nan
-                    sched.loc[idx,'Status'] = 'COMPLETED'
-                else:
-                    break
-
-        self.schedule = sched_sort
-        return sched_sort
-
-    def UpdateRoutinesStatus(self):
-        sched = self.schedule                
-        local_tz = pytz.timezone(str(get_localzone()))
-        # RefreshLogs
-        dflogs = self.consumer.readLogs()
-        if not dflogs.empty:
-            dflogs['index'] = dflogs['user_name']+':'+dflogs['logger_name']
-            dflogs['index'] = [s.lower().replace('\\','/') for s in dflogs['index']]
-
-            dflogs = dflogs[dflogs['asctime'].notnull()].copy()
-            dflogs['asctime'] = pd.to_datetime(dflogs['asctime'])
-            dflogs['asctime'] = [dt.astimezone(tz=local_tz) for dt in dflogs['asctime']]
-
-            i=0
-            for i in sched.index:
-                r = sched.loc[i]
-                idx = dflogs['index']==r['index']
-                idx = (idx) & (dflogs['asctime']>=r['Run Times'])    
-                if np.any(idx):    
-                    sched.loc[i,'Last Message'] = dflogs[idx].iloc[-1]['message']   
-
-                                
-            dferr = dflogs[dflogs['message']=='ROUTINE ERROR!']
-            dferr = dferr.reset_index(drop=True).sort_values(by='asctime')
-            i=0
-            for i in dferr.index:
-                r = dferr.iloc[i]
-                idx = sched['index']==r['index']
-                idx = (idx) & (r['asctime']>=sched['Run Times'])
-                if idx.any():
-                    ids = idx[::-1].idxmax()
-                    sched.loc[ids,'Status'] = 'ERROR'
-                    idx = sched.loc[idx,'Status'].isnull()
-                    idx = idx.index[idx]
-                    sched.loc[idx,'Status'] = 'EXPIRED'
-
-            compl = dflogs[dflogs['message']=='ROUTINE COMPLETED!'].reset_index(drop=True).sort_values(by='asctime')
-            i=0
-            for i in compl.index:
-                r = compl.iloc[i]
-                idx = sched['index']==r['index']                
-                idx = (idx) & (r['asctime']>=sched['Run Times'])
-                if idx.any():
-                    ids = idx[::-1].idxmax()
-                    sched.loc[ids,'Status'] = 'COMPLETED'
-                    idx = sched.loc[idx,'Status'].isnull()
-                    idx = idx.index[idx]
-                    sched.loc[idx,'Status'] = 'EXPIRED'
-
-        # mark pending routines
-        idx = datetime.now().astimezone(tz=local_tz)>=sched['Run Times']
-        idx = (idx) & ((sched['Status'].isnull()) | (sched['Status']=='WAITING DEPENDENCIES'))
-        
-        dfpending = sched[idx]
-        expiredidx = dfpending.duplicated(['Computer','Script'],keep='last')
-        if expiredidx.any():
-            expiredids = expiredidx.index[expiredidx]
-            sched.loc[expiredids,'Status'] = 'EXPIRED'
-        
-        dfpending = dfpending[~expiredidx]
-        for i in dfpending.index:
-            r = dfpending.loc[i]
-            if (not str(r['Dependencies'])=='') & (not str(r['Dependencies'])=='nan'):
-                run=True
-                sched.loc[i,'Status'] = 'WAITING DEPENDENCIES'
-                dependencies = r['Dependencies'].replace('\n','').split(',')                
-                for dep in dependencies:                    
-                    idx = sched['index']==dep                    
-                    idx = (idx) & (sched['Run Times']<=datetime.now().astimezone(tz=local_tz))
-                    ids = sched.index[idx]
-                    if len(ids)==0:                        
-                        Logger.log.error('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
-                    else:
-                        if not str(sched.loc[ids[-1],'Status']) == 'COMPLETED':
-                            run=False
-                if run:
-                    if sched.loc[i,'Run']:
-                        sched.loc[i,'Status'] = 'PENDING'
-                    else:
-                        sched.loc[i,'Status'] = 'PENDING EXTERNAL'
-            else:
-                if sched.loc[i,'Run']:
-                        sched.loc[i,'Status'] = 'PENDING'
-                else:
-                    sched.loc[i,'Status'] = 'PENDING EXTERNAL'                
-        
-        self.schedule=sched
-        return sched
-
-    def RunPendingRoutines(self):   
-        sched = self.schedule
-        
-        # Run pending routines
-        dfpending = sched[sched['Status']=='PENDING']
-
-        for i in dfpending.index:
-            r = dfpending.loc[i].copy()
-            if str(r['Last Message'])=='nan':
-                target = r['Computer']
-                
-                if '#' in r['Script']: # has branch
-                    branch = r['Script'].split('\\')[0].split('#')[-1]
-                    repo = r['Script'].split('\\')[0].split('#')[0]
-                    routine = r['Script'].replace(repo,'').\
-                        replace('#','').replace(branch,'')[1:]+'.py'
-                else:
-                    branch=''
-                    repo = r['Script'].split('\\')[0]
-                    routine = r['Script'].replace(repo,'')[1:]+'.py'
-                                    
-                data = {
-                    "sender" : "MASTER",
-                    "job" : "routine",
-                    "target" : target,        
-                    "repo" : repo,
-                    "routine" : routine
-                }
-                if branch != '':                    
-                    data['branch']=branch
-
-                if 'args' in r:
-                    r['args'] = str(r['args'])
-                    if (r['args']!='') & (r['args']!='nan'):
-                        data['args']=r['args']
-
-                self.producer.produce(data,'command')
-                sched.loc[r.name,'Status'] = 'RUNNING'
-                Logger.log.info('Command to run %s:%s sent!' % (target,r['Script']))
-        
-        self.schedule = sched
-        return sched
-
-
-
+import os,glob,subprocess,pytz
+from pathlib import Path
+import pandas as pd
+import numpy as np
+from datetime import datetime
+from tzlocal import get_localzone 
+local_tz = pytz.timezone(str(get_localzone()))
+
+from SharedData.Metadata import Metadata
+from SharedData.Logger import Logger
+from SharedData.SharedDataAWSKinesis import KinesisLogStreamConsumer,KinesisStreamProducer
+
+class RoutineScheduler:
+
+    def __init__(self,stream_name):
+        self.consumer = KinesisLogStreamConsumer()
+        self.producer = KinesisStreamProducer(stream_name)
+
+    def LoadSchedule(self,schedule_name):
+        self.schedule=[]        
+
+        today = datetime.now().date()
+        year = today.timetuple()[0]
+        month = today.timetuple()[1]
+        day = today.timetuple()[2]        
+
+        _sched = Metadata('SCHEDULES/'+schedule_name).static.reset_index()
+        sched = pd.DataFrame()
+        for i,s in _sched.iterrows():
+            runtimes = s['Run Times'].split(',')
+            for t in runtimes:
+                hour = int(t.split(':')[0])
+                minute = int(t.split(':')[1])
+                dttm = local_tz.localize(datetime(year,month,day,hour,minute))
+                s['Run Times'] = dttm
+                sched = sched.reindex(columns=s.index.union(sched.columns))
+                sched = pd.concat([sched, pd.DataFrame(s).T])
+
+        sched = sched.sort_values(by=['Run Times','Name']).reset_index(drop=True)
+        sched['Status'] = np.nan
+        sched['Last Message'] = np.nan
+        sched['index'] = [s.lower().replace('\\','/') for s in sched['index']]
+        sched.loc[sched['Dependencies'].isnull(),'Dependencies'] = ''
+        sched['Dependencies'] = [s.lower().replace('\\','/') for s in sched['Dependencies']]
+
+
+        uruntimes = sched['Run Times'].unique()
+        runtime = uruntimes[0]
+        sched_sort = pd.DataFrame(columns=sched.columns)
+        for runtime in uruntimes:
+            # mark pending routines
+            while True:
+                idx = runtime.astimezone(tz=local_tz)>=sched['Run Times']
+                idx = (idx) & ((sched['Status'].isnull()) | (sched['Status']=='WAITING DEPENDENCIES'))
+
+                dfpending = sched[idx]
+                expiredidx = dfpending.duplicated(['Computer','Script'],keep='last')
+                if expiredidx.any():
+                    expiredids = expiredidx.index[expiredidx]
+                    sched.loc[expiredids,'Status'] = 'EXPIRED'
+                dfpending = dfpending[~expiredidx]
+                i=0
+                for i in dfpending.index:
+                    r = dfpending.loc[i]
+                    if (not str(r['Dependencies'])=='') & (not str(r['Dependencies'])=='nan'):
+                        run=True
+                        sched.loc[i,'Status'] = 'WAITING DEPENDENCIES'
+                        dependencies = r['Dependencies'].replace('\n','').split(',')                
+                        for dep in dependencies:                            
+                            idx = sched['index']==dep
+                            idx = (idx) & (sched['Run Times']<=runtime.astimezone(tz=local_tz))                            
+                            ids = sched.index[idx]
+                            if len(ids)==0:
+                                # Logger.log.info('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
+                                Logger.log.error('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
+                                raise Exception('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
+                            else:
+                                if not str(sched.loc[ids[-1],'Status']) == 'COMPLETED':
+                                    run=False
+                        if run:
+                            sched.loc[i,'Status'] = 'PENDING'
+                    else:
+                        sched.loc[i,'Status'] = 'PENDING'
+
+                idx = sched['Status']=='PENDING'
+                if idx.any():
+                    sched_sort = pd.concat([sched_sort, sched[idx]])
+                    sched_sort['Status'] = np.nan
+                    sched.loc[idx,'Status'] = 'COMPLETED'
+                else:
+                    break
+
+        self.schedule = sched_sort
+        return sched_sort
+
+    def UpdateRoutinesStatus(self):
+        sched = self.schedule                
+        local_tz = pytz.timezone(str(get_localzone()))
+        # RefreshLogs
+        dflogs = self.consumer.readLogs()
+        if not dflogs.empty:
+            dflogs['index'] = dflogs['user_name']+':'+dflogs['logger_name']
+            dflogs['index'] = [s.lower().replace('\\','/') for s in dflogs['index']]
+
+            dflogs = dflogs[dflogs['asctime'].notnull()].copy()
+            dflogs['asctime'] = pd.to_datetime(dflogs['asctime'])
+            dflogs['asctime'] = [dt.astimezone(tz=local_tz) for dt in dflogs['asctime']]
+
+            i=0
+            for i in sched.index:
+                r = sched.loc[i]
+                idx = dflogs['index']==r['index']
+                idx = (idx) & (dflogs['asctime']>=r['Run Times'])    
+                if np.any(idx):    
+                    sched.loc[i,'Last Message'] = dflogs[idx].iloc[-1]['message']   
+
+                                
+            dferr = dflogs[dflogs['message']=='ROUTINE ERROR!']
+            dferr = dferr.reset_index(drop=True).sort_values(by='asctime')
+            i=0
+            for i in dferr.index:
+                r = dferr.iloc[i]
+                idx = sched['index']==r['index']
+                idx = (idx) & (r['asctime']>=sched['Run Times'])
+                if idx.any():
+                    ids = idx[::-1].idxmax()
+                    sched.loc[ids,'Status'] = 'ERROR'
+                    idx = sched.loc[idx,'Status'].isnull()
+                    idx = idx.index[idx]
+                    sched.loc[idx,'Status'] = 'EXPIRED'
+
+            compl = dflogs[dflogs['message']=='ROUTINE COMPLETED!'].reset_index(drop=True).sort_values(by='asctime')
+            i=0
+            for i in compl.index:
+                r = compl.iloc[i]
+                idx = sched['index']==r['index']                
+                idx = (idx) & (r['asctime']>=sched['Run Times'])
+                if idx.any():
+                    ids = idx[::-1].idxmax()
+                    sched.loc[ids,'Status'] = 'COMPLETED'
+                    idx = sched.loc[idx,'Status'].isnull()
+                    idx = idx.index[idx]
+                    sched.loc[idx,'Status'] = 'EXPIRED'
+
+        # mark pending routines
+        idx = datetime.now().astimezone(tz=local_tz)>=sched['Run Times']
+        idx = (idx) & ((sched['Status'].isnull()) | (sched['Status']=='WAITING DEPENDENCIES'))
+        
+        dfpending = sched[idx]
+        expiredidx = dfpending.duplicated(['Computer','Script'],keep='last')
+        if expiredidx.any():
+            expiredids = expiredidx.index[expiredidx]
+            sched.loc[expiredids,'Status'] = 'EXPIRED'
+        
+        dfpending = dfpending[~expiredidx]
+        for i in dfpending.index:
+            r = dfpending.loc[i]
+            if (not str(r['Dependencies'])=='') & (not str(r['Dependencies'])=='nan'):
+                run=True
+                sched.loc[i,'Status'] = 'WAITING DEPENDENCIES'
+                dependencies = r['Dependencies'].replace('\n','').split(',')                
+                for dep in dependencies:                    
+                    idx = sched['index']==dep                    
+                    idx = (idx) & (sched['Run Times']<=datetime.now().astimezone(tz=local_tz))
+                    ids = sched.index[idx]
+                    if len(ids)==0:                        
+                        Logger.log.error('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
+                    else:
+                        if not str(sched.loc[ids[-1],'Status']) == 'COMPLETED':
+                            run=False
+                if run:
+                    if sched.loc[i,'Run']:
+                        sched.loc[i,'Status'] = 'PENDING'
+                    else:
+                        sched.loc[i,'Status'] = 'PENDING EXTERNAL'
+            else:
+                if sched.loc[i,'Run']:
+                        sched.loc[i,'Status'] = 'PENDING'
+                else:
+                    sched.loc[i,'Status'] = 'PENDING EXTERNAL'                
+        
+        self.schedule=sched
+        return sched
+
+    def RunPendingRoutines(self):   
+        sched = self.schedule
+        
+        # Run pending routines
+        dfpending = sched[sched['Status']=='PENDING']
+
+        for i in dfpending.index:
+            r = dfpending.loc[i].copy()
+            if str(r['Last Message'])=='nan':
+                target = r['Computer']
+                
+                if '#' in r['Script']: # has branch
+                    branch = r['Script'].split('/')[0].split('#')[-1]
+                    repo = r['Script'].split('/')[0].split('#')[0]
+                    routine = r['Script'].replace(repo,'').\
+                        replace('#','').replace(branch,'')[1:]+'.py'
+                else:
+                    branch=''
+                    repo = r['Script'].split('/')[0]
+                    routine = r['Script'].replace(repo,'')[1:]+'.py'
+                                    
+                data = {
+                    "sender" : "MASTER",
+                    "job" : "routine",
+                    "target" : target,        
+                    "repo" : repo,
+                    "routine" : routine
+                }
+                if branch != '':                    
+                    data['branch']=branch
+
+                if 'args' in r:
+                    r['args'] = str(r['args'])
+                    if (r['args']!='') & (r['args']!='nan'):
+                        data['args']=r['args']
+
+                self.producer.produce(data,'command')
+                sched.loc[r.name,'Status'] = 'RUNNING'
+                Logger.log.info('Command to run %s:%s sent!' % (target,r['Script']))
+        
+        self.schedule = sched
+        return sched
+
+
+
```

### Comparing `decentralizedroutines-2.0.7/src/decentralizedroutines/defaults.py` & `decentralizedroutines-2.2.0/src/decentralizedroutines/defaults.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import os
-from dotenv import load_dotenv
-
-load_dotenv()  # take environment variables from .env.
-
-if not 'GIT_PROTOCOL' in os.environ:
-    os.environ['GIT_PROTOCOL'] = 'https'
-
-if not 'GIT_SERVER' in os.environ:
-    os.environ['GIT_SERVER']='github.com'
-
-if not 'SOURCE_FOLDER' in os.environ:
-    os.environ['SOURCE_FOLDER'] = os.environ['USERPROFILE']+'\\src\\'
-
-if not 'SLEEP_TIME' in os.environ:
-    os.environ['SLEEP_TIME'] = '5'
-
-if not 'WORKERPOOL_STREAM' in os.environ:
-    os.environ['WORKERPOOL_STREAM'] = 'deepportfolio-workerpool'
-
-os.environ['USER_COMPUTER'] = os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME']
+import os
+from dotenv import load_dotenv
+
+load_dotenv()  # take environment variables from .env.
+
+if not 'GIT_PROTOCOL' in os.environ:
+    os.environ['GIT_PROTOCOL'] = 'https'
+
+if not 'GIT_SERVER' in os.environ:
+    os.environ['GIT_SERVER']='github.com'
+
+if not 'SOURCE_FOLDER' in os.environ:
+    os.environ['SOURCE_FOLDER'] = os.environ['USERPROFILE']+'/src/'
+
+if not 'SLEEP_TIME' in os.environ:
+    os.environ['SLEEP_TIME'] = '5'
+
+if not 'WORKERPOOL_STREAM' in os.environ:
+    os.environ['WORKERPOOL_STREAM'] = 'deepportfolio-workerpool'
+
+os.environ['USER_COMPUTER'] = os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME']
```

### Comparing `decentralizedroutines-2.0.7/src/decentralizedroutines/runroutines.py` & `decentralizedroutines-2.2.0/src/decentralizedroutines/runroutines.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# PROPRIETARY LIBS
-import os,sys,time
-from decentralizedroutines.RoutineScheduler import RoutineScheduler
-from datetime import datetime
-
-import decentralizedroutines.defaults as defaults 
-from SharedData.Logger import Logger
-logger = Logger(__file__,'master')
-from SharedData.SharedDataAWSKinesis import KinesisStreamConsumer,KinesisStreamProducer
-
-
-if len(sys.argv)>=2:
-    SCHEDULE_NAME = str(sys.argv[1])
-else:
-    Logger.log.error('SCHEDULE_NAME not provided, please specify!')
-    raise Exception('SCHEDULE_NAME not provided, please specify!')
-
-Logger.log.info('Routine schedule starting for %s...' % (SCHEDULE_NAME))
-
-stream_name=os.environ['WORKERPOOL_STREAM']
-producer = KinesisStreamProducer(stream_name)
-
-sched = RoutineScheduler(stream_name)
-sched.LoadSchedule(SCHEDULE_NAME)
-sched.UpdateRoutinesStatus()
-
-Logger.log.info('Routine schedule STARTED!')
-#time.sleep(15)
-while(True):
-    print('',end='\r')
-    print('Running Schedule %s' % (str(datetime.now())),end='')
-    if sched.schedule['Run Times'][0].date()<datetime.now().date():
-        print('')
-        print('Reloading Schedule %s' % (str(datetime.now())))
-        print('')
-        sched.LoadSchedule(SCHEDULE_NAME)
-        sched.UpdateRoutinesStatus()
-
-    sched.UpdateRoutinesStatus()
-    sched.RunPendingRoutines()    
+# PROPRIETARY LIBS
+import os,sys,time
+from decentralizedroutines.RoutineScheduler import RoutineScheduler
+from datetime import datetime
+
+import decentralizedroutines.defaults as defaults 
+from SharedData.Logger import Logger
+logger = Logger(__file__,'master')
+from SharedData.SharedDataAWSKinesis import KinesisStreamConsumer,KinesisStreamProducer
+
+
+if len(sys.argv)>=2:
+    SCHEDULE_NAME = str(sys.argv[1])
+else:
+    Logger.log.error('SCHEDULE_NAME not provided, please specify!')
+    raise Exception('SCHEDULE_NAME not provided, please specify!')
+
+Logger.log.info('Routine schedule starting for %s...' % (SCHEDULE_NAME))
+
+stream_name=os.environ['WORKERPOOL_STREAM']
+producer = KinesisStreamProducer(stream_name)
+
+sched = RoutineScheduler(stream_name)
+sched.LoadSchedule(SCHEDULE_NAME)
+sched.UpdateRoutinesStatus()
+
+Logger.log.info('Routine schedule STARTED!')
+#time.sleep(15)
+while(True):
+    print('',end='\r')
+    print('Running Schedule %s' % (str(datetime.now())),end='')
+    if sched.schedule['Run Times'][0].date()<datetime.now().date():
+        print('')
+        print('Reloading Schedule %s' % (str(datetime.now())))
+        print('')
+        sched.LoadSchedule(SCHEDULE_NAME)
+        sched.UpdateRoutinesStatus()
+
+    sched.UpdateRoutinesStatus()
+    sched.RunPendingRoutines()    
     time.sleep(15)
```

### Comparing `decentralizedroutines-2.0.7/src/decentralizedroutines/schedule_sequence.py` & `decentralizedroutines-2.2.0/src/decentralizedroutines/schedule_sequence.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from datetime import datetime
-import pandas as pd
-import numpy as np
-import pytz
-from tzlocal import get_localzone 
-local_tz = pytz.timezone(str(get_localzone()))
-
-from SharedData.Logger import Logger
-logger = Logger(__file__,user='guest')
-from SharedData.Metadata import Metadata
-from SharedData.SharedDataAWSKinesis import KinesisLogStreamConsumer
-
-schedule_name = 'SCHEDULES/TRADEBOT06'
-today = datetime.now().date()
-year = today.timetuple()[0]
-month = today.timetuple()[1]
-day = today.timetuple()[2]        
-
-_sched = Metadata(schedule_name).static.reset_index(drop=True)
-sched = pd.DataFrame()
-for i,s in _sched.iterrows():
-    runtimes = s['Run Times'].split(',')
-    for t in runtimes:
-        hour = int(t.split(':')[0])
-        minute = int(t.split(':')[1])
-        dttm = local_tz.localize(datetime(year,month,day,hour,minute))
-        s['Run Times'] = dttm
-        sched = sched.reindex(columns=s.index.union(sched.columns))
-        sched = pd.concat([sched, pd.DataFrame(s).T])
-
-sched = sched.sort_values(by=['Run Times','Name']).reset_index(drop=True)
-sched['Status'] = np.nan
-sched['Last Message'] = np.nan
-
-uruntimes = sched['Run Times'].unique()
-runtime = uruntimes[0]
-sched_sort = pd.DataFrame(columns=sched.columns)
-for runtime in uruntimes:
-    # mark pending routines
-    while True:
-        idx = runtime.astimezone(tz=local_tz)>=sched['Run Times']
-        idx = (idx) & ((sched['Status'].isnull()) | (sched['Status']=='WAITING DEPENDENCIES'))
-
-        dfpending = sched[idx]
-        expiredidx = dfpending.duplicated(['Computer','Script'],keep='last')
-        if expiredidx.any():
-            expiredids = expiredidx.index[expiredidx]
-            sched.loc[expiredids,'Status'] = 'EXPIRED'
-        dfpending = dfpending[~expiredidx]
-        i=0
-        for i in dfpending.index:
-            r = dfpending.loc[i]
-            if not str(r['Dependencies'])=='nan':
-                run=True
-                sched.loc[i,'Status'] = 'WAITING DEPENDENCIES'
-                dependencies = r['Dependencies'].replace('\n','').split(',')                
-                for dep in dependencies:
-                    computer = dep.split(':')[0]
-                    script = dep.split(':')[1]
-                    idx = sched['Computer']==computer
-                    idx = (idx) & (sched['Script']==script)
-                    idx = (idx) & (sched['Run Times']<=runtime.astimezone(tz=local_tz))
-                    ids = sched.index[idx]
-                    if len(ids)==0:
-                        Logger.log.error('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
-                        raise Exception('Dependency not scheduled for '+r['Computer']+':'+r['Script'])                        
-                    else:
-                        if not str(sched.loc[ids[-1],'Status']) == 'COMPLETED':
-                            run=False
-                if run:
-                    sched.loc[i,'Status'] = 'PENDING'
-            else:
-                sched.loc[i,'Status'] = 'PENDING'
-
-        idx = sched['Status']=='PENDING'
-        if idx.any():
-            sched_sort = pd.concat([sched_sort, sched[idx]])
-            sched_sort['Status'] = np.nan
-            sched.loc[idx,'Status'] = 'COMPLETED'
-        else:
-            break
-
-sched_sort.head(50)
-
-    
-
+from datetime import datetime
+import pandas as pd
+import numpy as np
+import pytz
+from tzlocal import get_localzone 
+local_tz = pytz.timezone(str(get_localzone()))
+
+from SharedData.Logger import Logger
+logger = Logger(__file__,user='guest')
+from SharedData.Metadata import Metadata
+from SharedData.SharedDataAWSKinesis import KinesisLogStreamConsumer
+
+schedule_name = 'SCHEDULES/TRADEBOT06'
+today = datetime.now().date()
+year = today.timetuple()[0]
+month = today.timetuple()[1]
+day = today.timetuple()[2]        
+
+_sched = Metadata(schedule_name).static.reset_index(drop=True)
+sched = pd.DataFrame()
+for i,s in _sched.iterrows():
+    runtimes = s['Run Times'].split(',')
+    for t in runtimes:
+        hour = int(t.split(':')[0])
+        minute = int(t.split(':')[1])
+        dttm = local_tz.localize(datetime(year,month,day,hour,minute))
+        s['Run Times'] = dttm
+        sched = sched.reindex(columns=s.index.union(sched.columns))
+        sched = pd.concat([sched, pd.DataFrame(s).T])
+
+sched = sched.sort_values(by=['Run Times','Name']).reset_index(drop=True)
+sched['Status'] = np.nan
+sched['Last Message'] = np.nan
+
+uruntimes = sched['Run Times'].unique()
+runtime = uruntimes[0]
+sched_sort = pd.DataFrame(columns=sched.columns)
+for runtime in uruntimes:
+    # mark pending routines
+    while True:
+        idx = runtime.astimezone(tz=local_tz)>=sched['Run Times']
+        idx = (idx) & ((sched['Status'].isnull()) | (sched['Status']=='WAITING DEPENDENCIES'))
+
+        dfpending = sched[idx]
+        expiredidx = dfpending.duplicated(['Computer','Script'],keep='last')
+        if expiredidx.any():
+            expiredids = expiredidx.index[expiredidx]
+            sched.loc[expiredids,'Status'] = 'EXPIRED'
+        dfpending = dfpending[~expiredidx]
+        i=0
+        for i in dfpending.index:
+            r = dfpending.loc[i]
+            if not str(r['Dependencies'])=='nan':
+                run=True
+                sched.loc[i,'Status'] = 'WAITING DEPENDENCIES'
+                dependencies = r['Dependencies'].replace('\n','').split(',')                
+                for dep in dependencies:
+                    computer = dep.split(':')[0]
+                    script = dep.split(':')[1]
+                    idx = sched['Computer']==computer
+                    idx = (idx) & (sched['Script']==script)
+                    idx = (idx) & (sched['Run Times']<=runtime.astimezone(tz=local_tz))
+                    ids = sched.index[idx]
+                    if len(ids)==0:
+                        Logger.log.error('Dependency not scheduled for '+r['Computer']+':'+r['Script'])
+                        raise Exception('Dependency not scheduled for '+r['Computer']+':'+r['Script'])                        
+                    else:
+                        if not str(sched.loc[ids[-1],'Status']) == 'COMPLETED':
+                            run=False
+                if run:
+                    sched.loc[i,'Status'] = 'PENDING'
+            else:
+                sched.loc[i,'Status'] = 'PENDING'
+
+        idx = sched['Status']=='PENDING'
+        if idx.any():
+            sched_sort = pd.concat([sched_sort, sched[idx]])
+            sched_sort['Status'] = np.nan
+            sched.loc[idx,'Status'] = 'COMPLETED'
+        else:
+            break
+
+sched_sort.head(50)
+
+    
+
```

### Comparing `decentralizedroutines-2.0.7/src/decentralizedroutines/worker.py` & `decentralizedroutines-2.2.0/src/decentralizedroutines/worker.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-# implements a decentralized routines worker 
-# connects to worker pool
-# broadcast heartbeat
-# listen to commands
-# environment variables:
-# SOURCE_FOLDER
-# WORKERPOOL_STREAM
-# GIT_SERVER
-# GIT_USER
-# GIT_ACRONYM
-# GIT_TOKEN
-
-import os,time
-from importlib.metadata import version
-import numpy as np
-from threading import Thread
-
-import decentralizedroutines.defaults as defaults 
-from SharedData.Logger import Logger
-logger = Logger(r'decentralizedroutines\worker',user='worker')
-
-from SharedData.SharedDataAWSKinesis import KinesisStreamConsumer,\
-    KinesisStreamProducer
-from decentralizedroutines.worker_lib import send_command,install_repo,\
-    restart_program,run_routine,run_logger,run_scheduler
-
-Logger.log.info('Initializing decentralizedroutines worker version %s...' % \
-    (version('decentralizedroutines')))
-
-routines = []
-consumer = KinesisStreamConsumer(os.environ['WORKERPOOL_STREAM'])
-producer = KinesisStreamProducer(os.environ['WORKERPOOL_STREAM'])
-SLEEP_TIME = int(os.environ['SLEEP_TIME'])
-
-Logger.log.info('decentralizedroutines worker version %s STARTED!' % \
-    (version('decentralizedroutines')))
-
-while True:
-    try:
-            
-        for routine in routines:
-            if ('process' in routine):
-                if (not routine['process'] is None):
-                    if routine['process'].poll() is not None:
-                        routines.remove(routine)
-            elif (not routine['thread'].is_alive()):
-                routines.remove(routine)
-
-        if not consumer.consume():
-            consumer.get_stream()
-            Logger.log.error('Cannot consume workerpool messages!')
-            time.sleep(5)
-
-        for record in consumer.stream_buffer:
-            print('Received:'+str(record))
-            
-            command = record
-            if ('job' in command) & ('target' in command):
-                if ((command['target'].lower()==os.environ['USER_COMPUTER'].lower())\
-                     | (command['target']=='ALL')):
-                    
-                    if command['job'] == 'command':
-                        send_command(command['command'])
-
-                    elif command['job'] == 'gitpwd':
-                        if 'GIT_USER' in command:
-                            os.environ['GIT_USER'] = command['GIT_USER']
-                        if 'GIT_TOKEN' in command:
-                            os.environ['GIT_TOKEN'] = command['GIT_TOKEN']
-                        if 'GIT_ACRONYM' in command:
-                            os.environ['GIT_ACRONYM'] = command['GIT_ACRONYM']
-                        if 'GIT_SERVER' in command:
-                            os.environ['GIT_SERVER'] = command['GIT_SERVER']
-                        Logger.log.info('Updated git parameters!')
-
-                    elif command['job'] == 'routine': 
-                        start_time = time.time()
-                        routine = {
-                            'command':command,
-                            'thread':None,
-                            'process':None,
-                            'start_time':start_time,
-                        }                     
-                        thread = Thread(target=run_routine,args=(command,routine))
-                        routine['thread'] = thread
-                        routines.append(routine)
-                        thread.start()
-                        
-                    elif command['job'] == 'install':
-                        start_time = time.time()
-                        routine = {
-                            'command':command,
-                            'thread':None,
-                            'start_time':start_time,
-                        }                     
-                        thread = Thread(target=install_repo,args=(command,routine))
-                        routine['thread'] = thread
-                        routines.append(routine)
-                        thread.start()
-
-                    elif command['job'] == 'logger':
-                        isrunning = False
-                        for routine in routines:
-                            if (routine['command']['repo']=='logger'):
-                                isrunning=True
-                                break                                
-                        if not isrunning:
-                            routine = run_logger(command)
-                            routines.append(routine)
-                            
-                        else:
-                            Logger.log.info('Logger already running!')
-                            
-
-                    elif command['job'] == 'scheduler':
-                        isrunning = False
-                        for routine in routines:
-                            if (routine['command']['repo']=='scheduler'):
-                                if 'args' in routine['command']:
-                                    if (routine['command']['args']==command['args']):
-                                        isrunning=True
-                                        break                                
-                        if not isrunning:
-                            routine = run_scheduler(command)
-                            routines.append(routine)
-                            
-                        else:
-                            Logger.log.info('Scheduler %s already running!' % (command['args']))
-
-                    elif command['job'] == 'status': 
-
-                        Logger.log.info('Status: %i process' % (len(routines)))
-                        for routine in routines:
-                            if 'routine' in routine['command']:
-                                Logger.log.info('Status: running %s/%s %.2fs' % \
-                                    (routine['command']['repo'],routine['command']['routine'],\
-                                        time.time()-routine['start_time']))
-                            else:
-                                Logger.log.info('Status: running %s %.2fs' % \
-                                    (routine['command']['repo'],\
-                                    time.time()-routine['start_time']))
-
-                    elif command['job'] == 'kill':
-                        if command['repo']=='ALL':
-                            Logger.log.info('Kill: ALL...')
-                            for routine in routines:                            
-                                try:
-                                    routine['process'].kill()
-                                except:
-                                    pass
-                            Logger.log.info('Kill: ALL DONE!')
-                        else:
-                            for routine in routines:
-                                kill=False
-                                if (routine['command']['repo']==command['repo']):
-                                    if 'routine' in command:
-                                        if (routine['command']['routine']==command['routine']):
-                                            kill=True
-                                    else:
-                                        kill=True
-                                
-                                if (kill) & ('process' in routine):
-                                    try:                                                                                
-                                        routine['process'].kill()
-                                        if 'routine' in command:
-                                            Logger.log.info('Kill: %s/%s %.2fs DONE!' % \
-                                                (routine['command']['repo'],routine['command']['routine'],\
-                                                time.time()-routine['start_time']))
-                                        else:
-                                            Logger.log.info('Kill: %s %.2fs DONE!' % \
-                                                (routine['command']['repo'],time.time()-routine['start_time']))
-                                    except:
-                                        pass
-
-                    elif command['job'] == 'restart':                    
-                        restart_program()
-
-                    elif command['job'] == 'ping':
-                        Logger.log.info('pong')
-
-                    elif command['job'] == 'pong':
-                        Logger.log.info('ping')
-
-        consumer.stream_buffer = []
-        time.sleep(SLEEP_TIME + SLEEP_TIME*np.random.rand() - SLEEP_TIME/2)
-
-    except Exception as e:
-        Logger.log.error('Worker ERROR\n%s' % (str(e)))
-        consumer.stream_buffer = []
-        time.sleep(SLEEP_TIME + SLEEP_TIME*np.random.rand() - SLEEP_TIME/2)
-        
+# implements a decentralized routines worker 
+# connects to worker pool
+# broadcast heartbeat
+# listen to commands
+# environment variables:
+# SOURCE_FOLDER
+# WORKERPOOL_STREAM
+# GIT_SERVER
+# GIT_USER
+# GIT_ACRONYM
+# GIT_TOKEN
+
+import os,time
+from importlib.metadata import version
+import numpy as np
+from threading import Thread
+
+import decentralizedroutines.defaults as defaults 
+from SharedData.Logger import Logger
+logger = Logger(r'decentralizedroutines\worker',user='worker')
+
+from SharedData.SharedDataAWSKinesis import KinesisStreamConsumer,\
+    KinesisStreamProducer
+from decentralizedroutines.worker_lib import send_command,install_repo,\
+    restart_program,run_routine,run_logger,run_scheduler
+
+Logger.log.info('Initializing decentralizedroutines worker version %s...' % \
+    (version('decentralizedroutines')))
+
+routines = []
+consumer = KinesisStreamConsumer(os.environ['WORKERPOOL_STREAM'])
+producer = KinesisStreamProducer(os.environ['WORKERPOOL_STREAM'])
+SLEEP_TIME = int(os.environ['SLEEP_TIME'])
+
+Logger.log.info('decentralizedroutines worker version %s STARTED!' % \
+    (version('decentralizedroutines')))
+
+while True:
+    try:
+            
+        for routine in routines:
+            if ('process' in routine):
+                if (not routine['process'] is None):
+                    if routine['process'].poll() is not None:
+                        routines.remove(routine)
+            elif (not routine['thread'].is_alive()):
+                routines.remove(routine)
+
+        if not consumer.consume():
+            consumer.get_stream()
+            Logger.log.error('Cannot consume workerpool messages!')
+            time.sleep(5)
+
+        for record in consumer.stream_buffer:
+            print('Received:'+str(record))
+            
+            command = record
+            if ('job' in command) & ('target' in command):
+                if ((command['target'].lower()==os.environ['USER_COMPUTER'].lower())\
+                     | (command['target']=='ALL')):
+                    
+                    if command['job'] == 'command':
+                        send_command(command['command'])
+
+                    elif command['job'] == 'gitpwd':
+                        if 'GIT_USER' in command:
+                            os.environ['GIT_USER'] = command['GIT_USER']
+                        if 'GIT_TOKEN' in command:
+                            os.environ['GIT_TOKEN'] = command['GIT_TOKEN']
+                        if 'GIT_ACRONYM' in command:
+                            os.environ['GIT_ACRONYM'] = command['GIT_ACRONYM']
+                        if 'GIT_SERVER' in command:
+                            os.environ['GIT_SERVER'] = command['GIT_SERVER']
+                        Logger.log.info('Updated git parameters!')
+
+                    elif command['job'] == 'routine': 
+                        start_time = time.time()
+                        routine = {
+                            'command':command,
+                            'thread':None,
+                            'process':None,
+                            'start_time':start_time,
+                        }                     
+                        thread = Thread(target=run_routine,args=(command,routine))
+                        routine['thread'] = thread
+                        routines.append(routine)
+                        thread.start()
+                        
+                    elif command['job'] == 'install':
+                        start_time = time.time()
+                        routine = {
+                            'command':command,
+                            'thread':None,
+                            'start_time':start_time,
+                        }                     
+                        thread = Thread(target=install_repo,args=(command,routine))
+                        routine['thread'] = thread
+                        routines.append(routine)
+                        thread.start()
+
+                    elif command['job'] == 'logger':
+                        isrunning = False
+                        for routine in routines:
+                            if (routine['command']['repo']=='logger'):
+                                isrunning=True
+                                break                                
+                        if not isrunning:
+                            routine = run_logger(command)
+                            routines.append(routine)
+                            
+                        else:
+                            Logger.log.info('Logger already running!')
+                            
+
+                    elif command['job'] == 'scheduler':
+                        isrunning = False
+                        for routine in routines:
+                            if (routine['command']['repo']=='scheduler'):
+                                if 'args' in routine['command']:
+                                    if (routine['command']['args']==command['args']):
+                                        isrunning=True
+                                        break                                
+                        if not isrunning:
+                            routine = run_scheduler(command)
+                            routines.append(routine)
+                            
+                        else:
+                            Logger.log.info('Scheduler %s already running!' % (command['args']))
+
+                    elif command['job'] == 'status': 
+
+                        Logger.log.info('Status: %i process' % (len(routines)))
+                        for routine in routines:
+                            if 'routine' in routine['command']:
+                                Logger.log.info('Status: running %s/%s %.2fs' % \
+                                    (routine['command']['repo'],routine['command']['routine'],\
+                                        time.time()-routine['start_time']))
+                            else:
+                                Logger.log.info('Status: running %s %.2fs' % \
+                                    (routine['command']['repo'],\
+                                    time.time()-routine['start_time']))
+
+                    elif command['job'] == 'kill':
+                        if command['repo']=='ALL':
+                            Logger.log.info('Kill: ALL...')
+                            for routine in routines:                            
+                                try:
+                                    routine['process'].kill()
+                                except:
+                                    pass
+                            Logger.log.info('Kill: ALL DONE!')
+                        else:
+                            for routine in routines:
+                                kill=False
+                                if (routine['command']['repo']==command['repo']):
+                                    if 'routine' in command:
+                                        if (routine['command']['routine']==command['routine']):
+                                            kill=True
+                                    else:
+                                        kill=True
+                                
+                                if (kill) & ('process' in routine):
+                                    try:                                                                                
+                                        routine['process'].kill()
+                                        if 'routine' in command:
+                                            Logger.log.info('Kill: %s/%s %.2fs DONE!' % \
+                                                (routine['command']['repo'],routine['command']['routine'],\
+                                                time.time()-routine['start_time']))
+                                        else:
+                                            Logger.log.info('Kill: %s %.2fs DONE!' % \
+                                                (routine['command']['repo'],time.time()-routine['start_time']))
+                                    except:
+                                        pass
+
+                    elif command['job'] == 'restart':                    
+                        restart_program()
+
+                    elif command['job'] == 'ping':
+                        Logger.log.info('pong')
+
+                    elif command['job'] == 'pong':
+                        Logger.log.info('ping')
+
+        consumer.stream_buffer = []
+        time.sleep(SLEEP_TIME + SLEEP_TIME*np.random.rand() - SLEEP_TIME/2)
+
+    except Exception as e:
+        Logger.log.error('Worker ERROR\n%s' % (str(e)))
+        consumer.stream_buffer = []
+        time.sleep(SLEEP_TIME + SLEEP_TIME*np.random.rand() - SLEEP_TIME/2)
+
```

### Comparing `decentralizedroutines-2.0.7/src/decentralizedroutines/worker_lib.py` & `decentralizedroutines-2.2.0/src/decentralizedroutines/worker_lib.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,234 +1,272 @@
-# implements a decentralized routines worker 
-# connects to worker pool
-# broadcast heartbeat
-# listen to commands
-
-import os,sys,psutil,time,subprocess
-from subprocess import DEVNULL
-
-import numpy as np
-from pathlib import Path
-
-from SharedData.Logger import Logger
-
-def restart_program():
-    """Restarts the current program, with file objects and descriptors
-       cleanup
-    """
-    Logger.log.info('restarting worker...')
-    try:
-        p = psutil.Process(os.getpid())
-        children = p.children(recursive=True)
-        for child in children:
-            child.kill()         
-
-    except Exception as e:
-        Logger.log.error('restarting worker ERROR!')
-        Logger.log.error(e)
-
-    python = sys.executable
-    os.execl(python, python, *sys.argv)
-
-def send_command(command,env=None):
-    Logger.log.debug('sending command: %s...' % (' '.join(command)))
-
-    if os.name=='posix':
-        command = ' '.join(command)
-
-    if env is None:
-        process = subprocess.Popen(command,\
-            stdout=subprocess.PIPE, stderr=subprocess.PIPE,\
-            universal_newlines=True, shell=True)        
-    else:    
-        process = subprocess.Popen(command,\
-            stdout=subprocess.PIPE, stderr=subprocess.PIPE,\
-            universal_newlines=True, shell=True,env=env)        
-
-    while True:
-        output = process.stdout.readline()
-        if ((output == '') | (output == b''))\
-                & (process.poll() is not None):
-            break        
-        if (output):
-            output = output.rstrip()
-            if output!='':
-                Logger.log.debug('command response:'+output)  
-    rc = process.poll() #block until process terminated
-    success= rc==0
-    if success:
-        Logger.log.debug('sending command DONE!')
-        return True
-    else:
-        Logger.log.error('sending command ERROR:%s!' % (''.join(process.stderr.readlines())))
-        return False
-
-def get_env(command):
-    hasbranch = False
-    if 'branch' in command:
-        if command['branch']!='':
-            hasbranch=True
-
-    if hasbranch:
-        repo_path=Path(os.environ['SOURCE_FOLDER'])/(command['repo']+'#'+command['branch'])
-    else:
-        repo_path=Path(os.environ['SOURCE_FOLDER'])/command['repo']
-
-    requirements_path = repo_path/'requirements.txt'
-    if os.name=='posix':
-        python_path=repo_path/'venv/bin/python'
-    else:
-        python_path=repo_path/'venv\\Scripts\\python.exe'
-
-    env = os.environ.copy()
-    env['VIRTUAL_ENV'] = str(repo_path/'venv')
-    env['PATH'] = str(repo_path/'venv')+';'+str(python_path.parents[0])+';'+env['PATH']
-    env['PYTHONPATH'] = str(repo_path/'venv')+';'+str(python_path.parents[0])
-    env['GIT_TERMINAL_PROMPT'] = "0"
-
-    return hasbranch, requirements_path, repo_path, python_path, env
-
-def run_routine(command,routine):
-    Logger.log.info('Running routine %s/%s' % (command['repo'],command['routine']))
-                        
-    if install_repo(command):
-        # RUN ROUTINE                         
-        Logger.log.info('Starting process %s/%s...' % (command['repo'],command['routine'])) 
-
-        hasbranch, requirements_path, repo_path, python_path, env = get_env(command)
-
-        if 'args' in command:
-            cmd = [str(python_path),str(repo_path/command['routine']),command['args']]
-        else:
-            cmd = [str(python_path),str(repo_path/command['routine'])]
-        
-        routine['process'] = subprocess.Popen(cmd,env=env)
-                
-        Logger.log.info('Starting process %s/%s DONE!' % (command['repo'],command['routine'])) 
-    else:
-        Logger.log.error('Aborting routine %s, could not install repo' % (command['routine']))
-
-def install_repo(command,routine=None):
-
-    Logger.log.info('Installing %s...' % (command['repo']))
-    runroutine = False
-    if  ('GIT_USER' not in os.environ) | \
-        ('GIT_TOKEN' not in os.environ) |\
-        ('GIT_ACRONYM' not in os.environ):
-        Logger.log.error('Installing repo %s ERROR missing git parameters'\
-                % (command['repo']))
-    else:
-        
-        hasbranch, requirements_path, repo_path, python_path, env = get_env(command)
-
-        repo_exists = repo_path.is_dir()
-        venv_exists = python_path.is_file()
-        install_requirements=~python_path.is_file()
-                
-        GIT_URL=os.environ['GIT_PROTOCOL']+'://'+os.environ['GIT_USER']+':'+os.environ['GIT_TOKEN']+'@'\
-            +os.environ['GIT_SERVER']+'/'+os.environ['GIT_ACRONYM']+'/'+command['repo']
-        
-        # GIT PULL OR GIT CLONE
-        if repo_exists:                 
-            Logger.log.info('Pulling repo %s' % (command['repo']))    
-            requirements_lastmod = 0
-            if requirements_path.is_file():
-                requirements_lastmod = os.path.getmtime(str(requirements_path))            
-            
-            # pull existing repo
-            if hasbranch:
-                cmd = ['git','-C',str(repo_path),'pull',GIT_URL,command['branch']]
-            else:
-                cmd = ['git','-C',str(repo_path),'pull',GIT_URL]
-
-            if not send_command(cmd):
-                Logger.log.error('Pulling repo %s ERROR!' % (command['repo']))
-                runroutine = False
-            else:
-                if requirements_path.is_file():
-                    install_requirements = os.path.getmtime(str(requirements_path))!=requirements_lastmod                        
-                    runroutine=True        
-                    Logger.log.info('Pulling repo %s DONE!' % (command['repo']))
-                else:
-                    install_requirements = False
-                    runroutine = False
-                    Logger.log.error('Pulling repo %s ERROR: requirements.txt not found!' % (command['repo']))
-                    
-        else:                        
-            Logger.log.info('Cloning repo %s...' % (command['repo']))
-            if hasbranch:
-                cmd = ['git','-C',str(repo_path.parents[0]),'clone','-b',command['branch'],GIT_URL,str(repo_path)]
-            else:
-                cmd = ['git','-C',str(repo_path.parents[0]),'clone',GIT_URL]
-            if not send_command(cmd):
-                Logger.log.error('Cloning repo %s ERROR!' % (command['repo']))
-                runroutine=False
-            else:               
-                runroutine=True
-                if requirements_path.is_file():
-                    install_requirements = True
-                    Logger.log.info('Cloning repo %s DONE!' % (command['repo']))
-                else:
-                    install_requirements = False
-                    Logger.log.error('Cloning repo %s ERROR: requirements.txt not found!' % (command['repo']))
-
-        # CREATE VENV
-        if (runroutine) & (not venv_exists):
-            Logger.log.info('Creating venv %s...' % (command['repo']))
-            if not send_command(['python','-m','venv',str(repo_path/'venv')]):
-                Logger.log.error('Creating venv %s ERROR!' % (command['repo']))
-                runroutine=False
-            else:
-                runroutine=True
-                if requirements_path.is_file():
-                    install_requirements=True
-                    Logger.log.info('Creating venv %s DONE!' % (command['repo']))
-                else:
-                    install_requirements = False
-                    Logger.log.error('Creating venv %s ERROR: requirements.txt not found!' % (command['repo']))   
-                        
-        # INSTALL REQUIREMENTS
-        if (runroutine) & (install_requirements):
-            Logger.log.info('Installing requirements %s...' % (command['repo']))
-            if not send_command([str(python_path),'-m','pip','install','-r',str(requirements_path)],env=env):
-                Logger.log.error('Installing requirements %s ERROR!' % (command['repo']))
-                runroutine=False
-            else:                
-                runroutine=True
-                Logger.log.info('Installing requirements %s DONE!' % (command['repo']))
-    
-    if runroutine:   
-        Logger.log.info('Installing %s DONE!' % (command['repo']))
-    else:
-        Logger.log.error('Installing %s ERROR!' % (command['repo']))
-    return runroutine
-
-def run_logger(command):
-    Logger.log.info('Starting logger...')                            
-    start_time = time.time()
-    routine = {
-        'command':command,
-        'process':None,
-        'start_time':start_time,
-    }   
-    command['repo']='' 
-    hasbranch, requirements_path, repo_path, python_path, env = get_env(command)
-    command['repo']='logger' 
-    cmd = [str(python_path),'-m','SharedData.LoggerConsumerProcess']
-    routine['process'] = subprocess.Popen(cmd,env=env)
-    return routine
-
-def run_scheduler(command):
-    Logger.log.info('Starting scheduler %s...' % (command['args']))                            
-    start_time = time.time()
-    routine = {
-        'command':command,                                
-        'process':None,
-        'start_time':start_time,
-    }
-    command['repo']='' 
-    hasbranch, requirements_path, repo_path, python_path, env = get_env(command)
-    command['repo']='scheduler'
-    cmd = [str(python_path),'-m','decentralizedroutines.runroutines',command['args']]
-    routine['process'] = subprocess.Popen(cmd,env=env)
-    return routine
+# implements a decentralized routines worker 
+# connects to worker pool
+# broadcast heartbeat
+# listen to commands
+
+import os,sys,psutil,time,subprocess
+import threading
+from subprocess import DEVNULL
+
+import numpy as np
+from pathlib import Path
+
+from SharedData.Logger import Logger
+
+def restart_program():
+    """Restarts the current program, with file objects and descriptors
+       cleanup
+    """
+    Logger.log.info('restarting worker...')
+    try:
+        p = psutil.Process(os.getpid())
+        children = p.children(recursive=True)
+        for child in children:
+            child.kill()         
+
+    except Exception as e:
+        Logger.log.error('restarting worker ERROR!')
+        Logger.log.error(e)
+
+    python = sys.executable
+    os.execl(python, python, *sys.argv)
+
+def read_stdout(stdout):
+    try:
+        while True:
+            out = stdout.readline()
+            if out:
+                out = out.replace('\n','')
+                if (out!=''):
+                    Logger.log.debug('<-' + out)
+            else:
+                break
+    except:
+        pass
+
+def read_stderr(stderr):
+    try:
+        while True:
+            err = stderr.readline()
+            if err:
+                err = err.replace('\n','')
+                if (err!=''):
+                    if ('INFO' in err):
+                        Logger.log.info('<-'+err)
+                    elif ('ERROR' in err):
+                        Logger.log.error('<-'+err)
+                    elif ('CRITICAL' in err):
+                        Logger.log.critical('<-'+err)
+                    else:
+                        Logger.log.debug('<-'+err)
+            else:
+                break
+    except:
+        pass
+
+def send_command(command,env=None):
+    Logger.log.debug('->%s' % (' '.join(command)))
+
+    _command = command
+    if os.name=='posix':
+        _command = ' '.join(command)
+
+    if env is None:
+        process = subprocess.Popen(_command,\
+            stdout=subprocess.PIPE, stderr=subprocess.PIPE,\
+            universal_newlines=True, shell=True)        
+    else:    
+        process = subprocess.Popen(_command,\
+            stdout=subprocess.PIPE, stderr=subprocess.PIPE,\
+            universal_newlines=True, shell=True,env=env)        
+
+    stdout_thread = threading.Thread(target=read_stdout, args=([process.stdout]))
+    stderr_thread = threading.Thread(target=read_stderr, args=([process.stderr]))
+    stdout_thread.start()
+    stderr_thread.start()
+
+    process.wait()  # block until process terminated
+
+    stdout_thread.join()
+    stderr_thread.join()
+
+    rc = process.returncode
+    success = rc == 0
+    if success:
+        Logger.log.debug('DONE!->%s' % (' '.join(command)))
+        return True
+    else:
+        Logger.log.error('ERROR!->%s' % (' '.join(command)))
+        return False
+
+def get_env(command):
+    hasbranch = False
+    if 'branch' in command:
+        if command['branch']!='':
+            hasbranch=True
+
+    if hasbranch:
+        repo_path=Path(os.environ['SOURCE_FOLDER'])/(command['repo']+'#'+command['branch'])
+    else:
+        repo_path=Path(os.environ['SOURCE_FOLDER'])/command['repo']
+
+    requirements_path = repo_path/'requirements.txt'
+    if os.name=='posix':
+        python_path=repo_path/'venv/bin/python'
+    else:
+        python_path=repo_path/'venv/Scripts/python.exe'
+
+    env = os.environ.copy()
+    env['VIRTUAL_ENV'] = str(repo_path/'venv')
+    env['PATH'] = str(repo_path/'venv')+';'+str(python_path.parents[0])+';'+env['PATH']
+    env['PYTHONPATH'] = str(repo_path/'venv')+';'+str(python_path.parents[0])
+    env['GIT_TERMINAL_PROMPT'] = "0"
+
+    return hasbranch, requirements_path, repo_path, python_path, env
+
+def run_routine(command,routine):
+    Logger.log.info('Running routine %s/%s' % (command['repo'],command['routine']))
+                        
+    if install_repo(command):
+        # RUN ROUTINE                         
+        Logger.log.info('Starting process %s/%s...' % (command['repo'],command['routine'])) 
+
+        hasbranch, requirements_path, repo_path, python_path, env = get_env(command)
+
+        if 'args' in command:
+            cmd = [str(python_path),str(repo_path/command['routine']),command['args']]
+        else:
+            cmd = [str(python_path),str(repo_path/command['routine'])]
+        
+        routine['process'] = subprocess.Popen(cmd,env=env)
+                
+        Logger.log.info('Starting process %s/%s DONE!' % (command['repo'],command['routine'])) 
+    else:
+        Logger.log.error('Aborting routine %s, could not install repo' % (command['routine']))
+
+def install_repo(command,routine=None):
+
+    Logger.log.info('Installing %s...' % (command['repo']))
+    runroutine = False
+    if  ('GIT_USER' not in os.environ) | \
+        ('GIT_TOKEN' not in os.environ) |\
+        ('GIT_ACRONYM' not in os.environ):
+        Logger.log.error('Installing repo %s ERROR missing git parameters'\
+                % (command['repo']))
+    else:
+        
+        hasbranch, requirements_path, repo_path, python_path, env = get_env(command)
+
+        repo_exists = repo_path.is_dir()
+        venv_exists = python_path.is_file()
+        install_requirements=~python_path.is_file()
+                
+        # GIT_URL=os.environ['GIT_PROTOCOL']+'://'+os.environ['GIT_USER']+':'+os.environ['GIT_TOKEN']+'@'\
+        #     +os.environ['GIT_SERVER']+'/'+os.environ['GIT_ACRONYM']+'/'+command['repo']
+        GIT_URL=os.environ['GIT_PROTOCOL']+'://'+os.environ['GIT_SERVER']+'/'+\
+            os.environ['GIT_ACRONYM']+'/'+command['repo']
+        
+        # GIT PULL OR GIT CLONE
+        if repo_exists:                 
+            Logger.log.info('Pulling repo %s' % (command['repo']))    
+            requirements_lastmod = 0
+            if requirements_path.is_file():
+                requirements_lastmod = os.path.getmtime(str(requirements_path))            
+            
+            # pull existing repo
+            if hasbranch:
+                cmd = ['git','-C',str(repo_path),'pull',GIT_URL,command['branch']]
+            else:
+                cmd = ['git','-C',str(repo_path),'pull',GIT_URL]
+
+            if not send_command(cmd):
+                Logger.log.error('Pulling repo %s ERROR!' % (command['repo']))
+                runroutine = False
+            else:
+                if requirements_path.is_file():
+                    install_requirements = os.path.getmtime(str(requirements_path))!=requirements_lastmod                        
+                    runroutine=True        
+                    Logger.log.info('Pulling repo %s DONE!' % (command['repo']))
+                else:
+                    install_requirements = False
+                    runroutine = False
+                    Logger.log.error('Pulling repo %s ERROR: requirements.txt not found!' % (command['repo']))
+                    
+        else:                        
+            Logger.log.info('Cloning repo %s...' % (command['repo']))
+            if hasbranch:
+                cmd = ['git','-C',str(repo_path.parents[0]),'clone','-b',command['branch'],GIT_URL,str(repo_path)]
+            else:
+                cmd = ['git','-C',str(repo_path.parents[0]),'clone',GIT_URL]
+            if not send_command(cmd):
+                Logger.log.error('Cloning repo %s ERROR!' % (command['repo']))
+                runroutine=False
+            else:               
+                runroutine=True
+                if requirements_path.is_file():
+                    install_requirements = True
+                    Logger.log.info('Cloning repo %s DONE!' % (command['repo']))
+                else:
+                    install_requirements = False
+                    Logger.log.error('Cloning repo %s ERROR: requirements.txt not found!' % (command['repo']))
+
+        # CREATE VENV
+        if (runroutine) & (not venv_exists):
+            Logger.log.info('Creating venv %s...' % (command['repo']))
+            if not send_command(['python','-m','venv',str(repo_path/'venv')]):
+                Logger.log.error('Creating venv %s ERROR!' % (command['repo']))
+                runroutine=False
+            else:
+                runroutine=True
+                if requirements_path.is_file():
+                    install_requirements=True
+                    Logger.log.info('Creating venv %s DONE!' % (command['repo']))
+                else:
+                    install_requirements = False
+                    Logger.log.error('Creating venv %s ERROR: requirements.txt not found!' % (command['repo']))   
+                        
+        # INSTALL REQUIREMENTS
+        if (runroutine) & (install_requirements):
+            Logger.log.info('Installing requirements %s...' % (command['repo']))
+            if not send_command([str(python_path),'-m','pip','install','-r',str(requirements_path)],env=env):
+                Logger.log.error('Installing requirements %s ERROR!' % (command['repo']))
+                runroutine=False
+            else:                
+                runroutine=True
+                Logger.log.info('Installing requirements %s DONE!' % (command['repo']))
+    
+    if runroutine:   
+        Logger.log.info('Installing %s DONE!' % (command['repo']))
+    else:
+        Logger.log.error('Installing %s ERROR!' % (command['repo']))
+    return runroutine
+
+def run_logger(command):
+    Logger.log.info('Starting logger...')                            
+    start_time = time.time()
+    routine = {
+        'command':command,
+        'process':None,
+        'start_time':start_time,
+    }   
+    command['repo']='' 
+    hasbranch, requirements_path, repo_path, python_path, env = get_env(command)
+    command['repo']='logger' 
+    cmd = [str(python_path),'-m','SharedData.LoggerConsumerProcess']
+    routine['process'] = subprocess.Popen(cmd,env=env)
+    return routine
+
+def run_scheduler(command):
+    Logger.log.info('Starting scheduler %s...' % (command['args']))                            
+    start_time = time.time()
+    routine = {
+        'command':command,                                
+        'process':None,
+        'start_time':start_time,
+    }
+    command['repo']='' 
+    hasbranch, requirements_path, repo_path, python_path, env = get_env(command)
+    command['repo']='scheduler'
+    cmd = [str(python_path),'-m','decentralizedroutines.runroutines',command['args']]
+    routine['process'] = subprocess.Popen(cmd,env=env)
+    return routine
```

### Comparing `decentralizedroutines-2.0.7/src/decentralizedroutines.egg-info/PKG-INFO` & `decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: decentralizedroutines
-Version: 2.0.7
-Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
-Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
-Author: Jose Carlito de Oliveira Filho
-Author-email: jcarlitooliveira@gmail.com
-Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# DecentralizedRoutines
-Decentralized routines orquestration through Kinesis working pool 
-
-### create virtual environment
-<ul>
-<li>enter command: pip -m venv venv</li>
-<li>activate virtual environnment (venv\Scripts\activate.bat)</li>
-</ul>
-
-## Create .env file in root folder Ie:
-<ul>
-<li>LOG_LEVEL=[DEBUG]</li>
-<li>GIT_USER=[GIT_USER]</li>
-<li>GIT_TOKEN=[GIT_TOKEN]</li>
-<li>GIT_ACRONYM=[GIT_ACRONYM]</li>
-<li>GIT_SERVER=[GIT_SERVER]</li>
-<li>SOURCE_FOLDER=[SOURCE_FOLDER]</li>
-</ul>
+Metadata-Version: 2.1
+Name: decentralizedroutines
+Version: 2.2.0
+Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
+Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
+Author: Jose Carlito de Oliveira Filho
+Author-email: jcarlitooliveira@gmail.com
+Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DecentralizedRoutines
+Decentralized routines orquestration through Kinesis working pool 
+
+### create virtual environment
+<ul>
+<li>enter command: pip -m venv venv</li>
+<li>activate virtual environnment (venv\Scripts\activate.bat)</li>
+</ul>
+
+## Create .env file in root folder Ie:
+<ul>
+<li>LOG_LEVEL=[DEBUG]</li>
+<li>GIT_USER=[GIT_USER]</li>
+<li>GIT_TOKEN=[GIT_TOKEN]</li>
+<li>GIT_ACRONYM=[GIT_ACRONYM]</li>
+<li>GIT_SERVER=[GIT_SERVER]</li>
+<li>SOURCE_FOLDER=[SOURCE_FOLDER]</li>
+</ul>
```

### Comparing `decentralizedroutines-2.0.7/src/decentralizedroutines.egg-info/SOURCES.txt` & `decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

