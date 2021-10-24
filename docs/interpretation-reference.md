# reference.legal Documentation ("Interpretation Reference")

Last Updated: October 24, 2021

## Introduction

The purpose of reference.legal is to create the tools necessary for the legal profession to finally rally behind one standard set of legal texts.

We modularize legal documents through reusable pieces of legal text, each called a "**Package**".  Users may link or reference the standard Packages available on the platform and include them in their own documents.

You can reference one or more Packages to shorten and simplify your document.  These lines are like hyperlinks to a set of general terms or a reference to a schedule or exhibit.  The structure for this reference is outlined in this Interpretation Reference, but the following is a simple example:

```
Incorporate http://reference.legal/v1/provisions/general/headings/.
```

This Interpretation Reference will set out the rules for using and understanding reference.legal.  ***Any party to a document governed by this Interpretation Reference represents that they have read and understood this Interpretation Reference.***

## Getting Started

### Writing a Document

#### Linking to a Package

Incorporate our standard headings clause by linking to it:

```
Incorporate http://reference.legal/v1/provisions/general/headings/.
```

#### Inline Reading

Packages that are incorporated into a document are read inline as if they are subsections of the section of the document where they are linked to.  They are not attached to the beginning or end of the document like traditional appendices or schedules.  Please see the Interpretation section of this document to see an example of inline reading.

#### Changes to the Template

If you want to change reference.legal's standard template, you may follow the link with plain language stating those changes.

```
Incorporate http://reference.legal/demo-library/provisions/general/force-majeure/ however, "reasonable efforts" may not, under any circumstances, exceed 30 calendar days.
```

#### Locking Down the Text

If you want to lock the text to exactly what you see, add a date stamp (YYYY-MM-DD format) to the end of your link.  Otherwise, we may make adjustments to keep up with best practices.  Text that is not locked down will be considered "amended from time to time" and will be deemed to be accepted by both parties.

```
Incorporate http://reference.legal/v1/agreements/non-disclosure-agreements/mutual-non-disclosure-agreement/2020-01-08.
```

### Reading a Document

Access the link referenced in your document with any modern web browser.  The displayed text will be in the center of the page.  Any additional tools on the page will not be a part of or affect the text in any way.  The text should be read inline where the link first appeared.  It acts as a section of the document, not an appendix or schedule.  Please see the Interpretation section of this document to see an example of inline reading.

Note any additional language in the document that may change or affect the legal text.  It should immediately follow the link.

```
Incorporate http://reference.legal/demo-library/provisions/general/force-majeure/ however, "reasonable efforts" may not, under any circumstances, exceed 30 calendar days.
```

## Interpretation

### Inline Reading

Packages that are incorporated into a document are read inline as if they are subsections of the section of the document where they are linked to.  They are not attached to the beginning or end of the document like traditional appendices or schedules.

```
10. The headings in this document are for convenience only and do not constitute a part of this document. The headings will not be deemed to limit or affect any of the provisions contained in this document.
11. Incorporate http://reference.legal/v1/provisions/general/counterparts/.
12. All notices and other communications required or permitted under this document will be sent by email.
```

is read as, and is identical to:

```
10. The headings in this document are for convenience only and do not constitute a part of this document. The headings will not be deemed to limit or affect any of the provisions contained in this document.
11. This document may be executed in any number of counterparts and by the different signatories on separate counterparts, each of which, when so executed, shall be deemed an original. All such counterparts shall constitute one and the same document.
12. All notices and other communications required or permitted under this document will be sent by email.
```

### Versioning and Amendments

Where a hyperlink is not locked to a version (does not include a date stamp in the URL), the intention will be to refer to the latest version of the Package and to benefit from all updates to language and intent made from time to time.  The goal is to continuously accept minor changes to improve and adhere to best practices, but to reserve major changes to other mechanisms.

#### Major and Minor Changes

Major Changes to a Package will be separated into a new Package and will have no effect on the existing Package.  Major Changes are for significant changes in the intention, or where there will be real and practical effects.  However, Minor Changes to a Package are updates that will become the latest version of the Package.  Minor Changes are generally limited to clarification and rephrasing.  For certain Packages, the intent may change to reflect best practices or a new legal requirement.  The distinction between Major and Minor Change will be determined by reference.legal in its sole discretion.

#### GitHub Processes

Versions will refer to "Releases" per GitHub terminology.  In other words, there may be intermediary, non-final changes and notes which do not count as versions.  These intermediary changes are called "Commits" per GitHub terminology.

### Orders of Precedence

Clauses in different Packages may overlap and contradict each other.  Subject to any explicit language otherwise, to determine which clause will govern and control (to "**Override**"), Packages are placed in a hierarchy.  The document is on the highest level, its direct links are on the next level, and links within those links are on a lower level, and so on.  Clauses in a higher level will Override over those in a lower level.  For clarity, the document will always Override over any Package unless explicitly stated otherwise.

Where the hierarchy does not establish an unambiguous overriding clause (for example, where the clauses are placed on the same level), the clause that appears earlier in the document will Override later clauses.  Note that the incorporation of a Package occurs inline, meaning that its placement in the document lies where the reference is made and not at the end of the document or elsewhere.

### Metadata, Instructions, Comments and Formatting

The metadata, instructions, comments and format contained in each Package are for reference purposes only and will not affect in any way the meaning or interpretation of the Package or any document it is made part of.  Additional elements of the webpage, such as the header, footer and toolbars will also not affect in any way the meaning or interpretation of the Package or any document it is made part of.

### Continuity and Backups

In the unlikely event that the reference.legal platform is unavailable for any reason, the GitHub repository at [https://github.com/dot-legal/reference/](https://github.com/dot-legal/reference/) is an accurate duplicate of the content on the reference.legal platform.  The corresponding Package on GitHub will have the same force as the Package on the reference.legal platform.  Please note the version of the documents when using GitHub.

## Syntax

### Intention

The intention of reference.legal is to standardize legal language to reduce ambiguity where it is not intended.  All parties to a document governed by this Interpretation Reference will read and interpret such documents in good faith through the eyes of a reasonable third party.  Where syntax is indecipherable but the intention is plainly discernible, the error should be ignored in favor of the clear intention of the user.

### Format

#### Markdown

Packages are written in the Markdown format (see the Commonmark spec at: https://commonmark.org/).

#### Fields

Inline code blocks (according to the Commonmark spec) are used to denote Fields.

#### Metadata

Some metadata that does not form part of the legal text may be stored as comments in this fashion:
    ```
    [Simplified]: # (Each party needs written permission from all the other parties to assign or transfer this document to someone else.)
    ```
    The square bracket indicates the type of metadata, and the round bracket indicates the associated metadata.

### Drafting Standards

#### Plain Language

1. Favor the use of plain language over archaic legalese.
2. Use of Oxford commas is preferred.
3. Numbering should break down into ordered lists whenever possible.

#### Document

1. Refer to the working document as "this document" as opposed to "this Agreement", "this Contract", etc.

#### Parties

1. Always assume more than 2 parties, addressed as "all parties" or "any party", etc.

#### Numbering and References

1. All subdivided text in a Package, whether sections, subsections or any other form of subdivided text will be numerated with cardinal numbers.  For example, there may be sections and several levels of subsections.  The reference to a sub-subsection would read as Section 1(2)(3).
2. To preserve numbering between Package versions, inserted sections between two cardinal numbers may be given decimal numbers such as 1.1 or 2.1.

#### Emphasis

1. Emphasis will be bolded or italicized.  All caps should never be used.
2. Definitions should be bolded where they are defined.

## Contributions

The reference.legal GitHub repository is located at [https://github.com/dot-legal/reference/](https://github.com/dot-legal/reference/).  GitHub offers a number of tools to make suggestions or to call out issues.  However, our roadmap includes additional tools in the [https://reference.legal/](https://reference.legal/) website to make it easy for anyone to comment and make suggestions.

## Best Practices

### Git

Each Package should, where possible, be committed via Git individually for granular descriptions.  Longer notes may be referenced in the Git description, then placed into the docs folder.

### Backups

Though GitHub is a reliable secondary store of reference.legal materials, users with important legal documents should take advantage of the many tools available on GitHub to backup Packages from time to time (including downloading, cloning and forking).

### Disclaimer

***reference.legal is not a law firm and does not offer legal advice.  The use of reference.legal creates no relationship with reference.legal in any way.  reference.legal and contributors to reference.legal offer no warranty of any kind and disclaim all forms of liability.  reference.legal is provided "as is".  Please seek independent legal advice before using reference.legal.***

***reference.legal is currently in ALPHA phase, which means that virtually all parts of reference.legal, including this Interpretation Reference and the Packages may change drastically.  Please do not use reference.legal in any binding legal document.***
