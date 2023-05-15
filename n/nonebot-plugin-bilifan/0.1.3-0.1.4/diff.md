# Comparing `tmp/nonebot_plugin_bilifan-0.1.3.tar.gz` & `tmp/nonebot_plugin_bilifan-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilifan-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_bilifan-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_bilifan-0.1.3.tar` & `nonebot_plugin_bilifan-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-04-18 02:40:25.334390 nonebot_plugin_bilifan-0.1.3/LICENSE
--rw-r--r--   0        0        0     5322 2023-05-04 01:20:09.661670 nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/__init__.py
--rw-r--r--   0        0        0     4993 2023-04-18 02:40:25.338332 nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/login/__init__.py
--rw-r--r--   0        0        0     4458 2023-04-18 02:40:25.339330 nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/main.py
--rw-r--r--   0        0        0       54 2023-04-18 02:40:25.340369 nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/src/__init__.py
--rw-r--r--   0        0        0    17462 2023-04-18 02:40:25.342325 nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/src/api.py
--rw-r--r--   0        0        0    17061 2023-04-18 02:40:25.343367 nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/src/user.py
--rw-r--r--   0        0        0     2230 2023-05-04 00:54:30.204242 nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/users.yaml
--rw-r--r--   0        0        0     2136 2023-05-04 01:20:00.867475 nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/utils.py
--rw-r--r--   0        0        0     1091 2023-05-04 01:20:54.181913 nonebot_plugin_bilifan-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2083 2023-05-04 01:16:44.131895 nonebot_plugin_bilifan-0.1.3/README.md
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2083 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/README.md
+-rw-r--r--   0        0        0     6358 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/__init__.py
+-rw-r--r--   0        0        0     4844 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/login/__init__.py
+-rw-r--r--   0        0        0     4331 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/main.py
+-rw-r--r--   0        0        0       52 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/__init__.py
+-rw-r--r--   0        0        0    16963 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/api.py
+-rw-r--r--   0        0        0    16706 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/user.py
+-rw-r--r--   0        0        0     2197 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/users.yaml
+-rw-r--r--   0        0        0     2068 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/utils.py
+-rw-r--r--   0        0        0     1100 2023-05-15 02:36:08.841744 nonebot_plugin_bilifan-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_bilifan-0.1.3/LICENSE` & `nonebot_plugin_bilifan-0.1.4/LICENSE`

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

### Comparing `nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/login/__init__.py` & `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/login/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-import hashlib
-import urllib.parse as urlparse
-import time
-import os
-import shutil
-import yaml
-import aiohttp , asyncio
-import time
-import hashlib
-import urllib.parse as urlparse
-from io import BytesIO
-from pathlib import Path
-# import qrcode_terminal
-import qrcode
-from nonebot.log import logger
-
-# Cookies = cookiejar.CookieJar()
-# session = requests.Session()
-# session.cookies = Cookies
-
-csrf = ""
-access_key = ""
-base_path = Path().joinpath('data/bilifan')
-
-
-
-
-async def is_login(session, cookies):
-    api = 'https://api.bilibili.com/x/web-interface/nav'
-    headers = {
-        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'
-    }
-    async with session.get(api, headers=headers, cookies=cookies) as resp:
-        data = await resp.json()
-        return data['code'] == 0, data['data']['uname']
-
-
-
-async def get_tv_qrcode_url_and_auth_code():
-    api = 'http://passport.bilibili.com/x/passport-tv-login/qrcode/auth_code'
-    data = {
-        "local_id": "0",
-        "ts": str(int(time.time())),
-    }
-    await signature(data)
-    async with aiohttp.ClientSession() as session:
-        async with session.post(api, data=await map_to_string(data), headers={"Content-Type": "application/x-www-form-urlencoded"}) as resp:
-            resp_data = await resp.json()
-            code = resp_data['code']
-            if code == 0:
-                qrcode_url = resp_data['data']['url']
-                auth_code = resp_data['data']['auth_code']
-                return qrcode_url, auth_code
-            else:
-                raise Exception('get_tv_qrcode_url_and_auth_code error')
-
-
-
-
-async def verify_login(auth_code,data_path):
-    api = "http://passport.bilibili.com/x/passport-tv-login/qrcode/poll"
-    data = {
-        "auth_code": auth_code,
-        "local_id": "0",
-        "ts": str(int(time.time())),
-    }
-    await signature(data)
-    data_string = await map_to_string(data)
-    headers = {
-        "Content-Type": "application/x-www-form-urlencoded",
-    }
-    while True:
-        async with aiohttp.ClientSession() as session:
-            async with session.post(api, headers=headers, data=data_string) as resp:
-                if resp.status != 200:
-                    raise Exception("Failed to connect to server")
-                response_dict = await resp.json()
-                code = response_dict["code"]
-                try:
-                    access_key = response_dict["data"]["access_token"]
-                except:
-                    await asyncio.sleep(3)
-            
-            if code == 0:
-                logger.success("登录成功")
-                with open(data_path/"login_info.txt", "w") as f:
-                    f.write(access_key)
-                if not os.path.exists(data_path/'users.yaml'):
-                    logger.info('初始化配置文件')
-                    shutil.copy2(Path().joinpath('data/bilifan/users.yaml'), data_path/'users.yaml')
-                with open(data_path/'users.yaml', 'r', encoding='utf-8') as f:
-                    config = yaml.safe_load(f)
-                config['USERS'][0]['access_key'] = access_key
-                with open(data_path/'users.yaml', 'w', encoding='utf-8') as f:
-                    yaml.dump(config, f, allow_unicode=True, default_flow_style=False)
-                return "access_key已保存"
-            else:
-                time.sleep(3)
-
-
-appkey = "4409e2ce8ffd12b8"
-appsec = "59b43e04ad6965f34319062b478f83dd"
-
-async def signature(params: dict):
-    keys = list(params.keys())
-    params["appkey"] = appkey
-    keys.append("appkey")
-    keys.sort()
-    query = "&".join([k + "=" + urlparse.quote(params[k]) for k in keys])
-    query += appsec
-    hash = hashlib.md5(query.encode("utf-8"))
-    params["sign"] = hash.hexdigest()
-
-async def map_to_string(params: dict) -> str:
-    query = "&".join([k + "=" + v for k, v in params.items()])
-    return query
-
-async def draw_QR(login_url):
-    "绘制二维码"
-    qr = qrcode.QRCode(version=1, box_size=10, border=4)
-    qr.add_data(login_url)
-    qr.make(fit=True)
-    img = qr.make_image(fill_color="black", back_color="white")
-    buffered = BytesIO()
-    img.save(buffered,format="PNG")
-    img_bytes = buffered.getvalue()
-    return img_bytes
-    # img.save("qrcode.png")
-
-
-# async def loginBili():
-    
-#     login_url, auth_code = await get_tv_qrcode_url_and_auth_code()
-#     qrcode_terminal.draw(login_url)
-#     print("或将此链接复制到手机B站打开:", login_url)
-#     while True:
-#         if await verify_login(auth_code):
-#             print("登录成功！")
-#             break
-#         else:
-#             time.sleep(3)
-#             print("等待扫码登录中...")
-            
-# async def main():
-#     loginBili()
-#     input()
-
-# if __name__ == "__main__":
-#     main()
+import hashlib
+import urllib.parse as urlparse
+import time
+import os
+import shutil
+import yaml
+import aiohttp , asyncio
+import time
+import hashlib
+import urllib.parse as urlparse
+from io import BytesIO
+from pathlib import Path
+# import qrcode_terminal
+import qrcode
+from nonebot.log import logger
+
+# Cookies = cookiejar.CookieJar()
+# session = requests.Session()
+# session.cookies = Cookies
+
+csrf = ""
+access_key = ""
+base_path = Path().joinpath('data/bilifan')
+
+
+
+
+async def is_login(session, cookies):
+    api = 'https://api.bilibili.com/x/web-interface/nav'
+    headers = {
+        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'
+    }
+    async with session.get(api, headers=headers, cookies=cookies) as resp:
+        data = await resp.json()
+        return data['code'] == 0, data['data']['uname']
+
+
+
+async def get_tv_qrcode_url_and_auth_code():
+    api = 'http://passport.bilibili.com/x/passport-tv-login/qrcode/auth_code'
+    data = {
+        "local_id": "0",
+        "ts": str(int(time.time())),
+    }
+    await signature(data)
+    async with aiohttp.ClientSession() as session:
+        async with session.post(api, data=await map_to_string(data), headers={"Content-Type": "application/x-www-form-urlencoded"}) as resp:
+            resp_data = await resp.json()
+            code = resp_data['code']
+            if code == 0:
+                qrcode_url = resp_data['data']['url']
+                auth_code = resp_data['data']['auth_code']
+                return qrcode_url, auth_code
+            else:
+                raise Exception('get_tv_qrcode_url_and_auth_code error')
+
+
+
+
+async def verify_login(auth_code,data_path):
+    api = "http://passport.bilibili.com/x/passport-tv-login/qrcode/poll"
+    data = {
+        "auth_code": auth_code,
+        "local_id": "0",
+        "ts": str(int(time.time())),
+    }
+    await signature(data)
+    data_string = await map_to_string(data)
+    headers = {
+        "Content-Type": "application/x-www-form-urlencoded",
+    }
+    while True:
+        async with aiohttp.ClientSession() as session:
+            async with session.post(api, headers=headers, data=data_string) as resp:
+                if resp.status != 200:
+                    raise Exception("Failed to connect to server")
+                response_dict = await resp.json()
+                code = response_dict["code"]
+                try:
+                    access_key = response_dict["data"]["access_token"]
+                except:
+                    await asyncio.sleep(3)
+            
+            if code == 0:
+                logger.success("登录成功")
+                with open(data_path/"login_info.txt", "w") as f:
+                    f.write(access_key)
+                if not os.path.exists(data_path/'users.yaml'):
+                    logger.info('初始化配置文件')
+                    shutil.copy2(Path().joinpath('data/bilifan/users.yaml'), data_path/'users.yaml')
+                with open(data_path/'users.yaml', 'r', encoding='utf-8') as f:
+                    config = yaml.safe_load(f)
+                config['USERS'][0]['access_key'] = access_key
+                with open(data_path/'users.yaml', 'w', encoding='utf-8') as f:
+                    yaml.dump(config, f, allow_unicode=True, default_flow_style=False)
+                return "access_key已保存"
+            else:
+                time.sleep(3)
+
+
+appkey = "4409e2ce8ffd12b8"
+appsec = "59b43e04ad6965f34319062b478f83dd"
+
+async def signature(params: dict):
+    keys = list(params.keys())
+    params["appkey"] = appkey
+    keys.append("appkey")
+    keys.sort()
+    query = "&".join([k + "=" + urlparse.quote(params[k]) for k in keys])
+    query += appsec
+    hash = hashlib.md5(query.encode("utf-8"))
+    params["sign"] = hash.hexdigest()
+
+async def map_to_string(params: dict) -> str:
+    query = "&".join([k + "=" + v for k, v in params.items()])
+    return query
+
+async def draw_QR(login_url):
+    "绘制二维码"
+    qr = qrcode.QRCode(version=1, box_size=10, border=4)
+    qr.add_data(login_url)
+    qr.make(fit=True)
+    img = qr.make_image(fill_color="black", back_color="white")
+    buffered = BytesIO()
+    img.save(buffered,format="PNG")
+    img_bytes = buffered.getvalue()
+    return img_bytes
+    # img.save("qrcode.png")
+
+
+# async def loginBili():
+    
+#     login_url, auth_code = await get_tv_qrcode_url_and_auth_code()
+#     qrcode_terminal.draw(login_url)
+#     print("或将此链接复制到手机B站打开:", login_url)
+#     while True:
+#         if await verify_login(auth_code):
+#             print("登录成功！")
+#             break
+#         else:
+#             time.sleep(3)
+#             print("等待扫码登录中...")
+            
+# async def main():
+#     loginBili()
+#     input()
+
+# if __name__ == "__main__":
+#     main()
```

### Comparing `nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/main.py` & `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/main.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import json
-import os
-from nonebot.log import logger as log
-import warnings
-import asyncio
-import aiohttp
-import itertools
-from pathlib import Path
-from .src import BiliUser
-from nonebot.log import logger
-local_path = Path(__file__).parent
-
-__VERSION__ = "0.3.6"
-
-warnings.filterwarnings(
-    "ignore",
-    message="The localize method is no longer necessary, as this time zone supports the fold attribute",
-)
-# os.chdir(os.path.dirname(os.path.abspath(__file__)).split(__file__)[0])
-
-base_path = Path().joinpath('data/bilifan')
-base_path.mkdir(parents=True, exist_ok=True)
-logger.info(base_path)
-
-global users
-async def read_yaml(msg_path:Path):
-    global config,users
-    try:
-        if os.environ.get("USERS"):
-            users = json.loads(os.environ.get("USERS"))
-        else:
-            import yaml   
-            with open(msg_path/'users.yaml', 'r', encoding='utf-8') as f:
-                users = yaml.load(f, Loader=yaml.FullLoader)
-        assert users['ASYNC'] in [0, 1], "ASYNC参数错误"
-        assert users['LIKE_CD'] >= 0, "LIKE_CD参数错误"
-        # assert users['SHARE_CD'] >= 0, "SHARE_CD参数错误"
-        assert users['DANMAKU_CD'] >= 0, "DANMAKU_CD参数错误"
-        assert users['WATCHINGLIVE'] >= 0, "WATCHINGLIVE参数错误"
-        assert users['WEARMEDAL'] in [0, 1], "WEARMEDAL参数错误"
-        config = {
-            "ASYNC": users['ASYNC'],
-            "LIKE_CD": users['LIKE_CD'],
-            # "SHARE_CD": users['SHARE_CD'],
-            "DANMAKU_CD": users['DANMAKU_CD'],
-            "WATCHINGLIVE": users['WATCHINGLIVE'],
-            "WEARMEDAL": users['WEARMEDAL'],
-            "SIGNINGROUP": users.get('SIGNINGROUP', 2),
-        }
-    except Exception as e:
-        log.error(f"读取配置文件失败,请检查配置文件格式是否正确: {e}")
-        exit(1)
-    return users
-
-@log.catch
-async def main(msg_path):
-    await read_yaml(msg_path)
-    init_tasks = []
-    start_tasks = []
-    catch_msg = []
-
-    for user in users['USERS']:
-        if user['access_key']:
-            bili_user = BiliUser(user['access_key'], user.get('white_uid', ''), user.get('banned_uid', ''), config)
-            init_tasks.append(bili_user.init())
-            start_tasks.append(bili_user.start())
-            catch_msg.append(bili_user.sendmsg())
-
-    try:
-        await asyncio.gather(*init_tasks)
-        await asyncio.gather(*start_tasks)
-    except Exception as e:
-        log.exception(e)
-        message_list = [f"任务执行失败: {e}"]
-    else:
-        message_list = []
-
-    try:
-        catch_msg_results = await asyncio.gather(*catch_msg)
-    except Exception as e:
-        log.exception(e)
-        message_list.append(f"发送消息失败: {e}")
-    else:
-        message_list += list(itertools.chain.from_iterable(catch_msg_results))
-
-    [log.info(message) for message in message_list]
-    return message_list
-
-
-
-def run(*args, **kwargs):
-    loop = asyncio.new_event_loop()
-    loop.run_until_complete(main())
-    log.info("任务结束，等待下一次执行。")
-
-
-        
-# if __name__ == '__main__':
-    # cron = users.get('CRON', None)
-
-    # if cron:
-    #     from apscheduler.schedulers.blocking import BlockingScheduler
-    #     from apscheduler.triggers.cron import CronTrigger
-
-    #     log.info(f'使用内置定时器 {cron}，开启定时任务，等待时间到达后执行。')
-    #     schedulers = BlockingScheduler()
-    #     schedulers.add_job(run, CronTrigger.from_crontab(cron), misfire_grace_time=3600)
-    #     schedulers.start()
-    # elif "--auto" in sys.argv:
-    #     from apscheduler.schedulers.blocking import BlockingScheduler
-    #     from apscheduler.triggers.interval import IntervalTrigger
-    #     import datetime
-
-    #     log.info('使用自动守护模式，每隔 24 小时运行一次。')
-    #     scheduler = BlockingScheduler(timezone='Asia/Shanghai')
-    #     scheduler.add_job(
-    #         run,
-    #         IntervalTrigger(hours=24),
-    #         next_run_time=datetime.datetime.now(),
-    #         misfire_grace_time=3600,
-    #     )
-    #     scheduler.start()
-    # else:
-    #     log.info('未配置定时器，开启单次任务。')
-    #     loop = asyncio.new_event_loop()
-    #     asyncio.set_event_loop(loop)
-    #     loop.run_until_complete(main())
+import json
+import os
+from nonebot.log import logger as log
+import warnings
+import asyncio
+import aiohttp
+import itertools
+from pathlib import Path
+from .src import BiliUser
+from nonebot.log import logger
+local_path = Path(__file__).parent
+
+__VERSION__ = "0.3.6"
+
+warnings.filterwarnings(
+    "ignore",
+    message="The localize method is no longer necessary, as this time zone supports the fold attribute",
+)
+# os.chdir(os.path.dirname(os.path.abspath(__file__)).split(__file__)[0])
+
+base_path = Path().joinpath('data/bilifan')
+base_path.mkdir(parents=True, exist_ok=True)
+logger.info(base_path)
+
+global users
+async def read_yaml(msg_path:Path):
+    global config,users
+    try:
+        if os.environ.get("USERS"):
+            users = json.loads(os.environ.get("USERS"))
+        else:
+            import yaml   
+            with open(msg_path/'users.yaml', 'r', encoding='utf-8') as f:
+                users = yaml.load(f, Loader=yaml.FullLoader)
+        assert users['ASYNC'] in [0, 1], "ASYNC参数错误"
+        assert users['LIKE_CD'] >= 0, "LIKE_CD参数错误"
+        # assert users['SHARE_CD'] >= 0, "SHARE_CD参数错误"
+        assert users['DANMAKU_CD'] >= 0, "DANMAKU_CD参数错误"
+        assert users['WATCHINGLIVE'] >= 0, "WATCHINGLIVE参数错误"
+        assert users['WEARMEDAL'] in [0, 1], "WEARMEDAL参数错误"
+        config = {
+            "ASYNC": users['ASYNC'],
+            "LIKE_CD": users['LIKE_CD'],
+            # "SHARE_CD": users['SHARE_CD'],
+            "DANMAKU_CD": users['DANMAKU_CD'],
+            "WATCHINGLIVE": users['WATCHINGLIVE'],
+            "WEARMEDAL": users['WEARMEDAL'],
+            "SIGNINGROUP": users.get('SIGNINGROUP', 2),
+        }
+    except Exception as e:
+        log.error(f"读取配置文件失败,请检查配置文件格式是否正确: {e}")
+        exit(1)
+    return users
+
+@log.catch
+async def main(msg_path):
+    await read_yaml(msg_path)
+    init_tasks = []
+    start_tasks = []
+    catch_msg = []
+
+    for user in users['USERS']:
+        if user['access_key']:
+            bili_user = BiliUser(user['access_key'], user.get('white_uid', ''), user.get('banned_uid', ''), config)
+            init_tasks.append(bili_user.init())
+            start_tasks.append(bili_user.start())
+            catch_msg.append(bili_user.sendmsg())
+
+    try:
+        await asyncio.gather(*init_tasks)
+        await asyncio.gather(*start_tasks)
+    except Exception as e:
+        log.exception(e)
+        message_list = [f"任务执行失败: {e}"]
+    else:
+        message_list = []
+
+    try:
+        catch_msg_results = await asyncio.gather(*catch_msg)
+    except Exception as e:
+        log.exception(e)
+        message_list.append(f"发送消息失败: {e}")
+    else:
+        message_list += list(itertools.chain.from_iterable(catch_msg_results))
+
+    [log.info(message) for message in message_list]
+    return message_list
+
+
+
+def run(*args, **kwargs):
+    loop = asyncio.new_event_loop()
+    loop.run_until_complete(main())
+    log.info("任务结束，等待下一次执行。")
+
+
+        
+# if __name__ == '__main__':
+    # cron = users.get('CRON', None)
+
+    # if cron:
+    #     from apscheduler.schedulers.blocking import BlockingScheduler
+    #     from apscheduler.triggers.cron import CronTrigger
+
+    #     log.info(f'使用内置定时器 {cron}，开启定时任务，等待时间到达后执行。')
+    #     schedulers = BlockingScheduler()
+    #     schedulers.add_job(run, CronTrigger.from_crontab(cron), misfire_grace_time=3600)
+    #     schedulers.start()
+    # elif "--auto" in sys.argv:
+    #     from apscheduler.schedulers.blocking import BlockingScheduler
+    #     from apscheduler.triggers.interval import IntervalTrigger
+    #     import datetime
+
+    #     log.info('使用自动守护模式，每隔 24 小时运行一次。')
+    #     scheduler = BlockingScheduler(timezone='Asia/Shanghai')
+    #     scheduler.add_job(
+    #         run,
+    #         IntervalTrigger(hours=24),
+    #         next_run_time=datetime.datetime.now(),
+    #         misfire_grace_time=3600,
+    #     )
+    #     scheduler.start()
+    # else:
+    #     log.info('未配置定时器，开启单次任务。')
+    #     loop = asyncio.new_event_loop()
+    #     asyncio.set_event_loop(loop)
+    #     loop.run_until_complete(main())
     #     log.info("任务结束")
```

### Comparing `nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/src/api.py` & `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/api.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,499 +1,499 @@
-import asyncio
-from hashlib import md5
-import hashlib
-import random
-import time
-import json
-from typing import Union
-from nonebot.log import logger
-from urllib.parse import urlencode, urlparse
-
-
-from aiohttp import ClientSession
-
-# sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-
-
-class Crypto:
-
-    APPKEY = '4409e2ce8ffd12b8'
-    APPSECRET = '59b43e04ad6965f34319062b478f83dd'
-
-    @staticmethod
-    def md5(data: Union[str, bytes]) -> str:
-        '''generates md5 hex dump of `str` or `bytes`'''
-        if type(data) == str:
-            return md5(data.encode()).hexdigest()
-        return md5(data).hexdigest()
-
-    @staticmethod
-    def sign(data: Union[str, dict]) -> str:
-        '''salted sign funtion for `dict`(converts to qs then parse) & `str`'''
-        if isinstance(data, dict):
-            _str = urlencode(data)
-        elif type(data) != str:
-            raise TypeError
-        return Crypto.md5(_str + Crypto.APPSECRET)
-
-
-class SingableDict(dict):
-    @property
-    def sorted(self):
-        '''returns a alphabetically sorted version of `self`'''
-        return dict(sorted(self.items()))
-
-    @property
-    def signed(self):
-        '''returns our sorted self with calculated `sign` as a new key-value pair at the end'''
-        _sorted = self.sorted
-        return {**_sorted, 'sign': Crypto.sign(_sorted)}
-
-
-def retry(tries=3, interval=1):
-    def decorate(func):
-        async def wrapper(*args, **kwargs):
-            count = 0
-            func.isRetryable = False
-            log = logger.bind(user=f"{args[0].u.name}")
-            while True:
-                try:
-                    result = await func(*args, **kwargs)
-                except Exception as e:
-                    count += 1
-                    if type(e) == BiliApiError:
-                        if e.code == 1011040:
-                            raise e
-                        elif e.code == 10030:
-                            await asyncio.sleep(10)
-                        elif e.code == -504:
-                            pass
-                        else:
-                            raise e
-                    if count > tries:
-                        log.error(f"API {urlparse(args[1]).path} 调用出现异常: {str(e)}")
-                        raise e
-                    else:
-                        # log.error(f"API {urlparse(args[1]).path} 调用出现异常: {str(e)}，重试中，第{count}次重试")
-                        await asyncio.sleep(interval)
-                    func.isRetryable = True
-                else:
-                    if func.isRetryable:
-                        pass
-                        # log.success(f"重试成功")
-                    return result
-
-        return wrapper
-
-    return decorate
-
-
-def client_sign(data: dict):
-    _str = json.dumps(data, separators=(',', ':'))
-    for n in ["sha512", "sha3_512", "sha384", "sha3_384", "blake2b"]:
-        _str = hashlib.new(n, _str.encode('utf-8')).hexdigest()
-    return _str
-
-
-def randomString(length: int = 16) -> str:
-    return ''.join(random.sample('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789', length))
-
-
-class BiliApiError(Exception):
-    def __init__(self, code: int, msg: str):
-        self.code = code
-        self.msg = msg
-
-    def __str__(self):
-        return self.msg
-
-
-class BiliApi:
-    headers = {
-        "User-Agent": "Mozilla/5.0 BiliDroid/6.73.1 (bbcallen@gmail.com) os/android model/Mi 10 Pro mobi_app/android build/6731100 channel/xiaomi innerVer/6731110 osVer/12 network/2",
-    }
-    from .user import BiliUser
-
-    def __init__(self, u: BiliUser, s: ClientSession):
-        self.u = u
-        self.session = s
-
-    def __check_response(self, resp: dict) -> dict:
-        if resp['code'] != 0 or ('mode_info' in resp['data'] and resp['message'] != ''):
-            raise BiliApiError(resp['code'], resp['message'])
-        return resp['data']
-
-    @retry()
-    async def __get(self, *args, **kwargs):
-        async with self.session.get(*args, **kwargs) as resp:
-            return self.__check_response(await resp.json())
-
-    @retry()
-    async def __post(self, *args, **kwargs):
-        async with self.session.post(*args, **kwargs) as resp:
-            return self.__check_response(await resp.json())
-
-    async def getFansMedalandRoomID(self) -> dict:
-        """
-        获取用户粉丝勋章和直播间ID
-        """
-        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/fansMedal/panel"
-        params = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-            "page": 1,
-            "page_size": 50,
-        }
-        first_flag = True
-        while True:
-            data = await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
-            if first_flag and data['special_list']:
-                for item in data['special_list']:
-                    # 强制把正在佩戴的牌子加入任务列表
-                    item['medal']['today_feed'] = 0
-                    yield item
-                self.u.wearedMedal = data['special_list'][0]
-                first_flag = False
-            for item in data['list']:
-                yield item
-            if not data['list']:
-                break
-            params['page'] += 1
-
-    async def likeInteract(self, room_id: int):
-        """
-        点赞直播间
-        """
-        url = "https://api.live.bilibili.com/xlive/web-ucenter/v1/interact/likeInteract"
-        data = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-            "roomid": room_id,
-        }
-        # for _ in range(3):
-        await self.__post(
-            url,
-            data=SingableDict(data).signed,
-            headers=self.headers.update(
-                {
-                    "Content-Type": "application/x-www-form-urlencoded",
-                }
-            ),
-        )
-        # await asyncio.sleep(self.u.config['LIKE_CD'] if not self.u.config['ASYNC'] else 2)
-
-    async def likeInteractV3(self, room_id: int, up_id: int):
-        """
-        点赞直播间V3
-        """
-        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/like_info_v3/like/likeReportV3"
-        data = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-            "room_id": room_id,
-            "anchor_id": up_id,
-        }
-        # for _ in range(3):
-        await self.__post(
-            url,
-            data=SingableDict(data).signed,
-            headers=self.headers.update(
-                {
-                    "Content-Type": "application/x-www-form-urlencoded",
-                }
-            ),
-        )
-
-    async def shareRoom(self, room_id: int):
-        """
-        分享直播间
-        """
-        url = "https://api.live.bilibili.com/xlive/app-room/v1/index/TrigerInteract"
-        data = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-            "interact_type": 3,
-            "roomid": room_id,
-        }
-        # for _ in range(5):
-        await self.__post(
-            url,
-            data=SingableDict(data).signed,
-            headers=self.headers.update(
-                {
-                    "Content-Type": "application/x-www-form-urlencoded",
-                }
-            ),
-        )
-        # await asyncio.sleep(self.u.config['SHARE_CD'] if not self.u.config['ASYNC'] else 5)
-
-    async def sendDanmaku(self, room_id: int) -> str:
-        """
-        发送弹幕
-        """
-        url = "https://api.live.bilibili.com/xlive/app-room/v1/dM/sendmsg"
-        danmakus = [
-            "(⌒▽⌒).",
-            "（￣▽￣）.",
-            "(=・ω・=).",
-            "(｀・ω・´).",
-            "(〜￣△￣)〜.",
-            "(･∀･).",
-            "(°∀°)ﾉ.",
-            "(￣3￣).",
-            "╮(￣▽￣)╭.",
-            "_(:3」∠)_.",
-            "(^・ω・^ ).",
-            "(●￣(ｴ)￣●).",
-            "ε=ε=(ノ≧∇≦)ノ.",
-            "⁄(⁄ ⁄•⁄ω⁄•⁄ ⁄)⁄.",
-            "←◡←.",
-        ]
-        params = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-        }
-        data = {
-            "cid": room_id,
-            "msg": random.choice(danmakus),
-            "rnd": int(time.time()),
-            "color": "16777215",
-            "fontsize": "25",
-        }
-        try:
-            resp = await self.__post(
-                url,
-                params=SingableDict(params).signed,
-                data=data,
-                headers=self.headers.update(
-                    {
-                        "Content-Type": "application/x-www-form-urlencoded",
-                    }
-                ),
-            )
-        except BiliApiError as e:
-            if e.code == 0:
-                await asyncio.sleep(self.u.config['DANMAKU_CD'])
-                params.update(
-                    {
-                        "ts": int(time.time()),
-                    }
-                )
-                data.update(
-                    {
-                        "msg": "111",
-                    }
-                )
-                resp = await self.__post(
-                    url,
-                    params=SingableDict(params).signed,
-                    data=data,
-                    headers=self.headers.update(
-                        {
-                            "Content-Type": "application/x-www-form-urlencoded",
-                        }
-                    ),
-                )
-                return json.loads(resp['mode_info']['extra'])['content']
-            raise e
-        return json.loads(resp['mode_info']['extra'])['content']
-
-    async def loginVerift(self):
-        """
-        登录验证
-        """
-        url = "https://app.bilibili.com/x/v2/account/mine"
-        params = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-        }
-        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
-
-    async def doSign(self):
-        """
-        直播区签到
-        """
-        url = "https://api.live.bilibili.com/rc/v1/Sign/doSign"
-        params = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-        }
-        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
-
-    async def getUserInfo(self):
-        """
-        用户直播等级
-        """
-        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/user/get_user_info"
-        params = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-        }
-        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
-
-    async def getMedalsInfoByUid(self, uid: int):
-        """
-        用户勋章信息
-        """
-        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/fansMedal/fans_medal_info"
-        params = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-            "target_id": uid,
-        }
-        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
-
-    # async def entryRoom(self, room_id: int, up_id: int):
-    #     data = {
-    #         "access_key": self.u.access_key,
-    #         "actionKey": "appkey",
-    #         "appkey": Crypto.APPKEY,
-    #         "ts": int(time.time()),
-    #         'platform': 'android',
-    #         'uuid': self.u.uuids[0],
-    #         'buvid': randomString(37).upper(),
-    #         'seq_id': '1',
-    #         'room_id': f'{room_id}',
-    #         'parent_id': '6',
-    #         'area_id': '283',
-    #         'timestamp': f'{int(time.time())-60}',
-    #         'secret_key': 'axoaadsffcazxksectbbb',
-    #         'watch_time': '60',
-    #         'up_id': f'{up_id}',
-    #         'up_level': '40',
-    #         'jump_from': '30000',
-    #         'gu_id': randomString(43).lower(),
-    #         'visit_id': randomString(32).lower(),
-    #         'click_id': self.u.uuids[1],
-    #         'heart_beat': '[]',
-    #         'client_ts': f'{int(time.time())}'
-    #     }
-    #     url = "http://live-trace.bilibili.com/xlive/data-interface/v1/heartbeat/mobileEntry"
-    #     return await self.__post(url, data=SingableDict(data).signed, headers=self.headers.update({
-    #         "Content-Type": "application/x-www-form-urlencoded",
-    #     }))
-
-    async def heartbeat(self, room_id: int, up_id: int):
-        url = "https://live-trace.bilibili.com/xlive/data-interface/v1/heartbeat/mobileHeartBeat"
-        data = {
-            'platform': 'android',
-            'uuid': self.u.uuids[0],
-            'buvid': randomString(37).upper(),
-            'seq_id': '1',
-            'room_id': f'{room_id}',
-            'parent_id': '6',
-            'area_id': '283',
-            'timestamp': f'{int(time.time())-60}',
-            'secret_key': 'axoaadsffcazxksectbbb',
-            'watch_time': '60',
-            'up_id': f'{up_id}',
-            'up_level': '40',
-            'jump_from': '30000',
-            'gu_id': randomString(43).lower(),
-            'play_type': '0',
-            'play_url': '',
-            's_time': '0',
-            'data_behavior_id': '',
-            'data_source_id': '',
-            'up_session': f'l:one:live:record:{room_id}:{int(time.time())-88888}',
-            'visit_id': randomString(32).lower(),
-            'watch_status': '%7B%22pk_id%22%3A0%2C%22screen_status%22%3A1%7D',
-            'click_id': self.u.uuids[1],
-            'session_id': '',
-            'player_type': '0',
-            'client_ts': f'{int(time.time())}',
-        }
-        data.update(
-            {
-                'client_sign': client_sign(data),
-                "access_key": self.u.access_key,
-                "actionKey": "appkey",
-                "appkey": Crypto.APPKEY,
-                "ts": int(time.time()),
-            }
-        )
-        return await self.__post(
-            url,
-            data=SingableDict(data).signed,
-            headers=self.headers.update(
-                {
-                    "Content-Type": "application/x-www-form-urlencoded",
-                }
-            ),
-        )
-
-    async def wearMedal(self, medal_id: int):
-        """
-        佩戴粉丝牌
-        """
-        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/fansMedal/wear"
-        data = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-            "medal_id": medal_id,
-            "platform": "android",
-            "type": "1",
-            "version": "0",
-        }
-        return await self.__post(
-            url,
-            data=SingableDict(data).signed,
-            headers=self.headers.update(
-                {
-                    "Content-Type": "application/x-www-form-urlencoded",
-                }
-            ),
-        )
-
-    async def getGroups(self):
-        url = "https://api.live.bilibili.com/link_group/v1/member/my_groups"
-        params = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-        }
-        list = (await self.__get(url, params=SingableDict(params).signed, headers=self.headers))['list']
-        for group in list:
-            yield group
-
-    async def signInGroups(self, group_id: int, owner_id: int):
-        url = "https://api.vc.bilibili.com/link_setting/v1/link_setting/sign_in"
-        params = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-            "group_id": group_id,
-            "owner_id": owner_id,
-        }
-        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
-
-    async def getOneBattery(self):
-        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/userTask/UserTaskReceiveRewards"
-        data = {
-            "access_key": self.u.access_key,
-            "actionKey": "appkey",
-            "appkey": Crypto.APPKEY,
-            "ts": int(time.time()),
-        }
-        return await self.__post(url, data=SingableDict(data).signed, headers=self.headers)
+import asyncio
+from hashlib import md5
+import hashlib
+import random
+import time
+import json
+from typing import Union
+from nonebot.log import logger
+from urllib.parse import urlencode, urlparse
+
+
+from aiohttp import ClientSession
+
+# sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+
+
+class Crypto:
+
+    APPKEY = '4409e2ce8ffd12b8'
+    APPSECRET = '59b43e04ad6965f34319062b478f83dd'
+
+    @staticmethod
+    def md5(data: Union[str, bytes]) -> str:
+        '''generates md5 hex dump of `str` or `bytes`'''
+        if type(data) == str:
+            return md5(data.encode()).hexdigest()
+        return md5(data).hexdigest()
+
+    @staticmethod
+    def sign(data: Union[str, dict]) -> str:
+        '''salted sign funtion for `dict`(converts to qs then parse) & `str`'''
+        if isinstance(data, dict):
+            _str = urlencode(data)
+        elif type(data) != str:
+            raise TypeError
+        return Crypto.md5(_str + Crypto.APPSECRET)
+
+
+class SingableDict(dict):
+    @property
+    def sorted(self):
+        '''returns a alphabetically sorted version of `self`'''
+        return dict(sorted(self.items()))
+
+    @property
+    def signed(self):
+        '''returns our sorted self with calculated `sign` as a new key-value pair at the end'''
+        _sorted = self.sorted
+        return {**_sorted, 'sign': Crypto.sign(_sorted)}
+
+
+def retry(tries=3, interval=1):
+    def decorate(func):
+        async def wrapper(*args, **kwargs):
+            count = 0
+            func.isRetryable = False
+            log = logger.bind(user=f"{args[0].u.name}")
+            while True:
+                try:
+                    result = await func(*args, **kwargs)
+                except Exception as e:
+                    count += 1
+                    if type(e) == BiliApiError:
+                        if e.code == 1011040:
+                            raise e
+                        elif e.code == 10030:
+                            await asyncio.sleep(10)
+                        elif e.code == -504:
+                            pass
+                        else:
+                            raise e
+                    if count > tries:
+                        log.error(f"API {urlparse(args[1]).path} 调用出现异常: {str(e)}")
+                        raise e
+                    else:
+                        # log.error(f"API {urlparse(args[1]).path} 调用出现异常: {str(e)}，重试中，第{count}次重试")
+                        await asyncio.sleep(interval)
+                    func.isRetryable = True
+                else:
+                    if func.isRetryable:
+                        pass
+                        # log.success(f"重试成功")
+                    return result
+
+        return wrapper
+
+    return decorate
+
+
+def client_sign(data: dict):
+    _str = json.dumps(data, separators=(',', ':'))
+    for n in ["sha512", "sha3_512", "sha384", "sha3_384", "blake2b"]:
+        _str = hashlib.new(n, _str.encode('utf-8')).hexdigest()
+    return _str
+
+
+def randomString(length: int = 16) -> str:
+    return ''.join(random.sample('abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789', length))
+
+
+class BiliApiError(Exception):
+    def __init__(self, code: int, msg: str):
+        self.code = code
+        self.msg = msg
+
+    def __str__(self):
+        return self.msg
+
+
+class BiliApi:
+    headers = {
+        "User-Agent": "Mozilla/5.0 BiliDroid/6.73.1 (bbcallen@gmail.com) os/android model/Mi 10 Pro mobi_app/android build/6731100 channel/xiaomi innerVer/6731110 osVer/12 network/2",
+    }
+    from .user import BiliUser
+
+    def __init__(self, u: BiliUser, s: ClientSession):
+        self.u = u
+        self.session = s
+
+    def __check_response(self, resp: dict) -> dict:
+        if resp['code'] != 0 or ('mode_info' in resp['data'] and resp['message'] != ''):
+            raise BiliApiError(resp['code'], resp['message'])
+        return resp['data']
+
+    @retry()
+    async def __get(self, *args, **kwargs):
+        async with self.session.get(*args, **kwargs) as resp:
+            return self.__check_response(await resp.json())
+
+    @retry()
+    async def __post(self, *args, **kwargs):
+        async with self.session.post(*args, **kwargs) as resp:
+            return self.__check_response(await resp.json())
+
+    async def getFansMedalandRoomID(self) -> dict:
+        """
+        获取用户粉丝勋章和直播间ID
+        """
+        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/fansMedal/panel"
+        params = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+            "page": 1,
+            "page_size": 50,
+        }
+        first_flag = True
+        while True:
+            data = await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
+            if first_flag and data['special_list']:
+                for item in data['special_list']:
+                    # 强制把正在佩戴的牌子加入任务列表
+                    item['medal']['today_feed'] = 0
+                    yield item
+                self.u.wearedMedal = data['special_list'][0]
+                first_flag = False
+            for item in data['list']:
+                yield item
+            if not data['list']:
+                break
+            params['page'] += 1
+
+    async def likeInteract(self, room_id: int):
+        """
+        点赞直播间
+        """
+        url = "https://api.live.bilibili.com/xlive/web-ucenter/v1/interact/likeInteract"
+        data = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+            "roomid": room_id,
+        }
+        # for _ in range(3):
+        await self.__post(
+            url,
+            data=SingableDict(data).signed,
+            headers=self.headers.update(
+                {
+                    "Content-Type": "application/x-www-form-urlencoded",
+                }
+            ),
+        )
+        # await asyncio.sleep(self.u.config['LIKE_CD'] if not self.u.config['ASYNC'] else 2)
+
+    async def likeInteractV3(self, room_id: int, up_id: int):
+        """
+        点赞直播间V3
+        """
+        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/like_info_v3/like/likeReportV3"
+        data = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+            "room_id": room_id,
+            "anchor_id": up_id,
+        }
+        # for _ in range(3):
+        await self.__post(
+            url,
+            data=SingableDict(data).signed,
+            headers=self.headers.update(
+                {
+                    "Content-Type": "application/x-www-form-urlencoded",
+                }
+            ),
+        )
+
+    async def shareRoom(self, room_id: int):
+        """
+        分享直播间
+        """
+        url = "https://api.live.bilibili.com/xlive/app-room/v1/index/TrigerInteract"
+        data = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+            "interact_type": 3,
+            "roomid": room_id,
+        }
+        # for _ in range(5):
+        await self.__post(
+            url,
+            data=SingableDict(data).signed,
+            headers=self.headers.update(
+                {
+                    "Content-Type": "application/x-www-form-urlencoded",
+                }
+            ),
+        )
+        # await asyncio.sleep(self.u.config['SHARE_CD'] if not self.u.config['ASYNC'] else 5)
+
+    async def sendDanmaku(self, room_id: int) -> str:
+        """
+        发送弹幕
+        """
+        url = "https://api.live.bilibili.com/xlive/app-room/v1/dM/sendmsg"
+        danmakus = [
+            "(⌒▽⌒).",
+            "（￣▽￣）.",
+            "(=・ω・=).",
+            "(｀・ω・´).",
+            "(〜￣△￣)〜.",
+            "(･∀･).",
+            "(°∀°)ﾉ.",
+            "(￣3￣).",
+            "╮(￣▽￣)╭.",
+            "_(:3」∠)_.",
+            "(^・ω・^ ).",
+            "(●￣(ｴ)￣●).",
+            "ε=ε=(ノ≧∇≦)ノ.",
+            "⁄(⁄ ⁄•⁄ω⁄•⁄ ⁄)⁄.",
+            "←◡←.",
+        ]
+        params = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+        }
+        data = {
+            "cid": room_id,
+            "msg": random.choice(danmakus),
+            "rnd": int(time.time()),
+            "color": "16777215",
+            "fontsize": "25",
+        }
+        try:
+            resp = await self.__post(
+                url,
+                params=SingableDict(params).signed,
+                data=data,
+                headers=self.headers.update(
+                    {
+                        "Content-Type": "application/x-www-form-urlencoded",
+                    }
+                ),
+            )
+        except BiliApiError as e:
+            if e.code == 0:
+                await asyncio.sleep(self.u.config['DANMAKU_CD'])
+                params.update(
+                    {
+                        "ts": int(time.time()),
+                    }
+                )
+                data.update(
+                    {
+                        "msg": "111",
+                    }
+                )
+                resp = await self.__post(
+                    url,
+                    params=SingableDict(params).signed,
+                    data=data,
+                    headers=self.headers.update(
+                        {
+                            "Content-Type": "application/x-www-form-urlencoded",
+                        }
+                    ),
+                )
+                return json.loads(resp['mode_info']['extra'])['content']
+            raise e
+        return json.loads(resp['mode_info']['extra'])['content']
+
+    async def loginVerift(self):
+        """
+        登录验证
+        """
+        url = "https://app.bilibili.com/x/v2/account/mine"
+        params = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+        }
+        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
+
+    async def doSign(self):
+        """
+        直播区签到
+        """
+        url = "https://api.live.bilibili.com/rc/v1/Sign/doSign"
+        params = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+        }
+        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
+
+    async def getUserInfo(self):
+        """
+        用户直播等级
+        """
+        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/user/get_user_info"
+        params = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+        }
+        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
+
+    async def getMedalsInfoByUid(self, uid: int):
+        """
+        用户勋章信息
+        """
+        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/fansMedal/fans_medal_info"
+        params = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+            "target_id": uid,
+        }
+        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
+
+    # async def entryRoom(self, room_id: int, up_id: int):
+    #     data = {
+    #         "access_key": self.u.access_key,
+    #         "actionKey": "appkey",
+    #         "appkey": Crypto.APPKEY,
+    #         "ts": int(time.time()),
+    #         'platform': 'android',
+    #         'uuid': self.u.uuids[0],
+    #         'buvid': randomString(37).upper(),
+    #         'seq_id': '1',
+    #         'room_id': f'{room_id}',
+    #         'parent_id': '6',
+    #         'area_id': '283',
+    #         'timestamp': f'{int(time.time())-60}',
+    #         'secret_key': 'axoaadsffcazxksectbbb',
+    #         'watch_time': '60',
+    #         'up_id': f'{up_id}',
+    #         'up_level': '40',
+    #         'jump_from': '30000',
+    #         'gu_id': randomString(43).lower(),
+    #         'visit_id': randomString(32).lower(),
+    #         'click_id': self.u.uuids[1],
+    #         'heart_beat': '[]',
+    #         'client_ts': f'{int(time.time())}'
+    #     }
+    #     url = "http://live-trace.bilibili.com/xlive/data-interface/v1/heartbeat/mobileEntry"
+    #     return await self.__post(url, data=SingableDict(data).signed, headers=self.headers.update({
+    #         "Content-Type": "application/x-www-form-urlencoded",
+    #     }))
+
+    async def heartbeat(self, room_id: int, up_id: int):
+        url = "https://live-trace.bilibili.com/xlive/data-interface/v1/heartbeat/mobileHeartBeat"
+        data = {
+            'platform': 'android',
+            'uuid': self.u.uuids[0],
+            'buvid': randomString(37).upper(),
+            'seq_id': '1',
+            'room_id': f'{room_id}',
+            'parent_id': '6',
+            'area_id': '283',
+            'timestamp': f'{int(time.time())-60}',
+            'secret_key': 'axoaadsffcazxksectbbb',
+            'watch_time': '60',
+            'up_id': f'{up_id}',
+            'up_level': '40',
+            'jump_from': '30000',
+            'gu_id': randomString(43).lower(),
+            'play_type': '0',
+            'play_url': '',
+            's_time': '0',
+            'data_behavior_id': '',
+            'data_source_id': '',
+            'up_session': f'l:one:live:record:{room_id}:{int(time.time())-88888}',
+            'visit_id': randomString(32).lower(),
+            'watch_status': '%7B%22pk_id%22%3A0%2C%22screen_status%22%3A1%7D',
+            'click_id': self.u.uuids[1],
+            'session_id': '',
+            'player_type': '0',
+            'client_ts': f'{int(time.time())}',
+        }
+        data.update(
+            {
+                'client_sign': client_sign(data),
+                "access_key": self.u.access_key,
+                "actionKey": "appkey",
+                "appkey": Crypto.APPKEY,
+                "ts": int(time.time()),
+            }
+        )
+        return await self.__post(
+            url,
+            data=SingableDict(data).signed,
+            headers=self.headers.update(
+                {
+                    "Content-Type": "application/x-www-form-urlencoded",
+                }
+            ),
+        )
+
+    async def wearMedal(self, medal_id: int):
+        """
+        佩戴粉丝牌
+        """
+        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/fansMedal/wear"
+        data = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+            "medal_id": medal_id,
+            "platform": "android",
+            "type": "1",
+            "version": "0",
+        }
+        return await self.__post(
+            url,
+            data=SingableDict(data).signed,
+            headers=self.headers.update(
+                {
+                    "Content-Type": "application/x-www-form-urlencoded",
+                }
+            ),
+        )
+
+    async def getGroups(self):
+        url = "https://api.live.bilibili.com/link_group/v1/member/my_groups"
+        params = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+        }
+        list = (await self.__get(url, params=SingableDict(params).signed, headers=self.headers))['list']
+        for group in list:
+            yield group
+
+    async def signInGroups(self, group_id: int, owner_id: int):
+        url = "https://api.vc.bilibili.com/link_setting/v1/link_setting/sign_in"
+        params = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+            "group_id": group_id,
+            "owner_id": owner_id,
+        }
+        return await self.__get(url, params=SingableDict(params).signed, headers=self.headers)
+
+    async def getOneBattery(self):
+        url = "https://api.live.bilibili.com/xlive/app-ucenter/v1/userTask/UserTaskReceiveRewards"
+        data = {
+            "access_key": self.u.access_key,
+            "actionKey": "appkey",
+            "appkey": Crypto.APPKEY,
+            "ts": int(time.time()),
+        }
+        return await self.__post(url, data=SingableDict(data).signed, headers=self.headers)
```

### Comparing `nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/src/user.py` & `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/src/user.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,355 +1,355 @@
-from aiohttp import ClientSession, ClientTimeout
-import asyncio
-import uuid
-from loguru import logger
-from nonebot.log import logger as log
-from datetime import datetime, timedelta
-
-# sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-
-# logger.remove()
-# logger.add(
-    # sys.stdout,
-    # colorize=True,
-    # format="<green>{time:YYYY-MM-DD HH:mm:ss}</green> <blue> {extra[user]} </blue> <level>{message}</level>",
-    # backtrace=True,
-    # diagnose=True,
-# )
-
-global user
-class BiliUser:
-    def __init__(self, access_token: str, whiteUIDs: str = '', bannedUIDs: str = '', config: dict = {}):
-        from .api import BiliApi
-
-        self.mid, self.name = 0, ""
-        self.access_key = access_token  # 登录凭证
-        try:
-            self.whiteList = list(map(lambda x: int(x if x else 0), str(whiteUIDs).split(',')))  # 白名单UID
-            self.bannedList = list(map(lambda x: int(x if x else 0), str(bannedUIDs).split(',')))  # 黑名单
-        except ValueError:
-            raise ValueError("白名单或黑名单格式错误")
-        self.config = config
-        self.medals = []  # 用户所有勋章
-        self.medalsNeedDo = []  # 用户所有勋章，等级小于20的 未满1500的
-
-        self.session = ClientSession(timeout=ClientTimeout(total=3))
-        self.api = BiliApi(self, self.session)
-
-        self.retryTimes = 0  # 点赞任务重试次数
-        self.maxRetryTimes = 10  # 最大重试次数
-        self.message = []
-        self.errmsg = ["错误日志："]
-        self.uuids = [str(uuid.uuid4()) for _ in range(2)]
-
-    async def loginVerify(self) -> bool:
-        """
-        登录验证
-        """
-        loginInfo = await self.api.loginVerift()
-        self.mid, self.name = loginInfo['mid'], loginInfo['name']
-        #self.log = logger.info(user=self.name)
-        self.log = logger.info(f"b站名称：{self.name}")
-        if loginInfo['mid'] == 0:
-            self.isLogin = False
-            return False
-        userInfo = await self.api.getUserInfo()
-        if userInfo['medal']:
-            medalInfo = await self.api.getMedalsInfoByUid(userInfo['medal']['target_id'])
-            if medalInfo['has_fans_medal']:
-                self.initialMedal = medalInfo['my_fans_medal']
-        self.log = logger.success(str(loginInfo['mid']) + " 登录成功")
-        self.isLogin = True
-        return True
-
-    async def doSign(self):
-        try:
-            signInfo = await self.api.doSign()
-            log.success("签到成功,本月签到次数: {}/{}".format(signInfo['hadSignDays'], signInfo['allDays']))
-            self.message.append(f"【{self.name}】 签到成功,本月签到次数: {signInfo['hadSignDays']}/{signInfo['allDays']}")
-        except Exception as e:
-            log.error(e)
-            self.errmsg.append(f"【{self.name}】" + str(e))
-        userInfo = await self.api.getUserInfo()
-        log.info(
-            "当前用户UL等级: {} ,还差 {} 经验升级".format(userInfo['exp']['user_level'], userInfo['exp']['unext'])
-        )
-        self.message.append(
-            f"【{self.name}】 UL等级: {userInfo['exp']['user_level']} ,还差 {userInfo['exp']['unext']} 经验升级"
-        )
-
-    async def getMedals(self):
-        """
-        获取用户勋章
-        """
-        self.medals.clear()
-        self.medalsNeedDo.clear()
-        async for medal in self.api.getFansMedalandRoomID():
-            if self.whiteList == [0]:
-                if medal['medal']['target_id'] in self.bannedList:
-                    log.warning(f"{medal['anchor_info']['nick_name']} 在黑名单中，已过滤")
-                    continue
-                self.medals.append(medal) if medal['room_info']['room_id'] != 0 else ...
-            else:
-                if medal['medal']['target_id'] in self.whiteList:
-                    self.medals.append(medal) if medal['room_info']['room_id'] != 0 else ...
-                    log.success(f"{medal['anchor_info']['nick_name']} 在白名单中，加入任务")
-        [
-            self.medalsNeedDo.append(medal)
-            for medal in self.medals
-            if medal['medal']['level'] < 20 and medal['medal']['today_feed'] < 1500
-        ]
-
-    async def asynclikeandShare(self, failedMedals: list = []):
-        """
-        点赞 、 分享
-        """
-        if self.config['LIKE_CD'] == 0:
-            log.info("点赞任务已关闭")
-        elif self.config['SHARE_CD'] == 0:
-            log.info("分享任务已关闭")
-        if self.config['LIKE_CD'] == 0 and self.config['SHARE_CD'] == 0:
-            return
-        try:
-            if not failedMedals:
-                failedMedals = self.medalsNeedDo
-            if not self.config['ASYNC']:
-                log.info("同步点赞、分享任务开始....")
-                for index, medal in enumerate(failedMedals):
-                    tasks = []
-                    tasks.append(self.api.likeInteract(medal['room_info']['room_id'])) if self.config[
-                        'LIKE_CD'
-                    ] else ...
-                    tasks.append(self.api.shareRoom(medal['room_info']['room_id'])) if self.config[
-                        'SHARE_CD'
-                    ] else ...
-                    await asyncio.gather(*tasks)
-                    log.success(
-                        f"{medal['anchor_info']['nick_name']} 点赞,分享成功 {index+1}/{len(self.medalsNeedDo)}",
-                    )
-                    await asyncio.sleep(max(self.config['LIKE_CD'], self.config['SHARE_CD']))
-            else:
-                log.info("异步点赞、分享任务开始....")
-                allTasks = []
-                for medal in failedMedals:
-                    allTasks.append(self.api.likeInteract(medal['room_info']['room_id'])) if self.config[
-                        'LIKE_CD'
-                    ] else ...
-                    allTasks.append(self.api.shareRoom(medal['room_info']['room_id'])) if self.config[
-                        'SHARE_CD'
-                    ] else ...
-                await asyncio.gather(*allTasks)
-            await asyncio.sleep(10)
-            await self.getMedals()  # 刷新勋章
-            log.success("点赞、分享任务完成")
-            finallyMedals = [medal for medal in self.medalsNeedDo if medal['medal']['today_feed'] >= 200]
-            failedMedals = [medal for medal in self.medalsNeedDo if medal['medal']['today_feed'] < 200]
-            msg = "20级以下牌子共 {} 个,完成任务 {} 个亲密度大于等于200".format(len(self.medalsNeedDo), len(finallyMedals))
-            log.info(msg)
-            log.warning(
-                "小于200或失败房间: {}... {}个".format(
-                    ' '.join([medals['anchor_info']['nick_name'] for medals in failedMedals[:5]]),
-                    len(failedMedals),
-                ),
-            )
-            if self.retryTimes > self.maxRetryTimes:
-                log.error("任务重试次数过多,停止任务")
-                return
-            if len(finallyMedals) / len(self.medalsNeedDo) <= 0.9:
-                log.warning("成功率过低,重新执行任务")
-                self.retryTimes += 1
-                log.warning("重试次数: {}/{}".format(self.retryTimes, self.maxRetryTimes))
-                await self.asynclikeandShare(failedMedals)
-        except Exception as e:
-            log.exception("点赞、分享任务异常")
-            self.errmsg.append(f"【{self.name}】 点赞、分享任务异常,请检查日志")
-
-    async def like_v3(self, failedMedals: list = []):
-        if self.config['LIKE_CD'] == 0:
-            log.info("点赞任务已关闭")
-            return
-        try:
-            if not failedMedals:
-                failedMedals = self.medalsNeedDo
-            if not self.config['ASYNC']:
-                log.info("同步点赞任务开始....")
-                for index, medal in enumerate(failedMedals):
-                    tasks = []
-                    tasks.append(
-                        self.api.likeInteractV3(medal['room_info']['room_id'], medal['medal']['target_id'])
-                    ) if self.config['LIKE_CD'] else ...
-                    await asyncio.gather(*tasks)
-                    log.success(
-                        f"{medal['anchor_info']['nick_name']} 点赞成功 {index+1}/{len(self.medalsNeedDo)}",
-                    )
-                    await asyncio.sleep(self.config['LIKE_CD'])
-            else:
-                log.info("异步点赞任务开始....")
-                allTasks = []
-                for medal in failedMedals:
-                    allTasks.append(
-                        self.api.likeInteractV3(medal['room_info']['room_id'], medal['medal']['target_id'])
-                    ) if self.config['LIKE_CD'] else ...
-                await asyncio.gather(*allTasks)
-            await asyncio.sleep(10)
-            log.success("点赞任务完成")
-            finallyMedals = [medal for medal in self.medalsNeedDo if medal['medal']['today_feed'] >= 100]
-            msg = "20级以下牌子共 {} 个,完成点赞任务 {} 个".format(len(self.medalsNeedDo), len(finallyMedals))
-            log.info(msg)
-        except Exception as e:
-            log.exception("点赞任务异常")
-            self.errmsg.append(f"【{self.name}】 点赞任务异常,请检查日志")
-
-    async def sendDanmaku(self):
-        """
-        每日弹幕打卡
-        """
-        if not self.config['DANMAKU_CD']:
-            log.info("弹幕任务关闭")
-            return
-        log.info("弹幕打卡任务开始....(预计 {} 秒完成)".format(len(self.medals) * self.config['DANMAKU_CD']))
-        n = 0
-        for medal in self.medals:
-            try:
-                (await self.api.wearMedal(medal['medal']['medal_id'])) if self.config['WEARMEDAL'] else ...
-                danmaku = await self.api.sendDanmaku(medal['room_info']['room_id'])
-                n += 1
-                log.success(
-                    "{} 房间弹幕打卡成功: {} ({}/{})".format(
-                        medal['anchor_info']['nick_name'], danmaku, n, len(self.medals)
-                    ),
-                )
-            except Exception as e:
-                log.error("{} 房间弹幕打卡失败: {}".format(medal['anchor_info']['nick_name'], e))
-                self.errmsg.append(f"【{self.name}】 {medal['anchor_info']['nick_name']} 房间弹幕打卡失败: {str(e)}")
-            finally:
-                await asyncio.sleep(self.config['DANMAKU_CD'])
-        if hasattr(self, 'initialMedal'):
-            (await self.api.wearMedal(self.initialMedal['medal_id'])) if self.config['WEARMEDAL'] else ...
-        log.success("弹幕打卡任务完成")
-        self.message.append(f"【{self.name}】 弹幕打卡任务完成 {n}/{len(self.medals)}")
-        if n >= 5:
-            try:
-                await self.api.getOneBattery()
-                log.success("领取电池成功")
-                self.message.append(f"【{self.name}】 领取电池成功")
-            except Exception as e:
-                log.error("领取电池失败: {}".format(e))
-                self.errmsg.append(f"【{self.name}】 领取电池失败: {str(e)}")
-
-    async def init(self):
-        if not await self.loginVerify():
-            log.error("登录失败 可能是 access_key 过期 , 请重新获取")
-            self.errmsg.append("登录失败 可能是 access_key 过期 , 请重新获取")
-            await self.session.close()
-        else:
-            await self.doSign()
-            await self.getMedals()
-
-    async def start(self):
-        if self.isLogin:
-            tasks = []
-            if self.medalsNeedDo:
-                log.info(f"共有 {len(self.medalsNeedDo)} 个牌子未满 1500 亲密度")
-                tasks.append(self.like_v3())
-                tasks.append(self.watchinglive())
-            else:
-                log.info("所有牌子已满 1500 亲密度")
-            tasks.append(self.sendDanmaku())
-            tasks.append(self.signInGroups())
-            await asyncio.gather(*tasks)
-
-    async def sendmsg(self):
-        if not self.isLogin:
-            await self.session.close()
-            return self.message + self.errmsg
-        await self.getMedals()
-        nameList1, nameList2, nameList3, nameList4 = [], [], [], []
-        for medal in self.medals:
-            if medal['medal']['level'] >= 20:
-                continue
-            today_feed = medal['medal']['today_feed']
-            nick_name = medal['anchor_info']['nick_name']
-            if today_feed >= 1500:
-                nameList1.append(nick_name)
-            elif 1300 < today_feed <= 1400:
-                nameList2.append(nick_name)
-            elif 1200 < today_feed <= 1300:
-                nameList3.append(nick_name)
-            elif today_feed <= 1200:
-                nameList4.append(nick_name)
-        self.message.append(f"【{self.name}】 今日亲密度获取情况如下（20级以下）：")
-
-        for l, n in zip(
-            [nameList1, nameList2, nameList3, nameList4],
-            ["【1500】", "【1300至1400】", "【1200至1300】", "【1200以下】"],
-        ):
-            if len(l) > 0:
-                self.message.append(f"{n}" + ' '.join(l[:5]) + f"{'等' if len(l) > 5 else ''}" + f' {len(l)}个')
-
-        if hasattr(self, 'initialMedal'):
-            initialMedalInfo = await self.api.getMedalsInfoByUid(self.initialMedal['target_id'])
-            if initialMedalInfo['has_fans_medal']:
-                initialMedal = initialMedalInfo['my_fans_medal']
-                self.message.append(
-                    f"【当前佩戴】「{initialMedal['medal_name']}」({initialMedal['target_name']}) {initialMedal['level']} 级 "
-                )
-                if initialMedal['level'] < 20 and initialMedal['today_feed'] != 0:
-                    need = initialMedal['next_intimacy'] - initialMedal['intimacy']
-                    need_days = need // 1500 + 1
-                    end_date = datetime.now() + timedelta(days=need_days)
-                    self.message.append(f"今日已获取亲密度 {initialMedal['today_feed']} (B站结算有延迟，请耐心等待)")
-                    self.message.append(
-                        f"距离下一级还需 {need} 亲密度 预计需要 {need_days} 天 ({end_date.strftime('%Y-%m-%d')},以每日 1500 亲密度计算)"
-                    )
-        await self.session.close()
-        return self.message + self.errmsg + ['---']
-
-    async def watchinglive(self):
-        if not self.config['WATCHINGLIVE']:
-            log.info("每日观看不直播任务关闭")
-            return
-        HEART_MAX = self.config['WATCHINGLIVE']
-        log.info(f"每日{HEART_MAX}分钟任务开始")
-        heartNum = 0
-        while True:
-            tasks = []
-            for medal in self.medalsNeedDo:
-                tasks.append(self.api.heartbeat(medal['room_info']['room_id'], medal['medal']['target_id']))
-            await asyncio.gather(*tasks)
-            heartNum += 1
-            log.info(
-                f"{' '.join([medal['anchor_info']['nick_name'] for medal in self.medalsNeedDo[:5]])} 等共 {len(self.medalsNeedDo)} 个房间的第{heartNum}次心跳包已发送（{heartNum}/{HEART_MAX}）",
-            )
-            await asyncio.sleep(60)
-            if heartNum >= HEART_MAX:
-                break
-        log.success(f"每日{HEART_MAX}分钟任务完成")
-
-    async def signInGroups(self):
-        if not self.config['SIGNINGROUP']:
-            log.info("应援团签到任务关闭")
-            return
-        log.info("应援团签到任务开始")
-        try:
-            n = 0
-            async for group in self.api.getGroups():
-                if group['owner_uid'] == self.mid:
-                    continue
-                try:
-                    await self.api.signInGroups(group['group_id'], group['owner_uid'])
-                except Exception as e:
-                    log.error(group['group_name'] + " 签到失败")
-                    self.errmsg.append(f"应援团签到失败: {e}")
-                    continue
-                log.success(group['group_name'] + " 签到成功")
-                await asyncio.sleep(self.config['SIGNINGROUP'])
-                n += 1
-            if n:
-                log.success(f"应援团签到任务完成 {n}/{n}")
-                self.message.append(f" 应援团签到任务完成 {n}/{n}")
-            else:
-                log.warning("没有加入应援团")
-        except Exception as e:
-            log.exception(e)
-            log.error("应援团签到任务失败: " + str(e))
-            self.errmsg.append("应援团签到任务失败: " + str(e))
+from aiohttp import ClientSession, ClientTimeout
+import asyncio
+import uuid
+from loguru import logger
+from nonebot.log import logger as log
+from datetime import datetime, timedelta
+
+# sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+
+# logger.remove()
+# logger.add(
+    # sys.stdout,
+    # colorize=True,
+    # format="<green>{time:YYYY-MM-DD HH:mm:ss}</green> <blue> {extra[user]} </blue> <level>{message}</level>",
+    # backtrace=True,
+    # diagnose=True,
+# )
+
+global user
+class BiliUser:
+    def __init__(self, access_token: str, whiteUIDs: str = '', bannedUIDs: str = '', config: dict = {}):
+        from .api import BiliApi
+
+        self.mid, self.name = 0, ""
+        self.access_key = access_token  # 登录凭证
+        try:
+            self.whiteList = list(map(lambda x: int(x if x else 0), str(whiteUIDs).split(',')))  # 白名单UID
+            self.bannedList = list(map(lambda x: int(x if x else 0), str(bannedUIDs).split(',')))  # 黑名单
+        except ValueError:
+            raise ValueError("白名单或黑名单格式错误")
+        self.config = config
+        self.medals = []  # 用户所有勋章
+        self.medalsNeedDo = []  # 用户所有勋章，等级小于20的 未满1500的
+
+        self.session = ClientSession(timeout=ClientTimeout(total=3))
+        self.api = BiliApi(self, self.session)
+
+        self.retryTimes = 0  # 点赞任务重试次数
+        self.maxRetryTimes = 10  # 最大重试次数
+        self.message = []
+        self.errmsg = ["错误日志："]
+        self.uuids = [str(uuid.uuid4()) for _ in range(2)]
+
+    async def loginVerify(self) -> bool:
+        """
+        登录验证
+        """
+        loginInfo = await self.api.loginVerift()
+        self.mid, self.name = loginInfo['mid'], loginInfo['name']
+        #self.log = logger.info(user=self.name)
+        self.log = logger.info(f"b站名称：{self.name}")
+        if loginInfo['mid'] == 0:
+            self.isLogin = False
+            return False
+        userInfo = await self.api.getUserInfo()
+        if userInfo['medal']:
+            medalInfo = await self.api.getMedalsInfoByUid(userInfo['medal']['target_id'])
+            if medalInfo['has_fans_medal']:
+                self.initialMedal = medalInfo['my_fans_medal']
+        self.log = logger.success(str(loginInfo['mid']) + " 登录成功")
+        self.isLogin = True
+        return True
+
+    async def doSign(self):
+        try:
+            signInfo = await self.api.doSign()
+            log.success("签到成功,本月签到次数: {}/{}".format(signInfo['hadSignDays'], signInfo['allDays']))
+            self.message.append(f"【{self.name}】 签到成功,本月签到次数: {signInfo['hadSignDays']}/{signInfo['allDays']}")
+        except Exception as e:
+            log.error(e)
+            self.errmsg.append(f"【{self.name}】" + str(e))
+        userInfo = await self.api.getUserInfo()
+        log.info(
+            "当前用户UL等级: {} ,还差 {} 经验升级".format(userInfo['exp']['user_level'], userInfo['exp']['unext'])
+        )
+        self.message.append(
+            f"【{self.name}】 UL等级: {userInfo['exp']['user_level']} ,还差 {userInfo['exp']['unext']} 经验升级"
+        )
+
+    async def getMedals(self):
+        """
+        获取用户勋章
+        """
+        self.medals.clear()
+        self.medalsNeedDo.clear()
+        async for medal in self.api.getFansMedalandRoomID():
+            if self.whiteList == [0]:
+                if medal['medal']['target_id'] in self.bannedList:
+                    log.warning(f"{medal['anchor_info']['nick_name']} 在黑名单中，已过滤")
+                    continue
+                self.medals.append(medal) if medal['room_info']['room_id'] != 0 else ...
+            else:
+                if medal['medal']['target_id'] in self.whiteList:
+                    self.medals.append(medal) if medal['room_info']['room_id'] != 0 else ...
+                    log.success(f"{medal['anchor_info']['nick_name']} 在白名单中，加入任务")
+        [
+            self.medalsNeedDo.append(medal)
+            for medal in self.medals
+            if medal['medal']['level'] < 20 and medal['medal']['today_feed'] < 1500
+        ]
+
+    async def asynclikeandShare(self, failedMedals: list = []):
+        """
+        点赞 、 分享
+        """
+        if self.config['LIKE_CD'] == 0:
+            log.info("点赞任务已关闭")
+        elif self.config['SHARE_CD'] == 0:
+            log.info("分享任务已关闭")
+        if self.config['LIKE_CD'] == 0 and self.config['SHARE_CD'] == 0:
+            return
+        try:
+            if not failedMedals:
+                failedMedals = self.medalsNeedDo
+            if not self.config['ASYNC']:
+                log.info("同步点赞、分享任务开始....")
+                for index, medal in enumerate(failedMedals):
+                    tasks = []
+                    tasks.append(self.api.likeInteract(medal['room_info']['room_id'])) if self.config[
+                        'LIKE_CD'
+                    ] else ...
+                    tasks.append(self.api.shareRoom(medal['room_info']['room_id'])) if self.config[
+                        'SHARE_CD'
+                    ] else ...
+                    await asyncio.gather(*tasks)
+                    log.success(
+                        f"{medal['anchor_info']['nick_name']} 点赞,分享成功 {index+1}/{len(self.medalsNeedDo)}",
+                    )
+                    await asyncio.sleep(max(self.config['LIKE_CD'], self.config['SHARE_CD']))
+            else:
+                log.info("异步点赞、分享任务开始....")
+                allTasks = []
+                for medal in failedMedals:
+                    allTasks.append(self.api.likeInteract(medal['room_info']['room_id'])) if self.config[
+                        'LIKE_CD'
+                    ] else ...
+                    allTasks.append(self.api.shareRoom(medal['room_info']['room_id'])) if self.config[
+                        'SHARE_CD'
+                    ] else ...
+                await asyncio.gather(*allTasks)
+            await asyncio.sleep(10)
+            await self.getMedals()  # 刷新勋章
+            log.success("点赞、分享任务完成")
+            finallyMedals = [medal for medal in self.medalsNeedDo if medal['medal']['today_feed'] >= 200]
+            failedMedals = [medal for medal in self.medalsNeedDo if medal['medal']['today_feed'] < 200]
+            msg = "20级以下牌子共 {} 个,完成任务 {} 个亲密度大于等于200".format(len(self.medalsNeedDo), len(finallyMedals))
+            log.info(msg)
+            log.warning(
+                "小于200或失败房间: {}... {}个".format(
+                    ' '.join([medals['anchor_info']['nick_name'] for medals in failedMedals[:5]]),
+                    len(failedMedals),
+                ),
+            )
+            if self.retryTimes > self.maxRetryTimes:
+                log.error("任务重试次数过多,停止任务")
+                return
+            if len(finallyMedals) / len(self.medalsNeedDo) <= 0.9:
+                log.warning("成功率过低,重新执行任务")
+                self.retryTimes += 1
+                log.warning("重试次数: {}/{}".format(self.retryTimes, self.maxRetryTimes))
+                await self.asynclikeandShare(failedMedals)
+        except Exception as e:
+            log.exception("点赞、分享任务异常")
+            self.errmsg.append(f"【{self.name}】 点赞、分享任务异常,请检查日志")
+
+    async def like_v3(self, failedMedals: list = []):
+        if self.config['LIKE_CD'] == 0:
+            log.info("点赞任务已关闭")
+            return
+        try:
+            if not failedMedals:
+                failedMedals = self.medalsNeedDo
+            if not self.config['ASYNC']:
+                log.info("同步点赞任务开始....")
+                for index, medal in enumerate(failedMedals):
+                    tasks = []
+                    tasks.append(
+                        self.api.likeInteractV3(medal['room_info']['room_id'], medal['medal']['target_id'])
+                    ) if self.config['LIKE_CD'] else ...
+                    await asyncio.gather(*tasks)
+                    log.success(
+                        f"{medal['anchor_info']['nick_name']} 点赞成功 {index+1}/{len(self.medalsNeedDo)}",
+                    )
+                    await asyncio.sleep(self.config['LIKE_CD'])
+            else:
+                log.info("异步点赞任务开始....")
+                allTasks = []
+                for medal in failedMedals:
+                    allTasks.append(
+                        self.api.likeInteractV3(medal['room_info']['room_id'], medal['medal']['target_id'])
+                    ) if self.config['LIKE_CD'] else ...
+                await asyncio.gather(*allTasks)
+            await asyncio.sleep(10)
+            log.success("点赞任务完成")
+            finallyMedals = [medal for medal in self.medalsNeedDo if medal['medal']['today_feed'] >= 100]
+            msg = "20级以下牌子共 {} 个,完成点赞任务 {} 个".format(len(self.medalsNeedDo), len(finallyMedals))
+            log.info(msg)
+        except Exception as e:
+            log.exception("点赞任务异常")
+            self.errmsg.append(f"【{self.name}】 点赞任务异常,请检查日志")
+
+    async def sendDanmaku(self):
+        """
+        每日弹幕打卡
+        """
+        if not self.config['DANMAKU_CD']:
+            log.info("弹幕任务关闭")
+            return
+        log.info("弹幕打卡任务开始....(预计 {} 秒完成)".format(len(self.medals) * self.config['DANMAKU_CD']))
+        n = 0
+        for medal in self.medals:
+            try:
+                (await self.api.wearMedal(medal['medal']['medal_id'])) if self.config['WEARMEDAL'] else ...
+                danmaku = await self.api.sendDanmaku(medal['room_info']['room_id'])
+                n += 1
+                log.success(
+                    "{} 房间弹幕打卡成功: {} ({}/{})".format(
+                        medal['anchor_info']['nick_name'], danmaku, n, len(self.medals)
+                    ),
+                )
+            except Exception as e:
+                log.error("{} 房间弹幕打卡失败: {}".format(medal['anchor_info']['nick_name'], e))
+                self.errmsg.append(f"【{self.name}】 {medal['anchor_info']['nick_name']} 房间弹幕打卡失败: {str(e)}")
+            finally:
+                await asyncio.sleep(self.config['DANMAKU_CD'])
+        if hasattr(self, 'initialMedal'):
+            (await self.api.wearMedal(self.initialMedal['medal_id'])) if self.config['WEARMEDAL'] else ...
+        log.success("弹幕打卡任务完成")
+        self.message.append(f"【{self.name}】 弹幕打卡任务完成 {n}/{len(self.medals)}")
+        if n >= 5:
+            try:
+                await self.api.getOneBattery()
+                log.success("领取电池成功")
+                self.message.append(f"【{self.name}】 领取电池成功")
+            except Exception as e:
+                log.error("领取电池失败: {}".format(e))
+                self.errmsg.append(f"【{self.name}】 领取电池失败: {str(e)}")
+
+    async def init(self):
+        if not await self.loginVerify():
+            log.error("登录失败 可能是 access_key 过期 , 请重新获取")
+            self.errmsg.append("登录失败 可能是 access_key 过期 , 请重新获取")
+            await self.session.close()
+        else:
+            await self.doSign()
+            await self.getMedals()
+
+    async def start(self):
+        if self.isLogin:
+            tasks = []
+            if self.medalsNeedDo:
+                log.info(f"共有 {len(self.medalsNeedDo)} 个牌子未满 1500 亲密度")
+                tasks.append(self.like_v3())
+                tasks.append(self.watchinglive())
+            else:
+                log.info("所有牌子已满 1500 亲密度")
+            tasks.append(self.sendDanmaku())
+            tasks.append(self.signInGroups())
+            await asyncio.gather(*tasks)
+
+    async def sendmsg(self):
+        if not self.isLogin:
+            await self.session.close()
+            return self.message + self.errmsg
+        await self.getMedals()
+        nameList1, nameList2, nameList3, nameList4 = [], [], [], []
+        for medal in self.medals:
+            if medal['medal']['level'] >= 20:
+                continue
+            today_feed = medal['medal']['today_feed']
+            nick_name = medal['anchor_info']['nick_name']
+            if today_feed >= 1500:
+                nameList1.append(nick_name)
+            elif 1300 < today_feed <= 1400:
+                nameList2.append(nick_name)
+            elif 1200 < today_feed <= 1300:
+                nameList3.append(nick_name)
+            elif today_feed <= 1200:
+                nameList4.append(nick_name)
+        self.message.append(f"【{self.name}】 今日亲密度获取情况如下（20级以下）：")
+
+        for l, n in zip(
+            [nameList1, nameList2, nameList3, nameList4],
+            ["【1500】", "【1300至1400】", "【1200至1300】", "【1200以下】"],
+        ):
+            if len(l) > 0:
+                self.message.append(f"{n}" + ' '.join(l[:5]) + f"{'等' if len(l) > 5 else ''}" + f' {len(l)}个')
+
+        if hasattr(self, 'initialMedal'):
+            initialMedalInfo = await self.api.getMedalsInfoByUid(self.initialMedal['target_id'])
+            if initialMedalInfo['has_fans_medal']:
+                initialMedal = initialMedalInfo['my_fans_medal']
+                self.message.append(
+                    f"【当前佩戴】「{initialMedal['medal_name']}」({initialMedal['target_name']}) {initialMedal['level']} 级 "
+                )
+                if initialMedal['level'] < 20 and initialMedal['today_feed'] != 0:
+                    need = initialMedal['next_intimacy'] - initialMedal['intimacy']
+                    need_days = need // 1500 + 1
+                    end_date = datetime.now() + timedelta(days=need_days)
+                    self.message.append(f"今日已获取亲密度 {initialMedal['today_feed']} (B站结算有延迟，请耐心等待)")
+                    self.message.append(
+                        f"距离下一级还需 {need} 亲密度 预计需要 {need_days} 天 ({end_date.strftime('%Y-%m-%d')},以每日 1500 亲密度计算)"
+                    )
+        await self.session.close()
+        return self.message + self.errmsg + ['---']
+
+    async def watchinglive(self):
+        if not self.config['WATCHINGLIVE']:
+            log.info("每日观看不直播任务关闭")
+            return
+        HEART_MAX = self.config['WATCHINGLIVE']
+        log.info(f"每日{HEART_MAX}分钟任务开始")
+        heartNum = 0
+        while True:
+            tasks = []
+            for medal in self.medalsNeedDo:
+                tasks.append(self.api.heartbeat(medal['room_info']['room_id'], medal['medal']['target_id']))
+            await asyncio.gather(*tasks)
+            heartNum += 1
+            log.info(
+                f"{' '.join([medal['anchor_info']['nick_name'] for medal in self.medalsNeedDo[:5]])} 等共 {len(self.medalsNeedDo)} 个房间的第{heartNum}次心跳包已发送（{heartNum}/{HEART_MAX}）",
+            )
+            await asyncio.sleep(60)
+            if heartNum >= HEART_MAX:
+                break
+        log.success(f"每日{HEART_MAX}分钟任务完成")
+
+    async def signInGroups(self):
+        if not self.config['SIGNINGROUP']:
+            log.info("应援团签到任务关闭")
+            return
+        log.info("应援团签到任务开始")
+        try:
+            n = 0
+            async for group in self.api.getGroups():
+                if group['owner_uid'] == self.mid:
+                    continue
+                try:
+                    await self.api.signInGroups(group['group_id'], group['owner_uid'])
+                except Exception as e:
+                    log.error(group['group_name'] + " 签到失败")
+                    self.errmsg.append(f"应援团签到失败: {e}")
+                    continue
+                log.success(group['group_name'] + " 签到成功")
+                await asyncio.sleep(self.config['SIGNINGROUP'])
+                n += 1
+            if n:
+                log.success(f"应援团签到任务完成 {n}/{n}")
+                self.message.append(f" 应援团签到任务完成 {n}/{n}")
+            else:
+                log.warning("没有加入应援团")
+        except Exception as e:
+            log.exception(e)
+            log.error("应援团签到任务失败: " + str(e))
+            self.errmsg.append("应援团签到任务失败: " + str(e))
```

### Comparing `nonebot_plugin_bilifan-0.1.3/nonebot_plugin_bilifan/users.yaml` & `nonebot_plugin_bilifan-0.1.4/nonebot_plugin_bilifan/users.yaml`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-USERS:
-    - access_key: # 注意冒号后的空格 否则会读取失败 英文冒号
-      white_uid: 0 # 白名单用户ID, 可以是多个用户ID, 以逗号分隔,填写后只会打卡这些用户,黑名单失效，不用就填0
-      banned_uid: 0 # 黑名单UID 同上,填了后将不会打卡，点赞，分享 用英文逗号分隔 不填则不限制,两个都填0则不限制,打卡所有直播间
-    - access_key:
-      white_uid: 0
-      banned_uid: 0
-    # 注意对齐
-    # 多用户以上格式添加
-    # 井号后为注释 井号前后必须有空格！井号前后必须有空格！井号前后必须有空格！
-    # 冒号后面也要有空格！冒号前面也要有空格！冒号前面也要有空格！
-    # 英文冒号,英文逗号！英文逗号！英文逗号！
-CRON: 0 0 * * * # 0 0 * * *
-# 这里是 cron 表达式, 第一个参数是小时, 第二个参数是分钟
-# 例如每天凌晨0点0分执行一次为 0 0 * * *
-# 如果不填,则不使用内置定时器,填写正确后要保持该进程一直运行
-
-#########以下为自定义配置#########
-ASYNC: 1 # 异步执行,默认异步执行,设置为0则同步执行,开启异步后,将不支持设置点赞CD时间
-
-LIKE_CD: 2 # 点赞间隔时间,单位秒,默认2秒,仅为同步时生效,设置为0则不点赞
-
-DANMAKU_CD: 6 # 弹幕间隔时间,单位秒,默认6秒,设置为0则不发弹幕打卡,只能同步打卡
-
-WATCHINGLIVE: 65 # 每日观看直播时长，单位 min ，设置为0则关闭, 默认 65 分钟
-
-WEARMEDAL: 0 # 是否弹幕打卡时自动带上当前房间的粉丝牌，避免房间有粉丝牌等级禁言，默认关闭，设置为1则开启
-
-SIGNINGROUP: 2 # 应援团签到CD时间,单位秒,默认2秒,设置为0则不签到
-# 说明：
-# 本项目中的异步执行指的是：同时点赞或者分享所有直播间，速度非常快，但缺点就是可能会被B站吞掉亲密度，所以建议粉丝牌较少的用户开启异步执行
-# 粉丝牌数大于30的用户建议使用同步，会更加稳定。缺点就是速度比较慢，但是可以设置点赞和分享的CD时间，避免被B站吞掉亲密度
-# 多用户之间依然是异步，不受配置影响
+USERS:
+    - access_key: # 注意冒号后的空格 否则会读取失败 英文冒号
+      white_uid: 0 # 白名单用户ID, 可以是多个用户ID, 以逗号分隔,填写后只会打卡这些用户,黑名单失效，不用就填0
+      banned_uid: 0 # 黑名单UID 同上,填了后将不会打卡，点赞，分享 用英文逗号分隔 不填则不限制,两个都填0则不限制,打卡所有直播间
+    - access_key:
+      white_uid: 0
+      banned_uid: 0
+    # 注意对齐
+    # 多用户以上格式添加
+    # 井号后为注释 井号前后必须有空格！井号前后必须有空格！井号前后必须有空格！
+    # 冒号后面也要有空格！冒号前面也要有空格！冒号前面也要有空格！
+    # 英文冒号,英文逗号！英文逗号！英文逗号！
+CRON: 0 0 * * * # 0 0 * * *
+# 这里是 cron 表达式, 第一个参数是小时, 第二个参数是分钟
+# 例如每天凌晨0点0分执行一次为 0 0 * * *
+# 如果不填,则不使用内置定时器,填写正确后要保持该进程一直运行
+
+#########以下为自定义配置#########
+ASYNC: 1 # 异步执行,默认异步执行,设置为0则同步执行,开启异步后,将不支持设置点赞CD时间
+
+LIKE_CD: 2 # 点赞间隔时间,单位秒,默认2秒,仅为同步时生效,设置为0则不点赞
+
+DANMAKU_CD: 6 # 弹幕间隔时间,单位秒,默认6秒,设置为0则不发弹幕打卡,只能同步打卡
+
+WATCHINGLIVE: 65 # 每日观看直播时长，单位 min ，设置为0则关闭, 默认 65 分钟
+
+WEARMEDAL: 0 # 是否弹幕打卡时自动带上当前房间的粉丝牌，避免房间有粉丝牌等级禁言，默认关闭，设置为1则开启
+
+SIGNINGROUP: 2 # 应援团签到CD时间,单位秒,默认2秒,设置为0则不签到
+# 说明：
+# 本项目中的异步执行指的是：同时点赞或者分享所有直播间，速度非常快，但缺点就是可能会被B站吞掉亲密度，所以建议粉丝牌较少的用户开启异步执行
+# 粉丝牌数大于30的用户建议使用同步，会更加稳定。缺点就是速度比较慢，但是可以设置点赞和分享的CD时间，避免被B站吞掉亲密度
+# 多用户之间依然是异步，不受配置影响
```

### Comparing `nonebot_plugin_bilifan-0.1.3/pyproject.toml` & `nonebot_plugin_bilifan-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-[tool.poetry]
-name = "nonebot_plugin_bilifan"
-version = "0.1.3"
-description = "刷bili粉丝牌子的机器人插件"
-authors = ["Agnes_Digital <Z735803792@163.com>"]
-license = "GPLv3"
-readme = "README.md"
-homepage = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
-repository = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
-keywords = ["bilibili", "nonebot2", "plugin"]
-classifiers = [
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Operating System :: OS Independent",
-]
-include = [
-    "LICENSE","README.md"
-]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-nonebot2 = "^2.0.0rc4"
-nonebot-adapter-onebot = ">=2.1.5"
-nonebot_plugin_apscheduler = ">=0.2.0"
-
-pillow = "^9.3.0"
-aiohttp = "^3.8.3"
-aiohttp-socks = "^0.8.0"
-pyyaml = "^6.0"
-qrcode = "^7.4.2"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "nonebot_plugin_bilifan"
+version = "0.1.4"
+description = "刷bili粉丝牌子的机器人插件"
+authors = ["Agnes_Digital <Z735803792@163.com>"]
+license = "GPLv3"
+readme = "README.md"
+homepage = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
+repository = "https://github.com/Agnes4m/nonebot_plugin_bilifan"
+keywords = ["bilibili", "nonebot2", "plugin"]
+classifiers = [
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: OS Independent",
+]
+include = [
+    "LICENSE","README.md"
+]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+nonebot2 = "^2.0.0rc4"
+nonebot-adapter-onebot = ">=2.1.5"
+nonebot_plugin_apscheduler = ">=0.2.0"
+
+pillow = "^9.3.0"
+aiohttp = "^3.8.3"
+aiohttp-socks = "^0.8.0"
+pyyaml = "^6.0"
+qrcode = "^7.4.2"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_bilifan-0.1.3/README.md` & `nonebot_plugin_bilifan-0.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-<div align="center">
-  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
-  <br>
-  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot_plugin_bilifan
-_✨自动b站粉丝牌✨_
-
-<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">
-        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">
-</a>
-<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">
-        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">
-</a>
-<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
-        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">
-        <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">
-</a>
-    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
-    <img src="https://img.shields.io/badge/nonebot-2.0.0rc4-red.svg" alt="NoneBot">
-</div>
-
-## 配置
-
-启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件
-
-## 指令
-
-- b站登录 - 返回b站二维码，扫码登录，绑定qq号
-- 开始刷牌子 - 开始执行命令
-- 自动刷牌子 - 添加或取消定时任务
-- 取消自动刷牌子 - 取消定时任务
-- 删除全部的定时任务 - [超管]删除全部的定时任务
-
-
-</details>
-
-## 🙈 其他
-
-- 本项目仅供学习使用，请勿用于商业用途
-- [爱发电](https://afdian.net/a/agnes_digital)
-- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
-
-## 🌐 感谢
-
-- [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他
+<div align="center">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <br>
+  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot_plugin_bilifan
+_✨自动b站粉丝牌✨_
+
+<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">
+</a>
+<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
+        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">
+        <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">
+</a>
+    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0rc4-red.svg" alt="NoneBot">
+</div>
+
+## 配置
+
+启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件
+
+## 指令
+
+- b站登录 - 返回b站二维码，扫码登录，绑定qq号
+- 删除登录信息 - 删除登录信息和绑定
+- 开始刷牌子 - 开始执行命令
+- 自动刷牌子 - 添加或取消定时任务
+- 取消自动刷牌子 - 取消定时任务
+- 删除全部的定时任务 - [超管]删除全部的定时任务
+
+
+</details>
+
+## 🙈 其他
+
+- 本项目仅供学习使用，请勿用于商业用途
+- [爱发电](https://afdian.net/a/agnes_digital)
+- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
+
+## 🌐 感谢
+
+- [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
-- è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å¼å§å·çå­ -
-å¼å§æ§è¡å½ä»¤ - èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ -
-åæ¶èªå¨å·çå­ - åæ¶å®æ¶ä»»å¡ - å é¤å¨é¨çå®æ¶ä»»å¡ -
+- è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å é¤ç»å½ä¿¡æ¯ -
+å é¤ç»å½ä¿¡æ¯åç»å® - å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤ -
+èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ - åæ¶èªå¨å·çå­ -
+åæ¶å®æ¶ä»»å¡ - å é¤å¨é¨çå®æ¶ä»»å¡ -
 [è¶ç®¡]å é¤å¨é¨çå®æ¶ä»»å¡  ## ð å¶ä» -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [ç±åçµ](https://
 afdian.net/a/agnes_digital) - [GPL-3.0 License](https://github.com/Agnes4m/
 nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
 Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https://github.com/
 XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
```

### Comparing `nonebot_plugin_bilifan-0.1.3/PKG-INFO` & `nonebot_plugin_bilifan-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilifan
-Version: 0.1.3
+Version: 0.1.4
 Summary: 刷bili粉丝牌子的机器人插件
 Home-page: https://github.com/Agnes4m/nonebot_plugin_bilifan
 License: GPLv3
 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -12,17 +12,14 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
@@ -60,14 +57,15 @@
 ## 配置
 
 启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件
 
 ## 指令
 
 - b站登录 - 返回b站二维码，扫码登录，绑定qq号
+- 删除登录信息 - 删除登录信息和绑定
 - 开始刷牌子 - 开始执行命令
 - 自动刷牌子 - 添加或取消定时任务
 - 取消自动刷牌子 - 取消定时任务
 - 删除全部的定时任务 - [超管]删除全部的定时任务
 
 
 </details>
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.1.4 Summary:
 å·biliç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
 nonebot_plugin_bilifan License: GPLv3 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.9 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Programming Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0) Requires-Dist: nonebot-adapter-
 onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist:
 nonebot_plugin_apscheduler (>=0.2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_bilifan
 Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
-- è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å¼å§å·çå­ -
-å¼å§æ§è¡å½ä»¤ - èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ -
-åæ¶èªå¨å·çå­ - åæ¶å®æ¶ä»»å¡ - å é¤å¨é¨çå®æ¶ä»»å¡ -
+- è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å é¤ç»å½ä¿¡æ¯ -
+å é¤ç»å½ä¿¡æ¯åç»å® - å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤ -
+èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ - åæ¶èªå¨å·çå­ -
+åæ¶å®æ¶ä»»å¡ - å é¤å¨é¨çå®æ¶ä»»å¡ -
 [è¶ç®¡]å é¤å¨é¨çå®æ¶ä»»å¡  ## ð å¶ä» -
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [ç±åçµ](https://
 afdian.net/a/agnes_digital) - [GPL-3.0 License](https://github.com/Agnes4m/
 nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
 Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https://github.com/
 XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
```

