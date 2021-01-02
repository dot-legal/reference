# Project Breeze Documentation ("Interpretation Reference")

Last Updated: January 1, 2021

1. Introduction
    1. The purpose of Project Breeze is to simplify and modularize legal documents through reusable pieces of legal text (each called a "Package").  Users of Project Breeze may reference the standard Packages available on the platform and include them in their own documents.
    2. You can reference one or more Packages with a single line and drastically shorten and simplify your document (the process is called an "Import").  These lines are like hyperlinks to a set of general terms or a reference to a schedule or exhibit.  The structure for this reference is outlined in this Interpretation Reference, but the following is a simple example:
        ```
        Import demo-library/provisions/general/amendment.md {"version": "0.0.0.2-alpha"}
        ```
    3. This Interpretation Reference will set out the rules for using and understanding Project Breeze.  **Any party to a document governed by this Interpretation Reference represents that they have read and understood this Interpretation Reference.**
    4. This Interpretation Reference may be updated from time to time.  For rules regarding which version applies, please see the "Versioning and Amendments" section below.
2. Getting Started
    1. Writing a Document
        1. Start by introducing this Interpretation Reference:
            ```
            This document is governed by the Project Breeze Interpretation Reference located at https://github.com/ProjectBreeze/ProjectBreeze/blob/master/docs/interpretation-reference.md.
            ```
        2. Then Import a Package.  You need to include a clear statement (called an "Import Statement") with the keyword "Import", a "Path" to the correct Package, and optional "Fields" inside a set of curly braces.
            ```
            Import demo-library/provisions/general/notices.md {"email_addresses": "admin@projectbreeze.com and support@projectbreeze.com"}
            ```
        3. Packages that are Imported into a document are read inline as if they are subsections of the section of the document where they are Imported.  They are not attached to the beginning or end of the document like traditional appendices or schedules.  An Import Statement is deemed to be substituted with the corresponding contents of the Package.
            ```
            1. The headings in this document are for convenience only and do not constitute a part of this document. The headings will not be deemed to limit or affect any of the provisions contained in this document.
            2. Import demo-library/provisions/general/counterparts.md {"version": "0.0.0.2-alpha"}
            3. All notices and other communications required or permitted under this document will be sent by email.
            ```
            is read as, and is identical to:
            ```
            1. The headings in this document are for convenience only and do not constitute a part of this document. The headings will not be deemed to limit or affect any of the provisions contained in this document.
            2. This document may be executed in any number of counterparts and by the different signatories on separate counterparts, each of which, when so executed, shall be deemed an original. All such counterparts shall constitute one and the same document.
            3. All notices and other communications required or permitted under this document will be sent by email.
            ```
        4. If you want to change an Imported clause, you may follow an Import Statement with plain language stating those changes.
            ```
            Import demo-library/provisions/general/force-majeure.md however, include "nuclear catastrophes" as an example of force majeure.
            ```
    2. Reading a Document
        1. Enter your Import Statement into the tool on the website to retrieve the legal text.  Be sure to include the optional Fields if they were included.
        2. Read the legal text inline where the document Imports the Package as if it is a subsection of the section of the document where it is Imported.
        3. Note any stated changes that may immediately follow the Import Statement.
3. Interpretation
    1. Import Statement
        1. The Import Statement **must** start with the word "Import" followed by a valid Path to a Package.
        2. The Import Statement may also include:
            1. Its own clause/section/article number
                1. Primarily for ease of reference
                2. See the Syntax section for more information on Numbering and References
            2. Changes
                1. Where you want to change the Package slightly, you may state those changes immediately following the Import statement in plain language.
            3. Field inputs in curly braces
                1. Allows for some inputs into template language (for example, the notices clause may include a field for an email address)
                2. See the Fields section for more information
            4. A specific version in the Field inputs
                1. If you want to ensure the Package language stays the same and will not be updated, you can state the specific version in the Field inputs.
                2. See the Versioning and Amendments section for more information
        3. An example of a longer Import Statement is:
            ```
            1. Import demo-library/provisions/general/notices.md {"version": "0.0.0.2-alpha", "email_addresses": "admin@projectbreeze.com and support@projectbreeze.com"} however, a second email may only be sent 10 calendar days after the initial email.
            ```
    2. Fields
        1. Certain Packages may include empty Fields as denoted by an inline code block (surrounded by the backtick or ` character) and a field name.  An example is the notices clause which reads:
            ```
            All notices and other communications required or permitted under this document will be sent by email to the following email addresses: `email_addresses`.
            ```
        2. The Import Statement should include Field inputs within curly braces, and both the label and input should be surrounded by double brackets.  For example:
            ```
            Import demo-library/provisions/general/notices.md {"version": "0.0.0.2-alpha", "email_addresses": "admin@projectbreeze.com and support@projectbreeze.com"}
            ```
            which will produce this result:
            ```
            All notices and other communications required or permitted under this document will be sent by email to the following email addresses: admin@projectbreeze.com and support@projectbreeze.com.
            ```
    3. Versioning and Amendments
        1. If the Import Statement includes a specific version in its Fields, the Import will reference only the language used in that particular version.
        2. Where the Import Statement does not specify a version, the intention will be to refer to the latest version of the Package and to benefit from all updates to language and intent made from time to time.
            1. Major Changes
                1. Major Changes to a Package will be separated into a new Package and will have no effect on the existing Package.  Major Changes are for significant changes in the intention, or where there will be real and practical effects.
                2. However, Minor Changes to a Package are updates that will become the latest version of the Package.  Minor Changes are generally limited to clarification and rephrasing.  For certain Packages, the intent may change to reflect best practices or a new legal requirement.
                3. The distinction between Major and Minor Change will be determined by Project Breeze in its sole discretion.
            2. Acceptance Period
                1. Any time a new version of Project Breeze is published, such version will undergo an "Acceptance Period" of thirty (30) calendar days beginning from the date it is published.  The Import of a Project Breeze Package without a version will refer to the latest version of such Package which is not undergoing an Acceptance Period.  During any Acceptance Period, any party may unilaterally object to the changes made by giving clear written notice to all other parties.  Such written notice will lock the Imported Package and it will refer to the latest version of the Package not undergoing an Acceptance Period from the date the written notice was given.
                2. At the end of the Acceptance Period, the new version will replace the existing version with an effective date of the end of the Acceptance Period.
        3. Where a reference number in the Import Statement is no longer accurate to a new version, the reference number will refer, to the greatest extent possible and in good faith, the logical successor based on the history of changes available.  Where such context remains ambiguous, the reference number will refer to the latest version in which a logical successor can be determined.
        4. Note that versions will refer to "Releases" per GitHub terminology.  In other words, there may be intermediary, non-final changes which do not count as versions.
    4. Orders of Precedence
        1. Clauses in different Packages may overlap and contradict each other.  Subject to any explicit language otherwise, to determine which clause will govern and control (to "Override"), Packages are placed in a hierarchy.  The document is on the highest level, its direct Imports are on the next level, and Imports within those Packages are on a lower level, and so on.  Clauses in a higher level will Override over those in a lower level.  For clarity, the document will always Override over any Package unless explicitly stated otherwise.
        2. Where the hierarchy does not establish an unambiguous overriding clause (for example, where the clauses are placed on the same level), the clause that appears earlier in the document will Override later clauses.  Note that the Import of a Package occurs inline, meaning that its placement in the document lies where the reference is made and not at the end of the document or elsewhere.
    5. Metadata, Instructions, Comments and Formatting
        1. The metadata, instructions, comments and format contained in each Package are for reference purposes only and will not affect in any way the meaning or interpretation of the Package or any document it is made part of.
    6. Continuity and Backups
        1. In the event that the Project Breeze platform is unavailable for any reason, the GitHub repository at [https://github.com/ProjectBreeze/ProjectBreeze](https://github.com/ProjectBreeze/ProjectBreeze) is an accurate duplicate of the content on the Project Breeze platform.  The corresponding Package on GitHub will have the same force as the Package on the Project Breeze platform.
4. Syntax
    1. Intention
        1. The intention of Project Breeze is to standardize legal language to reduce ambiguity where it is not intended.  Many of the choices deliberately mirror basic computer engineering concepts and such concepts may be used to further clarify areas where this Interpretation Reference alone is insufficient.
        2. Enforcing strict requirements, particularly with syntax, will eventually result in some mistake.  All parties to a document governed by this Interpretation Reference will read and interpret such documents in good faith through the eyes of a reasonable third party.  Where syntax is indecipherable by Project Breeze's official tools and the intention is plainly discernible, the error should be ignored and the syntax corrected.
    2. Format
        1. Packages are written in the Markdown format (see the Commonmark spec at: https://commonmark.org/).
        2. Inline code blocks (according to the Commonmark spec) are used to denote Fields that are replaced by values provided in the Import Statement.
        3. Some metadata that does not form part of the legal text may be stored as comments in this fashion:
            ```
            [Simplified]: # (Each party needs written permission from all the other parties to assign or transfer this document to someone else.)
            ```
            The square bracket indicates the type of metadata, and the round bracket indicates the associated metadata.
    3. Drafting standards
        1. Document
            1. Refer to the working document as "this document" as opposed to "this Agreement", "this Contract", etc.
        2. Parties
            1. Always assume more than 2 parties, addressed as "all parties" or "any party", etc.
        3. Numbering and References
            1. All subdivided text in a Package, whether sections, subsections or any other form of subdivided text will be numerated with cardinal numbers.  For example, there may be sections and several levels of subsections.  The reference to a sub-subsection would read as Section 1(2)(3).
            2. To preserve numbering between Package versions, inserted sections between two cardinal numbers may be given decimal numbers such as 1.1 or 2.1.
        4. Emphasis
            1. Emphasis will be bolded or italicized.  All caps should never be used.
5. Contributing
    1. Contributions, including suggestions, may be made via the GitHub repository as Issues, suggested Changes or Pull Requests.
6. Best Practices
    1. Git
        1. Each clause should, as much as possible, be committed via Git individually for detailed descriptions.  Longer notes may be referenced in the Git description, then placed into the docs folder.
    2. Backups
        1. Though GitHub is a reliable secondary store of Project Breeze materials, users with important legal documents should take advantage of the many tools available on GitHub to backup Packages from time to time (including downloading, cloning and forking).
    3. General formatting
        1. Underlining is the preferred styling to make text conspicuous when required.  Use of all capitalized text is highly discouraged.
7. Disclaimer
    1. **Project Breeze is not a law firm and does not offer legal advice.  The use of Project Breeze creates no relationship with Project Breeze in any way.  Project Breeze and contributors to Project Breeze offer no warranty of any kind and disclaim all forms of liability.  Please seek independent legal advice before using Project Breeze.**
    2. **Project Breeze is currently in ALPHA phase, which means that virtually all parts of Project Breeze, including this Interpretation Reference and the Package may change drastically.  Please do not use Project Breeze in any serious or binding legal documents.**
