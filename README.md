# Project Breeze

A framework for drafting shorter legal documents.

## Introduction

Project Breeze hides templated language away so you can focus on what really matters.  With a short tag in your document, you can reference our standard templates and dramatically reduce the complexity of your documents.

### Key Benefits

#### 1. Reference templated text and shorten your documents

![Reference text with an import statement](https://github.com/ProjectBreeze/ProjectBreeze/raw/master/docs/resources/images/animated/example-import.gif)

#### 2. Tailor to your needs and call out the changes

![Customize an import statement](https://github.com/ProjectBreeze/ProjectBreeze/raw/master/docs/resources/images/animated/example-customization.gif)

#### 3. Use as much or as little as you want

![Choose to use as much or as little as you want](https://github.com/ProjectBreeze/ProjectBreeze/raw/master/docs/resources/images/animated/example-minimal-use.gif)

#### 4. Read our templates once and re-use it anywhere

![Read once and never again](https://github.com/ProjectBreeze/ProjectBreeze/raw/master/docs/resources/images/animated/example-read-once.gif)

## Quick Start

### Reading a Document

1. Find the Import Statements and locate the associated Packages in the Project Breeze repository
2. Note any additional information in the Import Statement including:
   1. values for fields in the Package;
   2. plain language changes that may alter the meaning of the text; and
   3. a version number that may direct you to an older version of the repository.
3. Read your document, and insert the Packages inline as if they are subsections of the document.  The Pacakges are not attached to the beginning or end of the document akin to traditional appendices or schedules.  For clarity, an Import Statement in the document is deemed to be substited with the corresponding contents of the Package.

### Writing a Document

1. Introduce the Project Breeze Documentation in your legal document.
   1. "This document is governed by the Project Breeze Documentation located at [https://github.com/ProjectBreeze/ProjectBreeze/blob/master/docs/interpretation-reference.md](https://github.com/ProjectBreeze/ProjectBreeze/blob/master/docs/interpretation-reference.md)."
2. Import a Project Breeze Package by using the keyword Import and including at least:
   1. a section/clause/chapter/article number for the package;
   2. a valid URL to a Project Breeze Package; and
   3. values for mandatory fields.
3. The Import Statement may also include:
   1. a version number, which must also be accompanied by a version number in the URL;
   2. a definition (Import ... as "NDA"); and
   3. changes with reference to specific clauses.
      1. If the Import Statement includes or excludes specific references, only the selected clauses are Imported into the document and the rest of the Package is ignored and do not form part of the document.
4. Import with changes by describing the changes in plain language after the Import Statement.  See the examples below.

### Examples

1.  Simple Import:
    1.  Import https://github.com/ProjectBreeze/ProjectBreeze/blob/master/demo-library/provisions/general/entire-agreement.md
2.  Import with changes in plain language:
    1.  Import https://github.com/ProjectBreeze/ProjectBreeze/blob/master/demo-library/provisions/general/force-majeure.md however, include "nuclear catastrophes as an example of force majeure.


### Frequently Asked Questions

#### 1. Are Project Breeze documents legally enforceable?

Yes.  Agreements are enforceable in any form of media so long as all parties understand, agree and intend to be legally bound by it.  Legal documents already make heavy use of links to corporate websites, external policies, etc.  Project Breeze is merely an organizational paradigm and is functionally no different.

#### 2. How does Project Breeze differ from a clause library?

A clause library only benefits the party drafting a document.  From the perspective of outside parties, a clause library is private to the drafter.  There is no standard source of truth, and no guarantee the drafter has not modified the language.  As such, those parties do not save any time at all, they are forced to read the document from top to bottom no matter what clause library is used.

#### 3. How can I contribute?

The Project Breeze GitHub repository is located at [https://github.com/ProjectBreeze/ProjectBreeze](https://github.com/ProjectBreeze/ProjectBreeze).  GitHub offers a number of tools to make suggestions or to call out issues.

## Documentation

These instructions only cover the basics of Project Breeze.  If you are interested in the documentation, head over to [https://github.com/ProjectBreeze/ProjectBreeze/blob/master/docs/interpretation-reference.md](https://github.com/ProjectBreeze/ProjectBreeze/blob/master/docs/interpretation-reference.md).

## Copyright and License

All code, text and documentation Copyright ©2020 Project Breeze.  No commercial use is currently granted for the contents of this repository.

## Disclaimer

Project Breeze does not offer legal advice.  The use of Project Breeze does not create a relationship with Project Breeze in any way.  Project Breeze and contributors to Project Breeze offer no warranty of any kind and disclaim all forms of liability.  Please seek independent legal advice before using Project Breeze.