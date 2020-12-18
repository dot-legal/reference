# Project Breeze Documentation ("Interpretation Reference")

1. Introduction
   1. The purpose of Project Breeze is to simplify legal documents by hosting reusable pieces of legal text (each called a "Package").  Users of Project Breeze may reference the standardized Packages available on the Project Breeze platform and include them right in their own documents.
   2. The core of Project Breeze is to allow the "Import" of Packages.  The act of Importing a Package is similar to referencing attached appendices with several key differences that are outlined in this Interpretation Reference.
   3. This Interpretation Reference will set out the rules for understanding and using Project Breeze.
2. Disclaimer
   1. Project Breeze is not a law firm and does not offer legal advice.  The use of Project Breeze creates no relationship with Project Breeze in any way.  Project Breeze and contributors to Project Breeze offer no warranty of any kind and disclaim all forms of liability.  Please seek independent legal advice before using Project Breeze.
3. Getting Started
   1. Writing a Document
      1. Include a clause to introduce the Project Breeze Interpretation Reference.
      2. To Import a Project Breeze Package, a statement (called an "Import Statement") must be made beginning with the keyword Import and the statement must include at minimum:
         1. its own section/clause/chapter/article number; and
         2. a valid URL to a Project Breeze Package.
            1. A valid URL must point to either a specific version or to the latest version of a Project Breeze Package.
      3. The Import Statement may also include:
         1. A version number, which must also be accompanied by a version number in the URL
         2. A definition (Import ... as "NDA")
         3. References to or exclusions of specific enumerated clauses
            1. If the Import Statement includes or excludes specific references, only the selected clauses are Imported into the document and the rest of the Package is ignored and do not form part of the document.
         4. Field inputs
            1. Certain packages may include fillable fields with identifiers.  You should include inputs for each field.
      4. Packages that are Imported into a document are read inline as if they are subsections of the section of the document where they are Imported.  They are not attached to the beginning or end of the document akin to traditional appendices or schedules.  For clarity, an Import Statement in the contract are deemed to be substituted with the corresponding contents of the Package.
      5. Import with exceptions
         <!-- Amendments in terms of import, BUT do this -->
      6. Examples:
         <!-- Examples are missing -->
   2. Reading a Document
4. Interpretation
   1. Clause Enumeration
      1. All subdivided text in a Package, be they sections, subsections or any other form of subdivided text will be enumerated with numbers.  For example, there may be sections and several levels of subsections.  The reference to a sub-subsection would read as Section 1(2)(3).
      2. To preserve numbering between Package versions, inserted sections between two cardinal numbers may be given decimal enumerators.
   2. Versioning and Amendments
      1. If the Import of a Project Breeze Package specifies a corresponding version number, the parties will restrict and prohibit the use of preceding or subsequent versions of the Package in the reading or interpretation of the Package.  The Import will reference only the exact language used in the specific version referenced.
      2. Where the Import of a Project Breeze Package does not specify a version number, the intention is to refer to the Package on the Project Breeze platform including all changes in both language and intent made from time to time.
         1. Any time a new version of the Package is published on the Project Breeze platform, such version will undergo an "Acceptance Period" of thirty (30) calendar days beginning from the date it is published.  The Import of a Project Breeze Package without a version number will refer to the latest version of such Package which is not undergoing an Acceptance Period.  During any Acceptance Period, any party may unilaterally object to the changes made by giving clear written notice to all other parties.  Such written notice will lock the Imported Package and it will refer to the latest version of the Package not undergoing an Acceptance Period from the date the written notice was given.
         2. At the end of the Acceptance Period, the new version will replace the existing version with an effective date of the end of the Acceptance Period.
      3. Where a section reference in the Import Statement is no longer accurate to a new version, the section reference will refer, to the greatest extent possible and in good faith, the natural successor based on the history of changes available.  Where such context remains ambiguous, the section reference will refer to the latest version in which a natural successor can be determined.
      <!-- Minor versions for grammar, moderate for rephrasing but same intention, major for significant changes -->
      <!-- Need rules on succession and branching (will link to new package which will automatically be a major revision) -->
   3. Document Continuity
      1. In the event that the Project Breeze platform is unavailable for any reason, the GitHub repository at [https://github.com/ProjectBreeze/ProjectBreeze](https://github.com/ProjectBreeze/ProjectBreeze) is an accurate duplicate of the content on the Project Breeze platform.  The corresponding Package on GitHub will have the same force as the Package on the Project Breeze platform.
   4. Hierarchy
      1. By the very nature of incorporating and amending referenced Packages, provisions may overlap and contradict each other.  To determine which provision will govern and control, Project Breeze strictly adheres to a hierarchy of levels in which overlapping or contradictory provisions in a higher level of the hierarchy will override those in a lower level.  For clarity, the governing and controlling provision will be the provision found in the higher level Package.
      2. In the event where the hierarchy does not establish an unambiguous overriding provision, the provision that appears earlier in the document will govern and control.  For the purposes of determining an overriding provision, the Import of a Package will occur inline, meaning that its placement in the document lies where the reference is made and not at the end of the document like traditional appendices and schedules.
      3. To determine establish the hierarchy, the lowest level comprises of Packages which do not contain references to any other Package.  Packages which reference the lowest level are next in the hierarchy and the level will continue to raise with each subsequent reference.  The final document drafted by the end-user is on the highest level of the hierarchy, and will govern and control over any Package.
   5. Definitions
      <!-- Include clarification on: -->
      <!-- SCOPING DEFINITIONS WITHIN THE PACKAGE IF CONFLICTING -->
      <!-- REFERENCE RULES TO REFER TO DEFINING PACKAGE -->
   6. Metadata, Instructions, Comments and Formatting
      1. The metadata, instructions, comments and formatting contained in each Package are for reference purposes only and will not affect in any way the meaning or interpretation of the Package or any document it is made part of.
5. Versioning/GitHub
   <!-- Need significant discussion on Github changes versus actual releases -->
   <!-- Version should be denoted as a field -->
   <!-- Allow suggesting changes, can we do this anonymously or through a web service? -->
6. Syntax
   1. Intention
      1. The intention of Project Breeze is to standardize drafting language to reduce ambiguity where it is not intended.  Many of the syntactic and structural choices made by Project Breeze deliberately mirror basic computer engineering concepts and such concepts may be used to further clarify areas where this Interpretation Reference alone are insufficient.
   2. Keywords
      1. Whether capitalized or not, except as otherwise expressly provided or unless the context otherwise requires, the following keywords will have the following meanings:
         <!-- Definitions should be made to the keywords -->
         1. Import
         2. Override
            <!-- 1. to substitute one part of the package -->
         3. Package
   3. Drafting standards
      1. Document
      2. Party
         1. Always assume more than 2 parties, addressed as all parties
7. Best Practices
   <!-- Entirely missing -->
   1. Git
      1. Each clause/provision should, as much as possible, be committed individually for detailed descriptions.  Longer notes should be placed and deleted in the docs section.
   2. Backups
      1. Though GitHub is a reliable secondary store of Project Breeze materials, users with important legal documents should take advantage of the many tools available on GitHub to backup Packages from time to time (including downloading, cloning and forking).
   3. General formatting
      1. Underlining is the preferred styling to make text conspicuous when required.  Use of all capitalized text is highly discouraged.
