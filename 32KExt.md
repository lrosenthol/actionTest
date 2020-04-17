**Document Management --- Defining extensions to PDF --- Part 1:
Overview**

> **Warning**
>
> **This document is not an ISO International Standard. It is
> distributed for review and comment. It is subject to change without
> notice and may not be referred to as an International Standard.**
>
> **Recipients of this draft are invited to submit, with their comments,
> notification of any relevant patent rights of which they are aware and
> to provide supporting documentation.**
>
> © ISO 2020
>
> All rights reserved. Unless otherwise specified, or required in the
> context of its implementation, no part of this publication may be
> reproduced or utilized otherwise in any form or by any means,
> electronic or mechanical, including photocopying, or posting on the
> internet or an intranet, without prior written permission. Permission
> can be requested from either ISO at the address below or ISO's member
> body in the country of the requester.
>
> ISO copyright office
>
> CP 401 • Ch. de Blandonnet 8
>
> CH-1214 Vernier, Geneva
>
> Phone: +41 22 749 01 11
>
> Fax: +41 22 749 09 47
>
> Email: copyright\@iso.org
>
> Website: www.iso.org
>
> Published in Switzerland

Contents

 {#section .TOC-Heading}

[Foreword iv](#_Toc353342667)

[Introduction v](#_Toc353342668)

[1 Scope 1](#scope)

[2 Normative references 1](#normative-references)

[3 Terms and definitions 1](#terms-and-definitions)

[4 Defining extensions to PDF 1](#defining-extensions-to-pdf)

[4.1 Process 1](#process)

[4.2 Defining the extension 2](#defining-the-extension)

[4.3 Implementation Experience 2](#implementation-experience)

[]{#_Toc353342667 .anchor}Foreword

ISO (the International Organization for Standardization) is a worldwide
federation of national standards bodies (ISO member bodies). The work of
preparing International Standards is normally carried out through ISO
technical committees. Each member body interested in a subject for which
a technical committee has been established has the right to be
represented on that committee. International organizations, governmental
and non-governmental, in liaison with ISO, also take part in the work.
ISO collaborates closely with the International Electrotechnical
Commission (IEC) on all matters of electrotechnical standardization.

*Any feedback or questions on this document should be directed to the
user's national standards body. A complete listing of these bodies can
be found at
[www.iso.org/members.html](https://www.iso.org/members.html).*

[]{#_Toc353342668 .anchor}Introduction

The PDF specification (ISO 32000) is a very large and complex document,
which has many individual features catering for a diverse range of
industries and users. As a result, ISO 32000 is a difficult document to
prepare, review and ensure that the highest possible technical scrutiny
is applied to all aspects prior to publication. Throughout the history
of PDF, a number of features have also been proposed which have never
been widely adopted for various reasons -- some technical, some related
to business relevance, and some related to poor specification occurring
before implementation. These lesser used features also increase the size
and complexity of PDF implementations, and poor specifications lead to
lower levels of interoperability.

To address these issues ISO/TC 171/SC 2/WG 8 has decided on a new
process for the addition of new PDF features/capabilities. It is based
on the collective experience of WG 8 Subject Matter Experts (SMEs) and
aims to ensure better technical outcomes in a timely manner by relating
specification development to implementation, while providing a pathway
for new features to become part of future core PDF specifications (i.e.,
be included in future parts of ISO 32000).

Document Management --- Defining extensions to PDF --- Part 1: Overview

Scope
=====

The Portable Document Format (PDF) enables users to exchange and view
electronic documents easily and reliably, independent of the environment
in which they were created or the environment in which they are viewed
or printed. Reliable interoperability of PDF is achieved through a
common technical understanding of ISO 32000 (PDF) as realised as
software implementations.

This document describes the process agreed and adopted by ISO/TC 171/SC
2/WG 8 for developing new features or capabilities (extensions) for PDF,
as candidates for possible future adoption into future parts of PDF (ISO
32000). It is expected that PDF extension specifications will not be
developed solely by ISO/TC 171/SC 2/WG 8, but instead by other groups
where the relevant SMEs are present. However, the decision to include
any PDF extension specification into a future part of ISO 32000 is based
on resolution by ISO/TC 171/SC 2/WG 8.

Normative references
====================

The following documents are referred to in the text in such a way that
some or all of their content constitutes requirements of this document.
For dated references, only the edition cited applies. For undated
references, the latest edition of the referenced document (including any
amendments) applies.

ISO 32000-2 *Document Management* *--- Portable Document Format ---
Part 2: PDF 2.0*

*W3C World Wide Web Consortium Process Document -*
<https://www.w3.org/2019/Process-20190301>

Terms and definitions
=====================

For the purposes of this document, the terms and definitions given in
ISO 32000 and the following apply.

ISO and IEC maintain terminological databases for use in standardization
at the following addresses:

--- ISO Online browsing platform: available at
[[https://www.iso.org/obp]{.underline}](https://www.iso.org/obp)

--- IEC Electropedia: available at
[[http://www.electropedia.org/]{.underline}](http://www.electropedia.org/)

3.1

PDF extension specification

::: {.Definition}
ISO publication describing a new feature or capability that extends ISO
32000
:::

Defining extensions to PDF 
==========================

Process
-------

This agreed process can be summarised as:

-   New features / capabilities for PDF will be published as separate
    ISO documents using standard ISO processes (TR, TS, or IS, as
    decided on a case-by-case basis).

    -   NOTE: These separate smaller PDF extension specifications allow
        a more focused technical review and a more streamlined
        publication process as only the new feature/capability and its
        impact on core PDF is under review.

-   Each independent feature can be championed by a Subject Matter
    Expert (SME) as Project Leader (PL) and prepared on an independent
    timeline appropriate for its level of complexity and industry
    urgency.

-   PDF Extensions cannot remove existing functionality from ISO 32000;
    however, they may suggest that existing features are deprecated.
    Note that ISO 32000-2 carefully defines deprecation in order to
    support backwards compatibility and legacy documents.

-   PDF Extensions can modify existing functionality to ISO 32000, such
    as adding new values to an existing key (e.g. a new type of 3D
    stream or a new transparency blending mode).

-   Each PDF extension specification needs to also provide at least two
    PDF files that include the documented functionality. These example
    files may be either hand-crafted or automatically generated but must
    be directly examinable by SMEs but need not be made available to the
    general public.

-   Two (or more) independently developed processor implementations
    (i.e. Implementation Experience) that show sufficient functionality
    to demonstrate that a common technical understanding and
    interoperability is achieved from the PDF extension specification
    are required (See ‎4.3).

Since PDF extension specifications are ISO documents in their own right,
they may also be normatively referenced by other ISO documents (such as
PDF subset standards).

Once a business case is presented to ISO/TC 171/SC 2/WG 8 for a new
feature/capability described in a published PDF extension specification,
whether this be via proof of industry adoption or formal submission from
industry bodies, the PDF extension specification may, at the discretion
of ISO/TC 171/SC 2/WG 8, then be merged into the next part of ISO 32000
to become a core part of all future PDF specifications. When the future
part of ISO 32000 is published, the related PDF extension specification
document will then likely be withdrawn.

Defining the extension
----------------------

The content of these PDF extension specifications should mimic the style
and formatting of ISO 32000, to permit future merging with very minimal
changes, and should omit the type of material that is not typically
found in ISO 32000 (such as extensive background or explanatory
information or precise implementation details).

ISO 32000 defines a mechanism and process for the addition of new keys
to PDF \[Annex E, Extending PDF\] and a way to document their usage in a
PDF \[7.12.2 & 7.12.3, Extensions dictionary\]. As described in Annex E,
second class names are used to support private workflows and proprietary
data. Since documents developed according to this specification are for
use in public workflows and will be developed as part of an
international standardization process, first class names shall be used.
These first-class names shall be reviewed and approved by ISO/TC 171/SC
2/WG 8. In addition, all extension documents shall include an extensions
dictionary with a prefix listed in the specification.

Clause 12.11 of ISO 32000-2 discusses Document Requirements that can be
specified in a document to inform a conforming processor whether the
document should be processed given the functionality of the processor.
It is recommended that all extension documents should include new
requirement types (12.11.2, Table 275) for the new functionality they
provide.

Implementation Experience
-------------------------

Implementation experience is required to show that a specification is
sufficiently clear and complete, to ensure that independent
interoperable implementations of each feature of the specification will
be realized. To ensure this, ISO/TC 171/SC 2/WG 8 will consider (though
not be limited to) these questions from the W3C Process Document:

-   is each feature of the current specification implemented, and how is
    this demonstrated?

-   are there independent interoperable implementations of the current
    specification?

-   are there implementations created by people other than the authors
    of the specification?

-   is there implementation experience at all levels of the
    specification\'s ecosystem (authoring, consuming, publishing...)?

-   are there reports of difficulties or problems with implementation?

Planning and accomplishing a demonstration of (interoperable)
implementations can be very time consuming. It is recommended that a
plan for how a specification will demonstrate interoperable
implementations is determined early in the development process.

There are no detailed requirements imposed on such implementations --
they may be proprietary, open- or closed-source, proof of concept level,
plug-in based, etc. -- but their output must be available for
examination by SMEs to determine that they demonstrate sufficient
interoperability.
