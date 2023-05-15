# Comparing `tmp/pyUIauto-0.1.6.tar.gz` & `tmp/pyuiauto-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyUIauto-0.1.6.tar", max compression
+gzip compressed data, was "pyuiauto-0.1.7.tar", max compression
```

## Comparing `pyUIauto-0.1.6.tar` & `pyuiauto-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-05-11 08:21:35.782968 pyUIauto-0.1.6/LICENSE
--rw-r--r--   0        0        0     3898 2023-05-11 13:00:05.133282 pyUIauto-0.1.6/README.md
--rw-r--r--   0        0        0      877 2023-05-11 13:03:18.010544 pyUIauto-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 13:02:49.153584 pyUIauto-0.1.6/pyuiauto/.git/FETCH_HEAD
--rw-r--r--   0        0        0       23 2023-04-14 15:49:13.419447 pyUIauto-0.1.6/pyuiauto/.git/HEAD
--rw-r--r--   0        0        0      137 2023-04-14 15:49:13.420468 pyUIauto-0.1.6/pyuiauto/.git/config
--rw-r--r--   0        0        0       73 2023-04-14 15:49:13.416932 pyUIauto-0.1.6/pyuiauto/.git/description
--rwxr-xr-x   0        0        0      478 2023-04-14 15:49:13.417867 pyUIauto-0.1.6/pyuiauto/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2023-04-14 15:49:13.417217 pyUIauto-0.1.6/pyuiauto/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4655 2023-04-14 15:49:13.418048 pyUIauto-0.1.6/pyuiauto/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2023-04-14 15:49:13.418553 pyUIauto-0.1.6/pyuiauto/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2023-04-14 15:49:13.418735 pyUIauto-0.1.6/pyuiauto/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1643 2023-04-14 15:49:13.417684 pyUIauto-0.1.6/pyuiauto/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2023-04-14 15:49:13.418654 pyUIauto-0.1.6/pyuiauto/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1374 2023-04-14 15:49:13.418811 pyUIauto-0.1.6/pyuiauto/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2023-04-14 15:49:13.417423 pyUIauto-0.1.6/pyuiauto/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2023-04-14 15:49:13.418212 pyUIauto-0.1.6/pyuiauto/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2023-04-14 15:49:13.418394 pyUIauto-0.1.6/pyuiauto/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2783 2023-04-14 15:49:13.419156 pyUIauto-0.1.6/pyuiauto/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     3650 2023-04-14 15:49:13.418976 pyUIauto-0.1.6/pyuiauto/.git/hooks/update.sample
--rw-r--r--   0        0        0      240 2023-04-14 15:49:13.416691 pyUIauto-0.1.6/pyuiauto/.git/info/exclude
--rw-r--r--   0        0        0      174 2023-04-14 15:49:15.745880 pyUIauto-0.1.6/pyuiauto/.git/sourcetreeconfig
--rw-r--r--   0        0        0        0 2023-05-11 08:21:35.784952 pyUIauto-0.1.6/pyuiauto/__init__.py
--rw-r--r--   0        0        0      273 2023-05-11 08:21:35.785299 pyUIauto-0.1.6/pyuiauto/application.py
--rw-r--r--   0        0        0     8216 2023-05-11 13:00:05.134018 pyUIauto-0.1.6/pyuiauto/base/application.py
--rw-r--r--   0        0        0    15905 2023-05-11 08:21:35.785520 pyUIauto-0.1.6/pyuiauto/base/components.py
--rw-r--r--   0        0        0      474 2023-05-11 08:21:35.785580 pyUIauto-0.1.6/pyuiauto/components.py
--rw-r--r--   0        0        0      759 2023-05-11 08:21:35.785778 pyUIauto-0.1.6/pyuiauto/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-11 08:21:35.785833 pyUIauto-0.1.6/pyuiauto/mac/__init__.py
--rw-r--r--   0        0        0     4907 2023-05-11 08:21:35.785922 pyUIauto-0.1.6/pyuiauto/mac/application.py
--rw-r--r--   0        0        0    10968 2023-05-11 08:21:35.786019 pyUIauto-0.1.6/pyuiauto/mac/components.py
--rw-r--r--   0        0        0     2476 2023-05-11 08:21:35.786080 pyUIauto-0.1.6/pyuiauto/wait.py
--rw-r--r--   0        0        0        0 2023-05-11 08:21:35.786127 pyUIauto-0.1.6/pyuiauto/win/__init__.py
--rw-r--r--   0        0        0     7380 2023-05-11 13:00:05.134191 pyUIauto-0.1.6/pyuiauto/win/application.py
--rw-r--r--   0        0        0    10176 2023-05-11 13:00:05.134347 pyUIauto-0.1.6/pyuiauto/win/components.py
--rw-r--r--   0        0        0     5054 2023-05-11 13:03:25.100705 pyUIauto-0.1.6/setup.py
--rw-r--r--   0        0        0     4872 2023-05-11 13:03:25.101037 pyUIauto-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-05-11 11:46:20.965940 pyuiauto-0.1.7/LICENSE
+-rw-r--r--   0        0        0      956 2023-05-15 10:43:29.284240 pyuiauto-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 10:13:35.566412 pyuiauto-0.1.7/pyuiauto/__init__.py
+-rw-r--r--   0        0        0      284 2023-05-11 11:46:20.969173 pyuiauto-0.1.7/pyuiauto/application.py
+-rw-r--r--   0        0        0     9796 2023-05-15 10:14:01.090897 pyuiauto-0.1.7/pyuiauto/base/__pycache__/application.cpython-39.pyc
+-rw-r--r--   0        0        0    18104 2023-05-15 10:14:01.088892 pyuiauto-0.1.7/pyuiauto/base/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     7851 2023-05-15 10:08:51.151711 pyuiauto-0.1.7/pyuiauto/base/application.py
+-rw-r--r--   0        0        0    16607 2023-05-15 10:08:51.151711 pyuiauto-0.1.7/pyuiauto/base/components.py
+-rw-r--r--   0        0        0      480 2023-05-11 11:46:20.970476 pyuiauto-0.1.7/pyuiauto/components.py
+-rw-r--r--   0        0        0      792 2023-05-11 11:46:20.970476 pyuiauto-0.1.7/pyuiauto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:46:20.970476 pyuiauto-0.1.7/pyuiauto/mac/__init__.py
+-rw-r--r--   0        0        0     7883 2023-05-15 10:08:51.152715 pyuiauto-0.1.7/pyuiauto/mac/application.py
+-rw-r--r--   0        0        0    11678 2023-05-15 10:08:51.152715 pyuiauto-0.1.7/pyuiauto/mac/components.py
+-rw-r--r--   0        0        0     2522 2023-05-11 11:46:20.971889 pyuiauto-0.1.7/pyuiauto/wait.py
+-rw-r--r--   0        0        0        0 2023-05-11 11:46:20.971889 pyuiauto-0.1.7/pyuiauto/win/__init__.py
+-rw-r--r--   0        0        0      162 2023-05-15 09:48:46.590621 pyuiauto-0.1.7/pyuiauto/win/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9121 2023-05-15 11:28:34.364215 pyuiauto-0.1.7/pyuiauto/win/__pycache__/application.cpython-39.pyc
+-rw-r--r--   0        0        0    13624 2023-05-15 10:14:01.084613 pyuiauto-0.1.7/pyuiauto/win/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     8665 2023-05-15 11:28:19.266546 pyuiauto-0.1.7/pyuiauto/win/application.py
+-rw-r--r--   0        0        0    10557 2023-05-15 10:08:51.154160 pyuiauto-0.1.7/pyuiauto/win/components.py
+-rw-r--r--   0        0        0     4403 2023-05-15 10:08:51.148948 pyuiauto-0.1.7/README.md
+-rw-r--r--   0        0        0     5470 1970-01-01 00:00:00.000000 pyuiauto-0.1.7/setup.py
+-rw-r--r--   0        0        0     5413 1970-01-01 00:00:00.000000 pyuiauto-0.1.7/PKG-INFO
```

### Comparing `pyUIauto-0.1.6/LICENSE` & `pyuiauto-0.1.7/LICENSE`

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

### Comparing `pyUIauto-0.1.6/README.md` & `pyuiauto-0.1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,108 @@
-# pyUIauto
-
-[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
-[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
-[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)
-[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)
-
-
-| Tests       | Status                                                                                                                  |
-| :---------- | :---------------------------------------------------------------------------------------------------------------------: |
-| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |
-| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |
-
-Python UI Automation library, for cross-platform applications, interfacing through the accessibility API.
-
-## Description
-
-This library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.
-
-## Getting Started
-
-### Dependencies
-
-Python Packages:
-
-- pywinauto (Windows / Linux)
-- atomacos (MacOS)
-- pyautogui
-
-OS Compatibility:
-
-- Windows
-- MacOS
-
-( Currently untested on Linux )
-
-## Example
-
-```python
-# Import the tools needed
-from platform import system
-import os
-from pyuiauto.application import UIApplication
-from pyuiauto.components import UIButton
-
-# Finding the path location of the application
-app_paths = {
-  "Darwin": "/Applications/Visual Studio Code.app",
-  "Windows": os.path.expanduser('~') + "\\AppData\\Local\\Programs\\Microsoft VS Code\\Code.exe"
-}
-
-if system() in app_paths:
-  appPath = app_paths[system()]
-else:
-  raise NotImplementedError("The current OS is not currently supported: " + system())
-
-# Setting up an application template, launching the app, and connecting to it
-app = UIApplication(appName = "Visual Studio Code", appPath = appPath)
-app.launchApp()
-app.connectApp()
-
-# Finding the window component and searching for elements within this window component
-main_window = app.window(title = "Visual Studio Code", timeout = 2)
-main_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() '''  press will invoke a button without manually moving the mouse and clicking it 
-                                                                                          (a button could be invoked even if it isn't currently visible)  '''
-main_window.findR(title = "Open Folder", control_type = UIButton).click() ''' however, click will move the mouse to the button location and click it
-                                                                    (sometimes this can be more reliable) '''
-
-# Closing the window and terminating the application
-main_window.close()
-app.terminateApp()
-```
-
-## Authors
-
-ex. Harvey Fretwell
-ex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
-ex. [atomacos](https://github.com/daveenguyen/atomacos)
-ex. [pyAutoGUI](https://github.com/asweigart/pyautogui)
-
-## Version History
-
-- 0.1
-  - Initial Release
-  - 0.1.1
-    - Added UISystemTrayIcon and UIPopupMenu manager
-  - 0.1.4
-    - Fixed some issues with setValue() method on buttons and menus
-  - 0.1.5
-    - Added context managers for better popup menu handling
-
-## Acknowledgments
-
-- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
-- [atomacos](https://github.com/daveenguyen/atomacos)
-- [pyAutoGUI](https://github.com/asweigart/pyautogui)
+# pyUIauto
+
+[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
+[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
+[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)
+[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)
+
+
+| Tests       | Status                                                                                                                  |
+| :---------- | :---------------------------------------------------------------------------------------------------------------------: |
+| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |
+| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |
+
+Python UI Automation library, for cross-platform applications, interfacing through the accessibility API.
+
+## Description
+
+This library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.
+
+## Getting Started
+
+### Dependencies
+
+Python Packages:
+
+- pywinauto (Windows / Linux)
+- atomacos (MacOS)
+- pyautogui
+
+OS Compatibility:
+
+- Windows
+- MacOS
+
+( Currently untested on Linux )
+
+## Example
+
+```python
+# Import the tools needed
+from platform import system
+import os
+from pyuiauto.application import UIApplication
+from pyuiauto.components import UIButton
+
+# Finding the path location of the application
+app_paths = {
+  "Darwin": "/Applications/Visual Studio Code.app",
+  "Windows": os.path.expanduser('~') + "\\AppData\\Local\\Programs\\Microsoft VS Code\\Code.exe"
+}
+
+if system() in app_paths:
+  appPath = app_paths[system()]
+else:
+  raise NotImplementedError("The current OS is not currently supported: " + system())
+
+# Setting up an application template, launching the app, and connecting to it
+app = UIApplication(appName = "Visual Studio Code", appPath = appPath)
+app.launchApp()
+app.connectApp()
+
+# Finding the window component and searching for elements within this window component
+main_window = app.window(title = "Visual Studio Code", timeout = 2)
+main_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() '''  press will invoke a button without manually moving the mouse and clicking it 
+                                                                                          (a button could be invoked even if it isn't currently visible)  '''
+main_window.findR(title = "Open Folder", control_type = UIButton).click() ''' however, click will move the mouse to the button location and click it
+                                                                    (sometimes this can be more reliable) '''
+
+# Closing the window and terminating the application
+main_window.close()
+app.terminateApp()
+```
+
+## Authors
+
+ex. Harvey Fretwell
+
+ex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
+
+ex. [atomacos](https://github.com/daveenguyen/atomacos)
+
+ex. [pyAutoGUI](https://github.com/asweigart/pyautogui)
+
+## Version History
+
+- 0.1
+  - Initial Release
+  - 0.1.1
+    - Added UISystemTrayIcon and UIPopupMenu manager
+  - 0.1.4
+    - Fixed some issues with setValue() method on buttons and menus
+  - 0.1.5
+    - Added context managers for better popup menu handling
+  - 0.1.6
+    - Added isOnTop method for components
+    - Fixed isVisible method for components
+    - Added checks for components existing in helper methods
+  - 0.1.7
+    - Added MacOS compatibility
+    - Fixed getValue method for mac on menu items (with a bit of a work around ... hoping to find a better solution soon)
+    - Fixed menu path select and system tray popup select methods on mac
+
+## Acknowledgments
+
+- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
+- [atomacos](https://github.com/daveenguyen/atomacos)
+- [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

### Comparing `pyUIauto-0.1.6/pyproject.toml` & `pyuiauto-0.1.7/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-[tool.poetry]
-name = "pyUIauto"
-version = "0.1.6"
-description = "Python UI Automation library, for cross-platform applications, interfacing through the accessibility API"
-authors = ["Harvey Fretwell <hgfretwell@gmail.com>"]
-maintainers = ["Harvey Fretwell <hgfretwell@gmail.com>"]
-
-license = "GPL-3.0-only"
-readme = "README.md"
-homepage = "https://github.com/harveyf2801/pyUIauto"
-repository = "https://github.com/harveyf2801/pyUIauto"
-keywords = ["automation", "accessibility", "cross-platform", "ui", "desktop", "pywinauto", "atomac"]
-include = [
-    "LICENSE",
-]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-atomacos = {version = "^3.3.0", platform = "darwin"}
-pywinauto = {version = "^0.6.8", platform = "win32"}
-pyautogui = "0.9.41"
-
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "pyUIauto"
+version = "0.1.7"
+description = "Python UI Automation library, for cross-platform applications, interfacing through the accessibility API"
+authors = ["Harvey Fretwell <hgfretwell@gmail.com>"]
+maintainers = ["Harvey Fretwell <hgfretwell@gmail.com>"]
+
+license = "GPL-3.0-only"
+readme = "README.md"
+homepage = "https://github.com/harveyf2801/pyUIauto"
+repository = "https://github.com/harveyf2801/pyUIauto"
+keywords = ["automation", "accessibility", "cross-platform", "ui", "desktop", "pywinauto", "atomac"]
+include = [
+    "LICENSE",
+]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+atomacos = {version = "^3.3.0", platform = "darwin"}
+pywinauto = {version = "^0.6.8", platform = "win32"}
+pyautogui = "0.9.41"
+importlib-metadata = "^6.6.0"
+pathlib = "^1.0.1"
+
+[tool.poetry.dev-dependencies]
+pytest = "^5.2"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pyUIauto-0.1.6/pyuiauto/base/application.py` & `pyuiauto-0.1.7/pyuiauto/base/application.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,207 +1,197 @@
-# ___MODULES___
-from __future__ import annotations
-import time
-from abc import ABC, abstractmethod
-import logging
-import contextlib
-
-# __MY_MODULES__
-from pyuiauto.components import UIWindow, UIButton, UIMenuItem, UIMenuBarItem
-from pyuiauto.exceptions import ProcessNotFoundError, ElementNotFound
-
-
-# ___CLASSES___
-
-class UISystemTrayIconWrapper(ABC):
-    '''UISystemTrayIconWrapper\n
-    Provides a system tray icon manager to help find the system tray icon for an application\n
-    whether it be hidden within the notification expand window or on the taskbar.'''
-    def __init__(self, app: UIApplicationWrapper):
-        self.app = app
-
-    @abstractmethod
-    def __enter__(self) -> UIButton:
-        'Using a context manager helps to creates the UIButton dynamically.'
-
-    @abstractmethod
-    def __exit__(self, *args) -> None:
-        'Using a context manager helps to dynamically tidy any open windows.'
-    
-class UIPopupMenuWrapper(ABC):
-    '''UIPopupMenuWrapper\n
-    Provides a popup manager for popup windows to help select specific menu item\n
-    and provides a cleanup of popup windows.\n
-    
-    The popup_naming_scheme can vary from app to app however, these are some examples:\n
-        - *the application name*\n
-        - "Context"
-        - "Pop-up"
-    '''
-    def __init__(self, app: UIApplicationWrapper, popup_naming_scheme: str = None) -> None:
-        self.app = app
-        self.win_name = popup_naming_scheme if popup_naming_scheme else app.appName
-        self.current_popup = None
-        self.steps = 0
-
-    @abstractmethod
-    def getMenuItemFromPath(self, *path: str) -> UIMenuItem:
-        '''PopupMenu class get menu item from path method\n
-        Uses the specified path to return a menu item component at [-1] index of the path.'''
-    
-    @abstractmethod
-    def back(self):
-        'Go back a popup menu window to the previous item'
-
-    @abstractmethod
-    def backToRoot(self):
-        'Go back to the root popup menu window'
-    
-    @abstractmethod
-    def __enter__(self) -> UIPopupMenuWrapper:
-        'Using a context manager helps to creates the popup windows dynamically.'
-        
-    @abstractmethod
-    def __exit__(self, *args) -> None:
-        'Using a context manager helps to dynamically tidy any open windows.'
-
-class UIApplicationWrapper(ABC):
-    def __init__(self, appName: str, appPath: str = None) -> None:
-        self.appName = appName
-        self.appPath = appPath
-        self.end_time = 0
-        self.start_time = 0
-
-    @abstractmethod
-    def launchApp(self) -> None:
-        '''Application class launch app method\n
-        Launches the application.'''
-        self.start_time = time.time()
-
-    @abstractmethod
-    def connectApp(self) -> None:
-        '''Application class connect app method\n
-        Connects the application wrapper to the specfied running app.'''
-
-    @abstractmethod
-    def terminateApp(self) -> None:
-        '''Application class terminate app method\n
-        Force quits the application.'''
-        self.end_time = time.time()
-    
-    def getRuntime(self):
-        return self.end_time - self.start_time
-    
-    @abstractmethod
-    def window(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIWindow:
-        '''Application class window method\n
-        Finds a window child component with the specified criteria.
-        Raises an exception if the criteria matches no components (recursive).\n
-        Args:                    
-                    (criteria)
-                    title: the name of the component (of type string)
-
-                    (extra OS specific accessibility API criteria)
-        Returns: 
-                    component: window component wrapped to it's cross compatible custom wrapper of type UIWindowWrapper'''
-    
-    @abstractmethod
-    def windows(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIWindow]:
-        '''Application class windows method\n
-        Finds all window child components with the specified criteria.
-        Raises an exception if the criteria matches > 1 or no components (recursive).\n
-        Args:                    
-                    (criteria)
-                    title: the name of the component (of type string)
-
-                    (extra OS specific accessibility API criteria)
-        Returns: 
-                    components: window components wrapped to it's cross compatible custom wrapper in a list of type UIWindowWrapper'''
-
-    @abstractmethod
-    def isAppAlreadyRunning(self) -> bool:
-        '''Application class is app already running method\n
-        This method checks if the application name is found in already running instances.'''
-
-    @abstractmethod
-    def isAppRunning(self) -> bool:
-        '''Application class is app running method\n
-        This method checks if the application is still running which can help to identify crashes.'''
-
-    @abstractmethod
-    def getSystemTrayIcon(self) -> UISystemTrayIconWrapper:
-        '''Application class get system tray icon method\n
-        Returns the system tray icon button component wrapper.\n
-        (a context manager is required to interact with this component)\n
-        Example:\n
-        with UISystemTrayIcon() as icon:
-            icon.right_click()
-            ...'''
-    
-    @abstractmethod
-    def getPopupMenu(self, popup_naming_scheme: str = None) -> UIPopupMenuWrapper:
-        '''Application class get popup menu method\n
-        Returns the popup menu component wrapper.\n
-        (a context manager is required to interact with this component)\n
-        Example:\n
-        with UIPopupMenu() as popup:
-            item = popup.getMenuItemFromPath("Setup", "Set Sample Rate", "96kHz")
-            ...\n
-        
-        The popup_naming_scheme can vary from app to app however, these are some examples:\n
-        - *the application name* (default)
-        - "Context"
-        - "Pop-up"
-        '''
-
-    @contextlib.contextmanager
-    def systemTrayPopupPath(self, *path: str) -> UIMenuBarItem:
-        '''Application class system tray popup select method\n
-        This method selects menu items after clicking the system tray, from the *args passed in as a path.'''
-        with self.getSystemTrayIcon() as icon:
-            icon.right_click()
-            with self.getPopupMenu() as popup:
-                try:
-                    yield popup.getMenuItemFromPath(*path)
-                except ElementNotFound:
-                    raise ElementNotFound(f"{path} is disabled or not available")
-    
-    @contextlib.contextmanager
-    def menuBarPopupPath(self, window: UIWindow, *path: str) -> UIMenuBarItem:
-        '''Application class menu bar select method\n
-        This method selects menu items on the menubar from the *args passed in as a path.'''
-        try:
-            menuBarItem = window.findFirstR(title=path[0], control_type=UIMenuBarItem)
-            if len(path) == 1:
-                yield menuBarItem
-            
-            menuBarItem.click()
-            with self.getPopupMenu() as popup:
-                yield popup.getMenuItemFromPath(*path[1:])
-        
-        except ElementNotFound:
-                    raise ElementNotFound(f"{path} is disabled or not available")
-
-    @abstractmethod
-    def getCrashReport(self) -> str:
-        '''Application class get crash report method\n
-        Gets all crash reports between the start and end time of the application running.'''
-
-    def relaunchApp(self):
-        '''Application class relaunch app method\n
-        Uses it's context manager __enter__ __exit__ methods to quit and reopen the application.'''
-        self.__exit__()
-        self.launchApp()
-        self.__enter__()
-
-    def __enter__(self) -> UIApplicationWrapper:
-        self.launchApp()
-        self.connectApp()
-        return self
-    
-    def __exit__(self, *args):
-        if not self.isAppRunning():
-            logging.warning(f"The {self.appName} application may have crashed as it was not found in running applications")
-            # logging.error(f"Crash report:\n{self.getCrashReport()}")
-            # raise ProcessNotFoundError(f"The {self.appName} application was not found in running applications")
-        else:
-            self.terminateApp()
+# ___MODULES___
+from __future__ import annotations
+import time
+from abc import ABC, abstractmethod
+import logging
+import contextlib
+from typing import Union
+
+try:
+    from pyautogui import press
+except ImportError: # requires pip install
+        raise ModuleNotFoundError('To install the required modules use pip install pyautogui')
+
+# __MY_MODULES__
+from pyuiauto.components import UIWindow, UIButton, UIMenuItem, UIMenuBarItem
+from pyuiauto.exceptions import ProcessNotFoundError, ElementNotFound
+
+
+# ___CLASSES___
+
+class UISystemTrayIconWrapper(ABC):
+    '''UISystemTrayIconWrapper\n
+    Provides a system tray icon manager to help find the system tray icon for an application\n
+    whether it be hidden within the notification expand window or on the taskbar.'''
+    def __init__(self, app: UIApplicationWrapper):
+        self.app = app
+
+    @abstractmethod
+    def __enter__(self) -> UIButton:
+        'Using a context manager helps to creates the UIButton dynamically.'
+
+    @abstractmethod
+    def __exit__(self, *args) -> None:
+        'Using a context manager helps to dynamically tidy any open windows.'
+    
+    
+class UIPopupMenuWrapper(ABC):
+    '''UIPopupMenuWrapper\n
+    Provides a popup manager for popup windows to help select specific menu item\n
+    and provides a cleanup of popup windows.\n
+    
+    The popup_naming_scheme can vary from app to app however, these are some examples:\n
+        - *the application name*\n
+        - "Context"
+        - "Pop-up"
+    '''
+    def __init__(self, app: UIApplicationWrapper, popup_naming_scheme: str = None) -> None:
+        self.app = app
+        self.win_name = popup_naming_scheme if popup_naming_scheme else app.appName
+        self.current_popup = None
+        self.steps = 0
+
+    @abstractmethod
+    def getMenuItemFromPath(self, *path: str) -> UIMenuItem:
+        '''PopupMenu class get menu item from path method\n
+        Uses the specified path to return a menu item component at [-1] index of the path.'''
+    
+    @abstractmethod
+    def back(self):
+        'Go back a popup menu window to the previous item'
+
+    @abstractmethod
+    def backToRoot(self):
+        'Go back to the root popup menu window'
+    
+    @abstractmethod
+    def __enter__(self) -> UIPopupMenuWrapper:
+        'Using a context manager helps to creates the popup windows dynamically.'
+    
+    @abstractmethod
+    def __exit__(self, *args) -> None:
+        'Using a context manager helps to dynamically tidy any open windows.'
+
+
+class UIApplicationWrapper(ABC):
+    def __init__(self, appName: str, appPath: str = None) -> None:
+        self.appName = appName
+        self.appPath = appPath
+        self.end_time = 0
+        self.start_time = 0
+
+    @abstractmethod
+    def launchApp(self) -> None:
+        '''Application class launch app method\n
+        Launches the application.'''
+        self.start_time = time.time()
+
+    @abstractmethod
+    def connectApp(self) -> None:
+        '''Application class connect app method\n
+        Connects the application wrapper to the specfied running app.'''
+
+    @abstractmethod
+    def terminateApp(self) -> None:
+        '''Application class terminate app method\n
+        Force quits the application.'''
+        self.end_time = time.time()
+    
+    def getRuntime(self):
+        return self.end_time - self.start_time
+    
+    @abstractmethod
+    def window(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIWindow:
+        '''Application class window method\n
+        Finds a window child component with the specified criteria.
+        Raises an exception if the criteria matches no components (recursive).\n
+        Args:                    
+                    (criteria)
+                    title: the name of the component (of type string)
+
+                    (extra OS specific accessibility API criteria)
+        Returns: 
+                    component: window component wrapped to it's cross compatible custom wrapper of type UIWindowWrapper'''
+    
+    @abstractmethod
+    def windows(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIWindow]:
+        '''Application class windows method\n
+        Finds all window child components with the specified criteria.
+        Raises an exception if the criteria matches > 1 or no components (recursive).\n
+        Args:                    
+                    (criteria)
+                    title: the name of the component (of type string)
+
+                    (extra OS specific accessibility API criteria)
+        Returns: 
+                    components: window components wrapped to it's cross compatible custom wrapper in a list of type UIWindowWrapper'''
+
+    @abstractmethod
+    def isAppAlreadyRunning(self) -> bool:
+        '''Application class is app already running method\n
+        This method checks if the application name is found in already running instances.'''
+
+    @abstractmethod
+    def isAppRunning(self) -> bool:
+        '''Application class is app running method\n
+        This method checks if the application is still running which can help to identify crashes.'''
+
+    @abstractmethod
+    def getSystemTrayIcon(self) -> UISystemTrayIconWrapper:
+        '''Application class get system tray icon method\n
+        Returns the system tray icon button component wrapper.\n
+        (a context manager is required to interact with this component)\n
+        Example:\n
+        with UISystemTrayIcon() as icon:
+            icon.right_click()
+            ...'''
+    
+    @abstractmethod
+    def getPopupMenu(self, popup_naming_scheme: str = None) -> UIPopupMenuWrapper:
+        '''Application class get popup menu method\n
+        Returns the popup menu component wrapper.\n
+        (a context manager is required to interact with this component)\n
+        Example:\n
+        with UIPopupMenuWrapper() as popup:
+            item = popup.getMenuItemFromPath("Setup", "Set Sample Rate", "96kHz")
+            ...\n
+        
+        The popup_naming_scheme can vary from app to app however, these are some examples:\n
+        - *the application name* (default)
+        - "Context"
+        - "Pop-up"
+        '''
+
+    @abstractmethod
+    def systemTrayPopupPath(self, *path: str) -> UIMenuItem:
+        '''Application class system tray popup select method\n
+        This method selects menu items after clicking the system tray, from the *args passed in as a path.'''
+    
+    @abstractmethod
+    def menuBarPopupPath(self, window: UIWindow, *path: str) -> Union[UIMenuBarItem, UIMenuItem]:
+        '''Application class menu bar select method\n
+        This method selects menu items on the menubar from the *args passed in as a path.'''
+
+    @abstractmethod
+    def getCrashReport(self) -> str:
+        '''Application class get crash report method\n
+        Gets all crash reports between the start and end time of the application running.'''
+
+    def relaunchApp(self):
+        '''Application class relaunch app method\n
+        Uses it's context manager __enter__ __exit__ methods to quit and reopen the application.'''
+        self.__exit__()
+        self.launchApp()
+        self.__enter__()
+
+    def __enter__(self) -> UIApplicationWrapper:
+        self.launchApp()
+        self.connectApp()
+        return self
+    
+    def __exit__(self, *args):
+        if not self.isAppRunning():
+            logging.warning(f"The {self.appName} application may have crashed as it was not found in running applications")
+            # logging.error(f"Crash report:\n{self.getCrashReport()}")
+            # raise ProcessNotFoundError(f"The {self.appName} application was not found in running applications")
+        else:
+            self.terminateApp()
```

### Comparing `pyUIauto-0.1.6/pyuiauto/base/components.py` & `pyuiauto-0.1.7/pyuiauto/base/components.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,381 +1,392 @@
-# ___MODULES___
-from __future__ import annotations
-from abc import ABC, ABCMeta, abstractmethod
-from typing import Type, Union
-
-# ___CLASSES___
-
-class UIBaseComponentWrapperMeta(ABCMeta):
-    """Metaclass for UIComponentWrapper objects"""
-
-    control_type_to_cls = {}
-
-    def __init__(cls, name, bases, attrs):
-        """Register the control types"""
-
-        if name != "UIBaseComponentWrapper":
-            UIBaseComponentWrapperMeta.control_type_to_cls[cls.native_control_type] = cls
-
-    @staticmethod
-    def find_wrapper(component):
-        """Find the correct wrapper for this UIA component"""
-        raise NotImplementedError
-
-class UIBaseComponentWrapper(object, metaclass=UIBaseComponentWrapperMeta):
-    """
-    Abstract / Default wrapper for User Interface controls.
-
-    All other UI wrappers are derived from this.
-
-    This class wraps a lot of functionality of underlying UI features
-    for working with Mac or Windows.
-
-    Most of the methods apply to every single component type. For example
-    you can click() on any component.
-
-    """
-    
-    def __new__(cls, component):
-        return UIBaseComponentWrapper._create_wrapper(cls, component, UIBaseComponentWrapper)
-    
-    @staticmethod
-    def _create_wrapper(cls_spec, component, myself):
-        """Create a wrapper object according to the specified component"""
-        # only use the meta class to find the wrapper for BaseWrapper
-        # so allow users to force the wrapper if they want
-        
-        if cls_spec != myself:
-            obj = object.__new__(cls_spec)
-            obj.__init__(component)
-            return obj
-
-        new_class = cls_spec.find_wrapper(component)
-        
-        obj = object.__new__(new_class)
-
-        obj.__init__(component)
-
-        return obj
-
-    def __init__(self, component):
-        """
-        Initialize the component
-        """
-        if component:
-            
-            self.component = component
-        else:
-            raise RuntimeError('NULL pointer was used to initialize BaseWrapper')
-    
-    @abstractmethod
-    def setValue(self, value: Union[bool, str, int, float]):
-        'Standard base class set value method (may not currently work on all components).'
-        raise NotImplementedError
-
-    @abstractmethod
-    def getValue(self) -> Union[bool, str, int, float]:
-        'Standard base class get value method (may not currently work on all components).'
-        raise NotImplementedError
-    
-    @abstractmethod
-    def setFocus(self):
-        '''Standard base class set focus method (may not currently work on all components).\n
-        Brings the components root parent window to the top most level (z-index) and sets component as "active".'''
-        raise NotImplementedError
-
-    @abstractmethod
-    def invoke(self):
-        '''Standard base class invoke method (may not currently work on all components).\n
-        Invoke will select / click the component without actual mouse movement
-        (therefore this may work on components that are not visible).'''
-        raise NotImplementedError
-
-    @abstractmethod
-    def click(self):
-        '''Standard base class click method\n
-        Manually performs a mouse movement and clicks the component at it's mid-point.'''
-        raise NotImplementedError
-
-    @abstractmethod
-    def right_click(self):
-        '''Standard base class right click method\n
-        Manually performs a mouse movement and right clicks the component at it's mid-point.'''
-        raise NotImplementedError
-
-    @abstractmethod
-    def isVisible(self) -> bool:
-        '''Standard base class is visible method\n
-        Uses a combination of OS dependant accessibility API checks aswell as comparing the
-        components position against the top most level (z-index) component at this position.'''
-        raise NotImplementedError
-    
-    @abstractmethod
-    def getMidpoint(self) -> tuple[int, int]:
-        '''Standard base class get mid point method\n
-        Finds the components mid-point.\n
-        Returns: 
-                    x: x-position in pixels of type int
-                    y: y-position in pixels of type int'''
-        raise NotImplementedError
-    
-    @abstractmethod
-    def getCoordinates(self) -> tuple[int, int, int, int]:
-        '''Standard base class get coordinates method\n
-        Gets the components rectangular edge positions.\n
-        Returns: 
-                    left: x-position of left top corner in pixels of type int
-                    top: y-position of left top corner in pixels of type int
-                    right: x-position of bottom right corner in pixels of type int
-                    bottom: y-position of bottom right corner in pixels of type int'''
-        raise NotImplementedError
-    
-    @abstractmethod
-    def getSizes(self):
-        '''Standard base class get sizes method\n
-        Gets the components width and height.\n
-        Returns: 
-                    width: width in pixels of type int
-                    height: height in pixels of type int'''
-        raise NotImplementedError
-
-    @abstractmethod
-    def getChildren(self) -> UIBaseComponentWrapper:
-        '''Standard base class get children method\n
-        Gets all of the components children (non recursive).\n
-        Returns: 
-                    children: all children in a list of type UIBaseComponentWrapper
-                    (type should dynamicly wrap to it's cross compatible wrapper)'''
-        raise NotImplementedError
-    
-    @abstractmethod
-    def getDescendants(self) -> UIBaseComponentWrapper:
-        '''Standard base class get descendants method\n
-        Gets all of the components descendants (recursive).\n
-        Returns: 
-                    descendants: all descendants in a list of type UIBaseComponentWrapper
-                    (type should dynamicly wrap to it's cross compatible wrapper)'''
-        raise NotImplementedError
-
-    @abstractmethod
-    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIBaseComponentWrapper]:
-        '''Standard base class find all method\n
-        Gets all of the components children with the specified criteria.
-        Raises an exception if the criteria matches no components (pre order traversal, non recursive).\n
-        Args:
-                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
-                    
-                    (optional criteria)
-                    title: the name of the component (of type string)
-
-                    (extra OS specific accessibility API criteria)
-        Returns: 
-                    components: components dynamicly wrapped to it's cross compatible custom wrapper in a list of type UIBaseComponentWrapper'''
-        raise NotImplementedError
-    
-    @abstractmethod
-    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
-        '''Standard base class find first method\n
-        Gets the first child component with the specified criteria.
-        Raises an exception if the criteria matches no components (pre order traversal, non recursive).\n
-        Args:
-                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
-                    
-                    (optional criteria)
-                    title: the name of the component (of type string)
-
-                    (extra OS specific accessibility API criteria)
-        Returns: 
-                    component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
-        raise NotImplementedError
-    
-    @abstractmethod
-    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIBaseComponentWrapper]:
-        '''Standard base class find all recursive method\n
-        Gets all of the components children with the specified criteria.
-        Raises an exception if the criteria matches no components (pre order traversal, recursive).\n
-        Args:
-                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
-                    
-                    (optional criteria)
-                    title: the name of the component (of type string)
-
-                    (extra OS specific accessibility API criteria)
-        Returns: 
-                    components: components dynamicly wrapped to it's cross compatible custom wrapper in a list of type UIBaseComponentWrapper'''
-        raise NotImplementedError
-    
-    @abstractmethod
-    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
-        '''Standard base class find first recursive method\n
-        Gets the first child component with the specified criteria.
-        Raises an exception if the criteria matches no components (pre order traversal, recursive).\n
-        Args:
-                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
-                    
-                    (optional criteria)
-                    title: the name of the component (of type string)
-
-                    (extra OS specific accessibility API criteria)
-        Returns: 
-                    component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
-        raise NotImplementedError
-    
-    @abstractmethod
-    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
-        '''Standard base class find method\n
-        Finds a child component with the specified criteria.
-        Raises an exception if the criteria matches > 1 or no components (non recursive).\n
-        Args:
-                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
-                    
-                    (optional criteria)
-                    title: the name of the component (of type string)
-
-                    (extra OS specific accessibility API criteria)
-        Returns: 
-                    component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
-        raise NotImplementedError
-
-    @abstractmethod
-    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
-        '''Standard base class find recursive method\n
-        Finds a child component with the specified criteria.
-        Raises an exception if the criteria matches > 1 or no components (recursive).\n
-        Args:
-                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
-                    
-                    (optional criteria)
-                    title: the name of the component (of type string)
-
-                    (extra OS specific accessibility API criteria)
-        Returns: 
-                    component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
-        raise NotImplementedError
-    
-    @classmethod
-    @property
-    @abstractmethod
-    def native_control_type(cls) -> str:
-        'Standard base class control type property (name of the components native control type).'
-        raise NotImplementedError
-    
-    @classmethod
-    @property
-    @abstractmethod
-    def control_type(cls) -> Type:
-        'Standard base class control type property (name of the components control type).'
-        raise NotImplementedError
-    
-    @property
-    @abstractmethod
-    def title(self) -> str:
-        'Standard base class title property (name of the component).'
-        raise NotImplementedError
-
-    # _protected methods
-
-    def _check_element_exists(self, component) -> bool:
-        return not(component is None)
-
-    def _check_elements_exist(self, components) -> bool:
-        return len(components) > 0
-    
-    # def _wrapper_function_from_native(self, component, native_control_type: str) -> UIBaseComponentWrapper:
-    #     '''Wrap objects using their native component type
-    #     '''
-    #     return wrapper_mapping[native_control_type](component)
-    
-    # def _wrapper_function(self, component, control_type: Type) -> UIBaseComponentWrapper:
-    #     '''Wrap objects using the pyUIauto control types\n
-    #     ( also checks if the elements aren't null )
-    #     '''
-    #     return control_type(component) if self._check_element_exists(component) else None
-    
-    # def _list_wrapper_function(self, components, control_type: Type) -> list[UIBaseComponentWrapper]:
-    #     '''Wrap objects using the pyUIauto control types\n
-    #     ( also checks if the elements aren't null )
-    #     '''
-    #     return list(control_type(component) for component in components) if self._check_elements_exist(components) else None
-
-    def __str__(self) -> str:
-        return self.control_type
-
-class UIButtonWrapper():
-    @abstractmethod
-    def press(self):
-        '''Button press method\n
-        Similar to the invoke method, performs a button press without actual mouse movement.
-        (therefore this may work on components that are not visible).'''
-    
-    def toggle(self, value):
-        '''Button toggle method\n
-        Performs a button press if the provided value != current value.
-        (overrides the setValue method)'''
-        return self.press() if self.getValue() != value else None
-
-    def setValue(self, value):
-        return self.toggle(value)
-
-class UIRadioButtonWrapper(): ...
-
-class UITextWrapper(): ...
-
-class UISliderWrapper(): ...
-
-class UIEditWrapper(): ...
-
-class UIMenuWrapper(): ...
-class UIMenuItemWrapper():
-    @abstractmethod
-    def select(self):
-        '''Menu item select method\n
-        Similar to the invoke method, selects a menu item without actual mouse movement.'''
-    
-    def invoke(self):
-        return self.select()
-
-    def toggle(self, value) -> bool:
-        '''Menu item toggle method\n
-        Selects a menu item if the provided value != current value.
-        (overrides the setValue method)'''
-        if self.getValue() != value:
-            self.select()
-            return True
-        else:
-            return False
-    
-    def setValue(self, value):
-        return self.toggle(value)
-
-class UIWindowWrapper():
-    @abstractmethod
-    def moveResize(self, x: int = None, y: int = None, width: int = None, height: int = None):
-        '''Window move resize method\n
-        Moves a windows top left corner to the specified pixel points x, y (if provided)
-        and resizes the window to the specified pixel width, height (if provided)
-        Args:
-                    (optional | default = None)
-                    x: top left corner x-axis in pixels (of type int)
-                    y: top left corner y axis in pixels (of type int)
-                    width: width of the window size in pixels (of type int)
-                    height: height of the window size in pixels (of type int)'''
-
-    @abstractmethod
-    def close(self):
-        '''Window close method to press the close button\n
-        Similar to a button invoke method, selects the window's close button without actual mouse movement.'''
-
-class UIGroupWrapper(): ...
-class UIStaticTextWrapper(): ...
-
-class UIMenuBarWrapper(): ...
-
-class UIProgressBarWrapper(): ...
-
-class UITitleBarWrapper(): ...
-
-# !!! Mac Specific Components !!!
-class UIMenuBarItemWrapper(): ...
-
-
-# wrapper_mapping = {wrapper.native_control_type: wrapper for wrapper in (UIButtonWrapper, UIRadioButtonWrapper, UIMenuWrapper, UIMenuItemWrapper, UIProgressBarWrapper, UITextWrapper, UISliderWrapper, UIEditWrapper, UITitleBarWrapper, UIMenuBarWrapper, UIMenuBarItemWrapper, UIWindowWrapper, UIGroupWrapper, UIStaticTextWrapper)}
+# ___MODULES___
+from __future__ import annotations
+from abc import ABC, ABCMeta, abstractmethod
+from typing import Type, Union
+
+# ___CLASSES___
+
+class UIBaseComponentWrapperMeta(ABCMeta):
+    """Metaclass for UIComponentWrapper objects"""
+
+    control_type_to_cls = {}
+
+    def __init__(cls, name, bases, attrs):
+        """Register the control types"""
+
+        if name != "UIBaseComponentWrapper":
+            UIBaseComponentWrapperMeta.control_type_to_cls[cls.native_control_type] = cls
+
+    @staticmethod
+    def find_wrapper(component):
+        """Find the correct wrapper for this UIA component"""
+        raise NotImplementedError
+
+class UIBaseComponentWrapper(object, metaclass=UIBaseComponentWrapperMeta):
+    """
+    Abstract / Default wrapper for User Interface controls.
+
+    All other UI wrappers are derived from this.
+
+    This class wraps a lot of functionality of underlying UI features
+    for working with Mac or Windows.
+
+    Most of the methods apply to every single component type. For example
+    you can click() on any component.
+
+    """
+    
+    def __new__(cls, component):
+        return UIBaseComponentWrapper._create_wrapper(cls, component, UIBaseComponentWrapper)
+    
+    @staticmethod
+    def _create_wrapper(cls_spec, component, myself):
+        """Create a wrapper object according to the specified component"""
+        # only use the meta class to find the wrapper for BaseWrapper
+        # so allow users to force the wrapper if they want
+        
+        if cls_spec != myself:
+            obj = object.__new__(cls_spec)
+            obj.__init__(component)
+            return obj
+
+        new_class = cls_spec.find_wrapper(component)
+        
+        obj = object.__new__(new_class)
+
+        obj.__init__(component)
+
+        return obj
+
+    def __init__(self, component):
+        """
+        Initialize the component
+        """
+        if component:
+            
+            self.component = component
+        else:
+            raise RuntimeError('NULL pointer was used to initialize BaseWrapper')
+    
+    @abstractmethod
+    def setValue(self, value: Union[bool, str, int, float]):
+        'Standard base class set value method (may not currently work on all components).'
+        raise NotImplementedError
+
+    @abstractmethod
+    def getValue(self) -> Union[bool, str, int, float]:
+        'Standard base class get value method (may not currently work on all components).'
+        raise NotImplementedError
+    
+    @abstractmethod
+    def setFocus(self):
+        '''Standard base class set focus method (may not currently work on all components).\n
+        Brings the components root parent window to the top most level (z-index) and sets component as "active".'''
+        raise NotImplementedError
+
+    @abstractmethod
+    def invoke(self):
+        '''Standard base class invoke method (may not currently work on all components).\n
+        Invoke will select / click the component without actual mouse movement
+        (therefore this may work on components that are not visible).'''
+        raise NotImplementedError
+
+    @abstractmethod
+    def click(self):
+        '''Standard base class click method\n
+        Manually performs a mouse movement and clicks the component at it's mid-point.'''
+        raise NotImplementedError
+
+    @abstractmethod
+    def right_click(self):
+        '''Standard base class right click method\n
+        Manually performs a mouse movement and right clicks the component at it's mid-point.'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def isTopLevel(self) -> bool:
+        '''Standard base class is on top method\n
+        Compares the components position against the top most level (z-index) component at this position.'''
+        raise NotImplementedError
+
+    @abstractmethod
+    def isVisible(self) -> bool:
+        '''Standard base class is visible method\n
+        Uses a OS dependant accessibility API checks.'''
+        raise NotImplementedError
+
+    @abstractmethod
+    def exists(self) -> bool:
+        '''Standard base class exists method\n
+        Uses a OS dependant accessibility API checks.'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def getMidpoint(self) -> tuple[int, int]:
+        '''Standard base class get mid point method\n
+        Finds the components mid-point.\n
+        Returns: 
+                    x: x-position in pixels of type int
+                    y: y-position in pixels of type int'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def getCoordinates(self) -> tuple[int, int, int, int]:
+        '''Standard base class get coordinates method\n
+        Gets the components rectangular edge positions.\n
+        Returns: 
+                    left: x-position of left top corner in pixels of type int
+                    top: y-position of left top corner in pixels of type int
+                    right: x-position of bottom right corner in pixels of type int
+                    bottom: y-position of bottom right corner in pixels of type int'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def getSizes(self):
+        '''Standard base class get sizes method\n
+        Gets the components width and height.\n
+        Returns: 
+                    width: width in pixels of type int
+                    height: height in pixels of type int'''
+        raise NotImplementedError
+
+    @abstractmethod
+    def getChildren(self) -> UIBaseComponentWrapper:
+        '''Standard base class get children method\n
+        Gets all of the components children (non recursive).\n
+        Returns: 
+                    children: all children in a list of type UIBaseComponentWrapper
+                    (type should dynamicly wrap to it's cross compatible wrapper)'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def getDescendants(self) -> UIBaseComponentWrapper:
+        '''Standard base class get descendants method\n
+        Gets all of the components descendants (recursive).\n
+        Returns: 
+                    descendants: all descendants in a list of type UIBaseComponentWrapper
+                    (type should dynamicly wrap to it's cross compatible wrapper)'''
+        raise NotImplementedError
+
+    @abstractmethod
+    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIBaseComponentWrapper]:
+        '''Standard base class find all method\n
+        Gets all of the components children with the specified criteria.
+        Raises an exception if the criteria matches no components (pre order traversal, non recursive).\n
+        Args:
+                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
+                    
+                    (optional criteria)
+                    title: the name of the component (of type string)
+
+                    (extra OS specific accessibility API criteria)
+        Returns: 
+                    components: components dynamicly wrapped to it's cross compatible custom wrapper in a list of type UIBaseComponentWrapper'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
+        '''Standard base class find first method\n
+        Gets the first child component with the specified criteria.
+        Raises an exception if the criteria matches no components (pre order traversal, non recursive).\n
+        Args:
+                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
+                    
+                    (optional criteria)
+                    title: the name of the component (of type string)
+
+                    (extra OS specific accessibility API criteria)
+        Returns: 
+                    component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIBaseComponentWrapper]:
+        '''Standard base class find all recursive method\n
+        Gets all of the components children with the specified criteria.
+        Raises an exception if the criteria matches no components (pre order traversal, recursive).\n
+        Args:
+                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
+                    
+                    (optional criteria)
+                    title: the name of the component (of type string)
+
+                    (extra OS specific accessibility API criteria)
+        Returns: 
+                    components: components dynamicly wrapped to it's cross compatible custom wrapper in a list of type UIBaseComponentWrapper'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
+        '''Standard base class find first recursive method\n
+        Gets the first child component with the specified criteria.
+        Raises an exception if the criteria matches no components (pre order traversal, recursive).\n
+        Args:
+                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
+                    
+                    (optional criteria)
+                    title: the name of the component (of type string)
+
+                    (extra OS specific accessibility API criteria)
+        Returns: 
+                    component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
+        raise NotImplementedError
+    
+    @abstractmethod
+    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
+        '''Standard base class find method\n
+        Finds a child component with the specified criteria.
+        Raises an exception if the criteria matches > 1 or no components (non recursive).\n
+        Args:
+                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
+                    
+                    (optional criteria)
+                    title: the name of the component (of type string)
+
+                    (extra OS specific accessibility API criteria)
+        Returns: 
+                    component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
+        raise NotImplementedError
+
+    @abstractmethod
+    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
+        '''Standard base class find recursive method\n
+        Finds a child component with the specified criteria.
+        Raises an exception if the criteria matches > 1 or no components (recursive).\n
+        Args:
+                    control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
+                    
+                    (optional criteria)
+                    title: the name of the component (of type string)
+
+                    (extra OS specific accessibility API criteria)
+        Returns: 
+                    component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
+        raise NotImplementedError
+    
+    @classmethod
+    @property
+    @abstractmethod
+    def native_control_type(cls) -> str:
+        'Standard base class control type property (name of the components native control type).'
+        raise NotImplementedError
+    
+    @classmethod
+    @property
+    @abstractmethod
+    def control_type(cls) -> Type:
+        'Standard base class control type property (name of the components control type).'
+        raise NotImplementedError
+    
+    @property
+    @abstractmethod
+    def title(self) -> str:
+        'Standard base class title property (name of the component).'
+        raise NotImplementedError
+
+    # _protected methods
+
+    def _check_element_exists(self, component) -> bool:
+        return not(component is None)
+
+    def _check_elements_exist(self, components) -> bool:
+        return len(components) > 0
+    
+    # def _wrapper_function_from_native(self, component, native_control_type: str) -> UIBaseComponentWrapper:
+    #     '''Wrap objects using their native component type
+    #     '''
+    #     return wrapper_mapping[native_control_type](component)
+    
+    # def _wrapper_function(self, component, control_type: Type) -> UIBaseComponentWrapper:
+    #     '''Wrap objects using the pyUIauto control types\n
+    #     ( also checks if the elements aren't null )
+    #     '''
+    #     return control_type(component) if self._check_element_exists(component) else None
+    
+    # def _list_wrapper_function(self, components, control_type: Type) -> list[UIBaseComponentWrapper]:
+    #     '''Wrap objects using the pyUIauto control types\n
+    #     ( also checks if the elements aren't null )
+    #     '''
+    #     return list(control_type(component) for component in components) if self._check_elements_exist(components) else None
+
+    def __str__(self) -> str:
+        return self.control_type
+
+class UIButtonWrapper():
+    @abstractmethod
+    def press(self):
+        '''Button press method\n
+        Similar to the invoke method, performs a button press without actual mouse movement.
+        (therefore this may work on components that are not visible).'''
+    
+    def toggle(self, value):
+        '''Button toggle method\n
+        Performs a button press if the provided value != current value.
+        (overrides the setValue method)'''
+        return self.press() if self.getValue() != value else None
+
+    def setValue(self, value):
+        return self.toggle(value)
+
+class UIRadioButtonWrapper(): ...
+
+class UITextWrapper(): ...
+
+class UISliderWrapper(): ...
+
+class UIEditWrapper(): ...
+
+class UIMenuWrapper(): ...
+class UIMenuItemWrapper():
+    @abstractmethod
+    def select(self):
+        '''Menu item select method\n
+        Similar to the invoke method, selects a menu item without actual mouse movement.'''
+    
+    def invoke(self):
+        return self.select()
+
+    def toggle(self, value) -> bool:
+        '''Menu item toggle method\n
+        Selects a menu item if the provided value != current value.
+        (overrides the setValue method)'''
+        if self.getValue() != value:
+            self.select()
+            return True
+        else:
+            return False
+    
+    def setValue(self, value):
+        return self.toggle(value)
+
+class UIWindowWrapper():
+    @abstractmethod
+    def moveResize(self, x: int = None, y: int = None, width: int = None, height: int = None):
+        '''Window move resize method\n
+        Moves a windows top left corner to the specified pixel points x, y (if provided)
+        and resizes the window to the specified pixel width, height (if provided)
+        Args:
+                    (optional | default = None)
+                    x: top left corner x-axis in pixels (of type int)
+                    y: top left corner y axis in pixels (of type int)
+                    width: width of the window size in pixels (of type int)
+                    height: height of the window size in pixels (of type int)'''
+
+    @abstractmethod
+    def close(self):
+        '''Window close method to press the close button\n
+        Similar to a button invoke method, selects the window's close button without actual mouse movement.'''
+
+class UIGroupWrapper(): ...
+class UIStaticTextWrapper(): ...
+
+class UIMenuBarWrapper(): ...
+
+class UIProgressBarWrapper(): ...
+
+class UITitleBarWrapper(): ...
+
+# !!! Mac Specific Components !!!
+class UIMenuBarItemWrapper(): ...
+
+
+# wrapper_mapping = {wrapper.native_control_type: wrapper for wrapper in (UIButtonWrapper, UIRadioButtonWrapper, UIMenuWrapper, UIMenuItemWrapper, UIProgressBarWrapper, UITextWrapper, UISliderWrapper, UIEditWrapper, UITitleBarWrapper, UIMenuBarWrapper, UIMenuBarItemWrapper, UIWindowWrapper, UIGroupWrapper, UIStaticTextWrapper)}
```

### Comparing `pyUIauto-0.1.6/pyuiauto/wait.py` & `pyuiauto-0.1.7/pyuiauto/wait.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import time
-
-def wait_until_condition(conditional_func, timeout: float = 3, retry_interval: float = 0.01, *func_args, **func_kwargs) -> bool:
-    '''Wait until condition function\n
-    Returns True if the conditional function returns a value that is True before the Timeout is reached.\n
-    However, returns False if the conditional function doesn't return a value that is True before the Timeout is reached.\n
-    Args:
-                    conditional_func: the function to perform on each iteration check
-                    
-                    (optional)
-                    timeout: the timeout max (in seconds) of type float
-                    retry_interval: the delay time (in seconds) of type float between each check
-                    *func_args: the arguments to pass into the conditional function
-                    **func_kwargs: the keyword arguments to pass into the conditional function
-
-        Returns: 
-                    result: value of type bool
-    '''
-    timeafter = time.time() + timeout
-    while time.time() < timeafter:
-        if conditional_func(*func_args, **func_kwargs): return True
-        time.sleep(retry_interval)
-    return False
-
-def wait_until_raise(conditional_func, error: Exception = TimeoutError(), timeout: float = 3, retry_interval: float = 0.01, *func_args, **func_kwargs):
-    '''Wait until raise function\n
-    Returns the value if the conditional function returns a value that is True before the Timeout is reached.\n
-    However, raises an error if the conditional function doesn't return a value that is True before the Timeout is reached.\n
-    Args:
-                    conditional_func: the function to perform on each iteration check
-                    
-                    (optional)
-                    error: the error to raise if a timeout is reached of type exception
-                    timeout: the timeout max (in seconds) of type float
-                    retry_interval: the delay time (in seconds) of type float between each check
-                    *func_args: the arguments to pass into the conditional function
-                    **func_kwargs: the keyword arguments to pass into the conditional function
-
-        Returns: 
-                    result: value of type bool
-    '''
-    timeafter = time.time() + timeout
-    while time.time() < timeafter:
-        result = conditional_func(*func_args, **func_kwargs)
-        if result: return result
-        time.sleep(retry_interval)
+import time
+
+def wait_until_condition(conditional_func, timeout: float = 3, retry_interval: float = 0.01, *func_args, **func_kwargs) -> bool:
+    '''Wait until condition function\n
+    Returns True if the conditional function returns a value that is True before the Timeout is reached.\n
+    However, returns False if the conditional function doesn't return a value that is True before the Timeout is reached.\n
+    Args:
+                    conditional_func: the function to perform on each iteration check
+                    
+                    (optional)
+                    timeout: the timeout max (in seconds) of type float
+                    retry_interval: the delay time (in seconds) of type float between each check
+                    *func_args: the arguments to pass into the conditional function
+                    **func_kwargs: the keyword arguments to pass into the conditional function
+
+        Returns: 
+                    result: value of type bool
+    '''
+    timeafter = time.time() + timeout
+    while time.time() < timeafter:
+        if conditional_func(*func_args, **func_kwargs): return True
+        time.sleep(retry_interval)
+    return False
+
+def wait_until_raise(conditional_func, error: Exception = TimeoutError(), timeout: float = 3, retry_interval: float = 0.01, *func_args, **func_kwargs):
+    '''Wait until raise function\n
+    Returns the value if the conditional function returns a value that is True before the Timeout is reached.\n
+    However, raises an error if the conditional function doesn't return a value that is True before the Timeout is reached.\n
+    Args:
+                    conditional_func: the function to perform on each iteration check
+                    
+                    (optional)
+                    error: the error to raise if a timeout is reached of type exception
+                    timeout: the timeout max (in seconds) of type float
+                    retry_interval: the delay time (in seconds) of type float between each check
+                    *func_args: the arguments to pass into the conditional function
+                    **func_kwargs: the keyword arguments to pass into the conditional function
+
+        Returns: 
+                    result: value of type bool
+    '''
+    timeafter = time.time() + timeout
+    while time.time() < timeafter:
+        result = conditional_func(*func_args, **func_kwargs)
+        if result: return result
+        time.sleep(retry_interval)
     raise error
```

### Comparing `pyUIauto-0.1.6/pyuiauto/win/application.py` & `pyuiauto-0.1.7/pyuiauto/win/application.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,191 +1,221 @@
-#___MODULES___
-from __future__ import annotations
-from typing import Type
-import datetime
-import subprocess
-import logging
-
-# pip installed modules
-try:
-        import pywinauto
-        from pywinauto.application import process_get_modules
-except ImportError: # requires pip install
-        raise ModuleNotFoundError('To install the required modules use pip install pywinauto (Windows ONLY)')
-
-try:
-    from pyautogui import press
-except ImportError: # requires pip install
-        raise ModuleNotFoundError('To install the required modules use pip install pyautogui')
-
-
-#___MY_MODULES___
-from pywinauto.controls.uiawrapper import UIAWrapper
-from pyuiauto.win.components import UIBaseComponent, UIWindow, UIButton, UIMenuItem
-from pyuiauto.base.application import UIApplicationWrapper, UISystemTrayIconWrapper, UIPopupMenuWrapper
-from pyuiauto.exceptions import ElementNotFound, WindowNotFound
-
-class UIBackendExplorer():
-    backend_explorer_app = pywinauto.Application(backend="uia").connect(path="explorer.exe")
-    backend_explorer_app = pywinauto.Application(backend="uia").connect(path="explorer.exe")
-    taskbar: pywinauto.WindowSpecification = backend_explorer_app.window(title="Taskbar", class_name="Shell_TrayWnd")
-
-    try:
-        taskbarExpand = UIButton(taskbar.child_window(title="Show Hidden Icons", class_name="SystemTray.NormalButton").wrapper_object())
-    except:
-        try:
-            taskbarExpand = UIButton(taskbar.child_window(title="Notification Chevron").wrapper_object())
-        except:
-            raise ElementNotFound("Show Hidden Icons not found.")
-        
-backendExplorer = UIBackendExplorer()
-
-class UISystemTrayIcon(UISystemTrayIconWrapper):
-    def __init__(self, app: UIApplicationWrapper):
-        super().__init__(app)
-
-        self._iconHidden = False
-        
-        try:
-            self._getIcon(backendExplorer.taskbar)
-        except:
-                self.__systrayExpandWindow = None
-                self._iconHidden = True
-    
-    def _getIcon(self, parent: pywinauto.WindowSpecification) -> UIButton:
-        icon = parent.child_window(title_re=f".* {self.app.appName}", control_type="Button", found_index=0)
-        icon.wait('exists', timeout=2)
-        icon.wrapper_object()
-        return UIButton(icon)
-
-    def __openSystemTrayExpand(self) -> pywinauto.WindowSpecification:
-        # Open the system tray
-        backendExplorer.taskbarExpand.invoke()
-
-        # Select the audient icon
-        try:
-            systray = pywinauto.Application(backend="uia").connect(class_name="TopLevelWindowForOverflowXamlIsland")
-            systrayWindow = systray.window(class_name="TopLevelWindowForOverflowXamlIsland")
-            
-        except:
-            try:
-                systray = pywinauto.Application(backend="uia").connect(class_name="NotifyIconOverflowWindow")
-                systrayWindow = systray.window(class_name="NotifyIconOverflowWindow")
-                
-            except:
-                raise WindowNotFound("Notification Overflow Window not found.")
-
-        systrayWindow.wait("visible")
-        return systrayWindow
-
-    def __closeNotifictionExpand(self) -> None:
-        # Close the system tray
-        if self.__systrayExpandWindow.exists() and self.__systrayExpandWindow.is_visible():
-            backendExplorer.taskbarExpand.invoke() # pyautogui.press("esc") will also work for closing popup menu windows
-            self.__systrayExpandWindow.wait_not("visible")
-
-    def __enter__(self) -> UIButton:
-        if self._iconHidden:
-            try:
-                self.__systrayExpandWindow = self.__openSystemTrayExpand()
-                return self._getIcon(self.__systrayExpandWindow)
-            except: raise ElementNotFound("System Tray Icon not found.")
-        
-        return self._getIcon(backendExplorer.taskbar)
-    
-    def __exit__(self, *args):
-        if self._iconHidden:
-            self.__closeNotifictionExpand()
-
-class UIPopupMenu(UIPopupMenuWrapper):
-    def __init__(self, app: UIApplicationWrapper, popup_naming_scheme: str) -> None:
-        super().__init__(app, popup_naming_scheme)
-    
-    def getMenuItemFromPath(self, *path: str) -> UIMenuItem:
-        current_item = None
-
-        for count, i in enumerate(path):
-            self.current_popup = self.app.window(title=self.win_name, found_index=0)
-            current_item = self.current_popup.findFirstR(title=i, control_type=UIMenuItem)
-            if count != len(path)-1:
-                current_item.invoke()
-            self.steps += 1
-        
-        return current_item
-
-    def back(self):
-        if self.steps > 0:
-            press("left")
-            self.steps -= 1
-
-    def backToRoot(self):
-        for i in range(self.steps):
-            press("left")
-            self.steps -= 1
-    
-    def __enter__(self) -> UIPopupMenu:
-        return self
-        
-    def __exit__(self, *args) -> None:
-        if self.current_popup.isVisible():
-            press("esc")
-
-#___DEFINING_NATIVE_METHODS___
-class UIApplication(UIApplicationWrapper):
-
-    def launchApp(self) -> None:
-        pywinauto.Application().start(self.appPath)
-    
-    def connectApp(self) -> None:
-        self._app = pywinauto.Application(backend="uia", allow_magic_lookup=False).connect(title=self.appName, path=f"{self.appName}.exe")
-    
-    def terminateApp(self) -> None:
-        self._app.kill()
-    
-    def window(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIWindow:
-        try:
-            window = self._app.window(**criteria)
-            window.wait('exists', timeout=timeout, retry_interval=retry_interval)
-            return UIWindow(window.wrapper_object())
-        except pywinauto.timings.TimeoutError:
-             raise WindowNotFound
-    
-    def windows(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIWindow]:
-        try:
-            windows = list(UIWindow(window) for window in self._app.windows(**criteria))
-            if len(windows) == 0:
-                raise WindowNotFound
-            return windows
-        except pywinauto.timings.TimeoutError:
-             raise WindowNotFound
-    
-    def isAppAlreadyRunning(self):
-        for module in process_get_modules():
-            if self.appPath == module[1]:
-                 return True
-        return False
-
-    def isAppRunning(self):
-        return self._app.is_process_running()
-
-    def getSystemTrayIcon(self) -> UISystemTrayIcon:
-        return UISystemTrayIcon(self)
-    
-    def getPopupMenu(self, popup_naming_scheme: str = None) -> UIPopupMenu:
-        return UIPopupMenu(self, popup_naming_scheme)
-    
-    def getCrashReport(self):
-        # Convert epoch timestamp to a datetime object
-        start_datetime = datetime.datetime.fromtimestamp(self.start_time)
-        end_datetime = datetime.datetime.fromtimestamp(self.end_time)
-
-        # Format datetime object as a string in the required format
-        start_time = start_datetime.strftime('%Y-%m-%dT%H:%M:%S')
-        end_time = end_datetime.strftime('%Y-%m-%dT%H:%M:%S')
-
-        command = f"powershell.exe Get-WinEvent -FilterHashtable @{{Logname='Application';Data='{self.appName}';StartTime='{start_time}';EndTime='{end_time}'}}"
-        result = subprocess.run(command, capture_output=True, text=True)
-
-        if result.returncode == 0:
-            return result.stdout
-        else:
-            return result.stderr
+#___MODULES___
+from __future__ import annotations
+from typing import Type
+import datetime
+import subprocess
+import logging
+import contextlib
+from typing import Union
+
+# pip installed modules
+try:
+        import pywinauto
+        from pywinauto.application import process_get_modules
+except ImportError: # requires pip install
+        raise ModuleNotFoundError('To install the required modules use pip install pywinauto (Windows ONLY)')
+
+try:
+    from pyautogui import press
+except ImportError: # requires pip install
+        raise ModuleNotFoundError('To install the required modules use pip install pyautogui')
+
+
+#___MY_MODULES___
+from pywinauto.controls.uiawrapper import UIAWrapper
+from pyuiauto.win.components import UIBaseComponent, UIWindow, UIButton, UIMenuItem, UIMenuBarItem
+from pyuiauto.base.application import UIApplicationWrapper, UISystemTrayIconWrapper, UIPopupMenuWrapper
+from pyuiauto.exceptions import ElementNotFound, WindowNotFound
+
+class UIBackendExplorer():
+    backend_explorer_app = pywinauto.Application(backend="uia").connect(path="explorer.exe")
+    backend_explorer_app = pywinauto.Application(backend="uia").connect(path="explorer.exe")
+    taskbar: pywinauto.WindowSpecification = backend_explorer_app.window(title="Taskbar", class_name="Shell_TrayWnd")
+
+    try:
+        taskbarExpand = UIButton(taskbar.child_window(title="Show Hidden Icons", class_name="SystemTray.NormalButton").wrapper_object())
+    except:
+        try:
+            taskbarExpand = UIButton(taskbar.child_window(title="Notification Chevron").wrapper_object())
+        except:
+            raise ElementNotFound("Show Hidden Icons not found.")
+        
+backendExplorer = UIBackendExplorer()
+
+class UISystemTrayIcon(UISystemTrayIconWrapper):
+    def __init__(self, app: UIApplicationWrapper):
+        super().__init__(app)
+
+        self._iconHidden = False
+        
+        try:
+            self._getIcon(backendExplorer.taskbar)
+        except:
+                self.__systrayExpandWindow = None
+                self._iconHidden = True
+    
+    def _getIcon(self, parent: pywinauto.WindowSpecification) -> UIButton:
+        icon = parent.child_window(title_re=f".* {self.app.appName}", control_type="Button", found_index=0)
+        icon.wait('exists', timeout=2)
+        icon.wrapper_object()
+        return UIButton(icon)
+
+    def __openSystemTrayExpand(self) -> pywinauto.WindowSpecification:
+        # Open the system tray
+        backendExplorer.taskbarExpand.invoke()
+
+        # Select the audient icon
+        try:
+            systray = pywinauto.Application(backend="uia").connect(class_name="TopLevelWindowForOverflowXamlIsland")
+            systrayWindow = systray.window(class_name="TopLevelWindowForOverflowXamlIsland")
+            
+        except:
+            try:
+                systray = pywinauto.Application(backend="uia").connect(class_name="NotifyIconOverflowWindow")
+                systrayWindow = systray.window(class_name="NotifyIconOverflowWindow")
+                
+            except:
+                raise WindowNotFound("Notification Overflow Window not found.")
+
+        systrayWindow.wait("visible")
+        return systrayWindow
+
+    def __closeNotifictionExpand(self) -> None:
+        # Close the system tray
+        if self.__systrayExpandWindow.exists() and self.__systrayExpandWindow.is_visible():
+            backendExplorer.taskbarExpand.invoke() # pyautogui.press("esc") will also work for closing popup menu windows
+            self.__systrayExpandWindow.wait_not("visible")
+
+    def __enter__(self) -> UIButton:
+        if self._iconHidden:
+            try:
+                self.__systrayExpandWindow = self.__openSystemTrayExpand()
+                return self._getIcon(self.__systrayExpandWindow)
+            except: raise ElementNotFound("System Tray Icon not found.")
+        
+        return self._getIcon(backendExplorer.taskbar)
+    
+    def __exit__(self, *args):
+        if self._iconHidden:
+            self.__closeNotifictionExpand()
+
+
+class UIPopupMenu(UIPopupMenuWrapper):
+    def __init__(self, app: UIApplicationWrapper, popup_naming_scheme: str = None) -> None:
+        super().__init__(app, popup_naming_scheme)
+
+    def getMenuItemFromPath(self, *path: str) -> UIMenuItem:
+        current_item = None
+
+        for count, i in enumerate(path):
+            self.current_popup = self.app.window(title=self.win_name, found_index=0)
+            current_item = self.current_popup.findFirstR(title=i, control_type=UIMenuItem)
+            if count != len(path)-1:
+                current_item.invoke()
+            self.steps += 1
+        
+        return current_item
+    
+    def back(self):
+        if self.steps > 0:
+            press("left")
+            self.steps -= 1
+
+    def backToRoot(self):
+        for i in range(self.steps):
+            press("left")
+            self.steps -= 1
+    
+    def __enter__(self) -> UIPopupMenu:
+        return self
+        
+    def __exit__(self, *args) -> None:
+        if self.current_popup.isVisible():
+            press("esc")
+
+
+#___DEFINING_NATIVE_METHODS___
+class UIApplication(UIApplicationWrapper):
+
+    def launchApp(self) -> None:
+        pywinauto.Application().start(self.appPath)
+    
+    def connectApp(self) -> None:
+        self._app = pywinauto.Application(backend="uia", allow_magic_lookup=False).connect(title=self.appName, path=self.appPath)
+    
+    def terminateApp(self) -> None:
+        self._app.kill()
+    
+    def window(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIWindow:
+        try:
+            window = self._app.window(**criteria)
+            window.wait('exists', timeout=timeout, retry_interval=retry_interval)
+            return UIWindow(window.wrapper_object())
+        except pywinauto.timings.TimeoutError:
+             raise WindowNotFound
+    
+    def windows(self, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIWindow]:
+        try:
+            windows = list(UIWindow(window) for window in self._app.windows(**criteria))
+            if len(windows) == 0:
+                raise WindowNotFound
+            return windows
+        except pywinauto.timings.TimeoutError:
+             raise WindowNotFound
+    
+    def isAppAlreadyRunning(self):
+        for module in process_get_modules():
+            if self.appPath == module[1]:
+                 return True
+        return False
+
+    def isAppRunning(self):
+        return self._app.is_process_running()
+    
+    def getCrashReport(self):
+        # Convert epoch timestamp to a datetime object
+        start_datetime = datetime.datetime.fromtimestamp(self.start_time)
+        end_datetime = datetime.datetime.fromtimestamp(self.end_time)
+
+        # Format datetime object as a string in the required format
+        start_time = start_datetime.strftime('%Y-%m-%dT%H:%M:%S')
+        end_time = end_datetime.strftime('%Y-%m-%dT%H:%M:%S')
+
+        command = f"powershell.exe Get-WinEvent -FilterHashtable @{{Logname='Application';Data='{self.appName}';StartTime='{start_time}';EndTime='{end_time}'}}"
+        result = subprocess.run(command, capture_output=True, text=True)
+
+        if result.returncode == 0:
+            return result.stdout
+        else:
+            return result.stderr
+    
+    def getPopupMenu(self, popup_naming_scheme: str = None) -> UIPopupMenu:
+        return UIPopupMenu(self, popup_naming_scheme)
+    
+    def getSystemTrayIcon(self) -> UISystemTrayIcon:
+        return UISystemTrayIcon(self)
+
+    @contextlib.contextmanager
+    def systemTrayPopupPath(self, *path: str) -> UIMenuItem:
+        with self.getSystemTrayIcon() as icon:
+            icon.right_click()
+        
+            with self.getPopupMenu() as popup:
+                try:
+
+                    yield popup.getMenuItemFromPath(*path)
+                except ElementNotFound:
+                    raise ElementNotFound(f"{path} is disabled or not available")
+    
+    @contextlib.contextmanager
+    def menuBarPopupPath(self, window: UIWindow, *path: str) -> Union[UIMenuBarItem, UIMenuItem]:
+        try:
+            menuBarItem = window.findFirstR(title=path[0], control_type=UIMenuBarItem)
+            if len(path) == 1:
+                yield menuBarItem
+            
+            menuBarItem.click()
+            with self.getPopupMenu() as popup:
+                yield popup.getMenuItemFromPath(*path[1:])
+        
+        except ElementNotFound:
+                    raise ElementNotFound(f"{path} is disabled or not available")
```

### Comparing `pyUIauto-0.1.6/pyuiauto/win/components.py` & `pyuiauto-0.1.7/pyuiauto/win/components.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,321 +1,324 @@
-#___MODULES___
-from __future__ import annotations
-from typing import Type
-import time
-from abc import ABCMeta
-import logging
-
-# pip installed modules
-try:
-        from pywinauto.controls.uiawrapper import UIAWrapper
-        from pywinauto.keyboard import send_keys
-        from pywinauto.timings import wait_until
-        from pywinauto.uia_defines import NoPatternInterfaceError
-except ImportError: # requires pip install
-        raise ModuleNotFoundError('To install the required modules use pip install pywinauto (Windows ONLY)')
-
-
-#___MY_MODULES___
-from pyuiauto.exceptions import ElementNotFound
-from pyuiauto.base.components import *
-
-
-#___DEFINING_NATIVE_WRAPPER_META___
-
-class UIBaseComponentMeta(UIBaseComponentWrapperMeta):
-    """Metaclass for UIComponent objects"""
-
-    control_type_to_cls = {}
-
-    def __init__(cls, name, bases, attrs):
-        """Register the control types"""
-
-        UIBaseComponentWrapperMeta.__init__(cls, name, bases, attrs)
-
-        if name != "UIBaseComponent":
-            UIBaseComponentMeta.control_type_to_cls[cls.native_control_type] = cls
-
-    @staticmethod
-    def find_wrapper(component):
-        """Find the correct wrapper for this UIA component"""
-        # Set a general wrapper by default
-        wrapper_match = UIBaseComponent
-
-        # Check for a more specific wrapper in the registry
-        control_type = component.element_info.control_type
-
-        if control_type in UIBaseComponentWrapperMeta.control_type_to_cls:
-            wrapper_match = UIBaseComponentWrapperMeta.control_type_to_cls[control_type]
-        else:
-            raise NotImplementedError(f"{component} doesn't have an implemented wrapper")
-
-        return wrapper_match
-
-
-
-
-
-
-#___DEFINING_NATIVE_METHODS___
-
-class UIBaseComponent(UIBaseComponentWrapper, metaclass=UIBaseComponentMeta):
-
-    def __new__(cls, component: UIAWrapper):
-        """Construct the control wrapper"""
-        return super(UIBaseComponent, cls)._create_wrapper(cls, component, UIBaseComponent)
-
-    # -----------------------------------------------------------
-    def __init__(self, component: UIAWrapper):
-        UIBaseComponentWrapper.__init__(self, component)
-
-    def getValue(self):
-        return self.component.iface_value
-    
-    def setValue(self, value):
-        self.component.set_value(value)
-    
-    def setFocus(self):
-        self.component.set_focus()
-    
-    def invoke(self):
-        self.component.invoke()
-
-    def click(self):
-        self.component.click_input()
-    
-    def right_click(self):
-        self.component.right_click_input()
-    
-    def isTopLevel(self):
-        x, y, _, _= self.getCoordinates()
-        return self.component.from_point(x, y).element_info.name == self.component.element_info.name
-
-    def isVisible(self):
-        return self.component.is_visible()
-    
-    def getMidpoint(self):
-        return self.component.rectangle().mid_point()
-    
-    def getCoordinates(self):
-        rectangle = self.component.rectangle()
-        return rectangle.left, rectangle.top, rectangle.right, rectangle.bottom
-    
-    def getSizes(self):
-        rectangle = self.component.rectangle()
-        return rectangle.width(), rectangle.height()
-    
-    def getChildren(self):
-        return list(UIBaseComponent(component) for component in self.component.children())
-
-    def getDescendants(self):
-        return list(UIBaseComponent(component) for component in self.component.descendants())
-    
-    def _wait_find(self, function, check_function, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        timeafter = time.time() + timeout
-        while time.time() < timeafter:
-            item = function(control_type=control_type.native_control_type, **criteria)
-            item_check = check_function(item)
-            if item_check:
-                if type(item) == list:
-                    return list(UIBaseComponent(i) for i in item)
-                else:
-                    return UIBaseComponent(item)
-            time.sleep(retry_interval)
-        raise ElementNotFound(f"CheckFunction returned: Element - ControlType: {control_type.native_control_type} - {criteria} - not found after {timeout} seconds")
-        
-    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        return self._wait_find(function=self.component.children,
-                        check_function=self._check_elements_exist,
-                        control_type=control_type,
-                        timeout=timeout,
-                        retry_interval=retry_interval,
-                        **criteria)
-    
-    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        return self.findAll(control_type, timeout, retry_interval, **criteria)[0]
-
-    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        items = self.findAll(control_type, timeout, retry_interval, **criteria)
-        
-        if len(items) > 1:
-            raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
-
-        return items[0]
-    
-    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        return self._wait_find(function=self.component.descendants,
-                        check_function=self._check_elements_exist,
-                        control_type=control_type,
-                        timeout=timeout,
-                        retry_interval=retry_interval,
-                        **criteria)
-    
-    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        return self.findAllR(control_type, timeout, retry_interval, **criteria)[0]
-
-    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
-        items = self.findAllR(control_type, timeout, retry_interval, **criteria)
-        
-        if len(items) > 1:
-            raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
-
-        return items[0]
-    
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return None
-    
-    @classmethod
-    @property
-    def control_type(cls) -> Type:
-        return type(cls)
-    
-    @property
-    def title(self):
-        return self.component.element_info.name
-    
-    
-
-class UIButton(UIButtonWrapper, UIBaseComponent):
-    native_control_type: str = "Button"
-
-    def getValue(self):
-        return self.component.get_toggle_state()
-    
-    def press(self):
-        self.component.click()
-    
-    def setValue(self, value):
-        return super().setValue(value)
-
-class UIRadioButton(UIRadioButtonWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "RadioButton"
-
-class UIText(UITextWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "Text"
-    
-class UISlider(UISliderWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "Slider"
-
-    def getValue(self):
-        return self.component.value()
-
-class UIEdit(UIEditWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "Edit"
-
-    def getValue(self):
-        return self.component.get_value()
-    
-    def setValue(self, value):
-        self.component.set_focus()
-        self.component.invoke()
-        send_keys(str(value) + "{ENTER}")
-
-class UIMenu(UIMenuWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "Menu"
-    
-class UIMenuItem(UIMenuItemWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "MenuItem"
-
-    def getValue(self):
-        try:
-            return bool(self.component.iface_toggle)
-        except NoPatternInterfaceError:
-            return False
-
-    def select(self):
-        self.component.select()
-    
-    def setValue(self, value):
-        return super().setValue(value)
-
-class UIWindow(UIWindowWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "Window"
-    
-    def moveResize(self, x=None, y=None, width=None, height=None):
-        cur_rect = self.component.rectangle()
-
-        # if no X is specified - so use current coordinate
-        if x is None:
-            x = cur_rect.left
-
-        # if no Y is specified - so use current coordinate
-        if y is None:
-            y = cur_rect.top
-
-        # if no width is specified - so use current width
-        if width is None:
-            width = cur_rect.width()
-
-        # if no height is specified - so use current height
-        if height is None:
-            height = cur_rect.height()
-
-        # ask for the window to be moved
-        self.component.iface_transform.Move(x, y)
-        self.component.iface_transform.Resize(width, height)
-
-    def close(self):
-        self.component.close()
-
-class UIGroup(UIGroupWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "Custom"
-
-class UIStaticText(UIStaticTextWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "Text"
-
-    def getValue(self):
-        return self.component.window_text()
-
-class UITitleBar(UITitleBarWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "TitleBar"
-        
-class UIMenuBar(UIMenuBarWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "MenuBar"
-
-class UIProgressBar(UIProgressBarWrapper, UIBaseComponent):
-    @classmethod
-    @property
-    def native_control_type(cls) -> str:
-        return "ProgressBar"
-
-    def getValue(self):
-        return int(self.component.legacy_properties()['Value'])
-
-# !!! Mac Specific !!!
-
+#___MODULES___
+from __future__ import annotations
+from typing import Type
+import time
+from abc import ABCMeta
+import logging
+
+# pip installed modules
+try:
+        from pywinauto.controls.uiawrapper import UIAWrapper
+        from pywinauto.keyboard import send_keys
+        from pywinauto.timings import wait_until
+        from pywinauto.uia_defines import NoPatternInterfaceError
+except ImportError: # requires pip install
+        raise ModuleNotFoundError('To install the required modules use pip install pywinauto (Windows ONLY)')
+
+
+#___MY_MODULES___
+from pyuiauto.exceptions import ElementNotFound
+from pyuiauto.base.components import *
+
+
+#___DEFINING_NATIVE_WRAPPER_META___
+
+class UIBaseComponentMeta(UIBaseComponentWrapperMeta):
+    """Metaclass for UIComponent objects"""
+
+    control_type_to_cls = {}
+
+    def __init__(cls, name, bases, attrs):
+        """Register the control types"""
+
+        UIBaseComponentWrapperMeta.__init__(cls, name, bases, attrs)
+
+        if name != "UIBaseComponent":
+            UIBaseComponentMeta.control_type_to_cls[cls.native_control_type] = cls
+
+    @staticmethod
+    def find_wrapper(component):
+        """Find the correct wrapper for this UIA component"""
+        # Set a general wrapper by default
+        wrapper_match = UIBaseComponent
+
+        # Check for a more specific wrapper in the registry
+        control_type = component.element_info.control_type
+
+        if control_type in UIBaseComponentWrapperMeta.control_type_to_cls:
+            wrapper_match = UIBaseComponentWrapperMeta.control_type_to_cls[control_type]
+        else:
+            raise NotImplementedError(f"{component} doesn't have an implemented wrapper")
+
+        return wrapper_match
+
+
+
+
+
+
+#___DEFINING_NATIVE_METHODS___
+
+class UIBaseComponent(UIBaseComponentWrapper, metaclass=UIBaseComponentMeta):
+
+    def __new__(cls, component: UIAWrapper):
+        """Construct the control wrapper"""
+        return super(UIBaseComponent, cls)._create_wrapper(cls, component, UIBaseComponent)
+
+    # -----------------------------------------------------------
+    def __init__(self, component: UIAWrapper):
+        UIBaseComponentWrapper.__init__(self, component)
+
+    def getValue(self):
+        return self.component.iface_value
+    
+    def setValue(self, value):
+        self.component.set_value(value)
+    
+    def setFocus(self):
+        self.component.set_focus()
+    
+    def invoke(self):
+        self.component.invoke()
+
+    def click(self):
+        self.component.click_input()
+    
+    def right_click(self):
+        self.component.right_click_input()
+    
+    def isTopLevel(self):
+        x, y, _, _= self.getCoordinates()
+        return self.component.from_point(x, y).element_info.name == self.component.element_info.name
+
+    def isVisible(self):
+        return self.component.is_visible()
+    
+    def exists(self):
+        raise self.isVisible()
+    
+    def getMidpoint(self):
+        return self.component.rectangle().mid_point()
+    
+    def getCoordinates(self):
+        rectangle = self.component.rectangle()
+        return rectangle.left, rectangle.top, rectangle.right, rectangle.bottom
+    
+    def getSizes(self):
+        rectangle = self.component.rectangle()
+        return rectangle.width(), rectangle.height()
+    
+    def getChildren(self):
+        return list(UIBaseComponent(component) for component in self.component.children())
+
+    def getDescendants(self):
+        return list(UIBaseComponent(component) for component in self.component.descendants())
+    
+    def _wait_find(self, function, check_function, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        timeafter = time.time() + timeout
+        while time.time() < timeafter:
+            item = function(control_type=control_type.native_control_type, **criteria)
+            item_check = check_function(item)
+            if item_check:
+                if type(item) == list:
+                    return list(UIBaseComponent(i) for i in item)
+                else:
+                    return UIBaseComponent(item)
+            time.sleep(retry_interval)
+        raise ElementNotFound(f"CheckFunction returned: Element - ControlType: {control_type.native_control_type} - {criteria} - not found after {timeout} seconds")
+        
+    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        return self._wait_find(function=self.component.children,
+                        check_function=self._check_elements_exist,
+                        control_type=control_type,
+                        timeout=timeout,
+                        retry_interval=retry_interval,
+                        **criteria)
+    
+    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        return self.findAll(control_type, timeout, retry_interval, **criteria)[0]
+
+    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        items = self.findAll(control_type, timeout, retry_interval, **criteria)
+        
+        if len(items) > 1:
+            raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
+
+        return items[0]
+    
+    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        return self._wait_find(function=self.component.descendants,
+                        check_function=self._check_elements_exist,
+                        control_type=control_type,
+                        timeout=timeout,
+                        retry_interval=retry_interval,
+                        **criteria)
+    
+    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        return self.findAllR(control_type, timeout, retry_interval, **criteria)[0]
+
+    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
+        items = self.findAllR(control_type, timeout, retry_interval, **criteria)
+        
+        if len(items) > 1:
+            raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
+
+        return items[0]
+    
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return None
+    
+    @classmethod
+    @property
+    def control_type(cls) -> Type:
+        return type(cls)
+    
+    @property
+    def title(self):
+        return self.component.element_info.name
+    
+    
+
+class UIButton(UIButtonWrapper, UIBaseComponent):
+    native_control_type: str = "Button"
+
+    def getValue(self):
+        return self.component.get_toggle_state()
+    
+    def press(self):
+        self.component.click()
+    
+    def setValue(self, value):
+        return super().setValue(value)
+
+class UIRadioButton(UIRadioButtonWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "RadioButton"
+
+class UIText(UITextWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Text"
+    
+class UISlider(UISliderWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Slider"
+
+    def getValue(self):
+        return self.component.value()
+
+class UIEdit(UIEditWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Edit"
+
+    def getValue(self):
+        return self.component.get_value()
+    
+    def setValue(self, value):
+        self.component.set_focus()
+        self.component.invoke()
+        send_keys(str(value) + "{ENTER}")
+
+class UIMenu(UIMenuWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Menu"
+    
+class UIMenuItem(UIMenuItemWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "MenuItem"
+
+    def getValue(self):
+        try:
+            return bool(self.component.iface_toggle)
+        except NoPatternInterfaceError:
+            return False
+
+    def select(self):
+        self.component.select()
+    
+    def setValue(self, value):
+        return super().setValue(value)
+
+class UIWindow(UIWindowWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Window"
+    
+    def moveResize(self, x=None, y=None, width=None, height=None):
+        cur_rect = self.component.rectangle()
+
+        # if no X is specified - so use current coordinate
+        if x is None:
+            x = cur_rect.left
+
+        # if no Y is specified - so use current coordinate
+        if y is None:
+            y = cur_rect.top
+
+        # if no width is specified - so use current width
+        if width is None:
+            width = cur_rect.width()
+
+        # if no height is specified - so use current height
+        if height is None:
+            height = cur_rect.height()
+
+        # ask for the window to be moved
+        self.component.iface_transform.Move(x, y)
+        self.component.iface_transform.Resize(width, height)
+
+    def close(self):
+        self.component.close()
+
+class UIGroup(UIGroupWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Custom"
+
+class UIStaticText(UIStaticTextWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "Text"
+
+    def getValue(self):
+        return self.component.window_text()
+
+class UITitleBar(UITitleBarWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "TitleBar"
+        
+class UIMenuBar(UIMenuBarWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "MenuBar"
+
+class UIProgressBar(UIProgressBarWrapper, UIBaseComponent):
+    @classmethod
+    @property
+    def native_control_type(cls) -> str:
+        return "ProgressBar"
+
+    def getValue(self):
+        return int(self.component.legacy_properties()['Value'])
+
+# !!! Mac Specific !!!
+
 class UIMenuBarItem(UIMenuItem, UIBaseComponent): ...
```

### Comparing `pyUIauto-0.1.6/setup.py` & `pyuiauto-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['pyuiauto', 'pyuiauto.base', 'pyuiauto.mac', 'pyuiauto.win']
 
 package_data = \
-{'': ['*'], 'pyuiauto': ['.git/*', '.git/hooks/*', '.git/info/*']}
+{'': ['*']}
 
 install_requires = \
-['pyautogui==0.9.41']
+['importlib-metadata>=6.6.0,<7.0.0',
+ 'pathlib>=1.0.1,<2.0.0',
+ 'pyautogui==0.9.41']
 
 extras_require = \
 {':sys_platform == "darwin"': ['atomacos>=3.3.0,<4.0.0'],
  ':sys_platform == "win32"': ['pywinauto>=0.6.8,<0.7.0']}
 
 setup_kwargs = {
     'name': 'pyuiauto',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Python UI Automation library, for cross-platform applications, interfacing through the accessibility API',
-    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\nex. [atomacos](https://github.com/daveenguyen/atomacos)\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.4\n    - Fixed some issues with setValue() method on buttons and menus\n  - 0.1.5\n    - Added context managers for better popup menu handling\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
+    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\n\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n\nex. [atomacos](https://github.com/daveenguyen/atomacos)\n\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n  - 0.1.4\n    - Fixed some issues with setValue() method on buttons and menus\n  - 0.1.5\n    - Added context managers for better popup menu handling\n  - 0.1.6\n    - Added isOnTop method for components\n    - Fixed isVisible method for components\n    - Added checks for components existing in helper methods\n  - 0.1.7\n    - Added MacOS compatibility\n    - Fixed getValue method for mac on menu items (with a bit of a work around ... hoping to find a better solution soon)\n    - Fixed menu path select and system tray popup select methods on mac\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
     'author': 'Harvey Fretwell',
     'author_email': 'hgfretwell@gmail.com',
     'maintainer': 'Harvey Fretwell',
     'maintainer_email': 'hgfretwell@gmail.com',
     'url': 'https://github.com/harveyf2801/pyUIauto',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyUIauto-0.1.6/PKG-INFO` & `pyuiauto-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: pyuiauto
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python UI Automation library, for cross-platform applications, interfacing through the accessibility API
 Home-page: https://github.com/harveyf2801/pyUIauto
 License: GPL-3.0-only
 Keywords: automation,accessibility,cross-platform,ui,desktop,pywinauto,atomac
 Author: Harvey Fretwell
 Author-email: hgfretwell@gmail.com
 Maintainer: Harvey Fretwell
 Maintainer-email: hgfretwell@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: atomacos (>=3.3.0,<4.0.0); sys_platform == "darwin"
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: atomacos (>=3.3.0,<4.0.0) ; sys_platform == "darwin"
+Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
+Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: pyautogui (==0.9.41)
-Requires-Dist: pywinauto (>=0.6.8,<0.7.0); sys_platform == "win32"
+Requires-Dist: pywinauto (>=0.6.8,<0.7.0) ; sys_platform == "win32"
 Project-URL: Repository, https://github.com/harveyf2801/pyUIauto
 Description-Content-Type: text/markdown
 
 # pyUIauto
 
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
@@ -93,28 +96,39 @@
 main_window.close()
 app.terminateApp()
 ```
 
 ## Authors
 
 ex. Harvey Fretwell
+
 ex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
+
 ex. [atomacos](https://github.com/daveenguyen/atomacos)
+
 ex. [pyAutoGUI](https://github.com/asweigart/pyautogui)
 
 ## Version History
 
 - 0.1
   - Initial Release
   - 0.1.1
     - Added UISystemTrayIcon and UIPopupMenu manager
   - 0.1.4
     - Fixed some issues with setValue() method on buttons and menus
   - 0.1.5
     - Added context managers for better popup menu handling
+  - 0.1.6
+    - Added isOnTop method for components
+    - Fixed isVisible method for components
+    - Added checks for components existing in helper methods
+  - 0.1.7
+    - Added MacOS compatibility
+    - Fixed getValue method for mac on menu items (with a bit of a work around ... hoping to find a better solution soon)
+    - Fixed menu path select and system tray popup select methods on mac
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

