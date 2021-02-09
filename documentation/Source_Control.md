# Source Control

[:arrow\_backward: Software versioning](Software_Versioning.md) | [:house: Home](../README.md) | [Code Reviews :arrow\_forward:](Code_Reviews.md)
<details><summary>Menu Map</summary>
<p>

* [Home](../README.md)
  * [Code Reviews](Code_Reviews.md)
  * [Coding Standards](Coding_Standards.md)
  * [Development Cycle](Dev_Cycle.md)
  * [Documentation Scopes](Documentation_Scopes.md)
    * [Dev Documentation](Document_Design.md)
    * [Markdown Language Guide](Markdown_Language_Guide.md)
      * [Block Quotes](md_pages/Blockquotes_Tutorial.md)
      * [Colors](md_pages/Colors_Tutorial.md)
      * [Emojis](md_pages/Emojis_Tutorial.md)
      * [Emphasis](md_pages/Emphasis_Tutorial.md)
      * [Footnotes](md_pages/Footnotes_Tutorial.md)
      * [Headings](md_pages/Headings_Tutorial.md)
      * [Horizontal Rules](md_pages/Horizontal_Ruiles_Tutorial.md)
      * [Line Breaks](md_pages/Line_Breaks_Tutorial.md)
      * [Links](md_pages/Links_Tutorial.md)
      * [Lists](md_pages/Lists_Tutorial.md)
      * [Math](md_pages/Math_Tutorial.md)
      * [Paragraphs](md_pages/Paragraphs_Tutorial.md)
      * [Syntax Highlighted Code](md_pages/Syntax_Highlighed_Code_Tutorial.md)
      * [Tables](md_pages/Tables_Tutorial.md)
    * [Markdown Lint Guide](Markdown_Lint_Guide.md)
    * [Your README.md](Create_README.md)
  * [Software versioning](Software_Versioning.md)
  * [**Source Control** :arrow\_backward: (Current Page)](Source_Control.md)
  * [Project references](Project_References.md)

</p>
</details>

## Overview

* The selected source control management to be used with all source code is Git.
* All commits should have meaningful comments.
* Production builds must have a matching commit with the production build number
  * *Some comment Build 1.1.1.1*
  * The build number can be added to a previous commit with *git commit --amend*
* All work performed must be done in a branch.  No code changes to master.
* Master must be merged into a branch before submitting changes for code review or testing.
* Once code changes have passed code review and testing, the branch can be merged into master and a production build can be made for release.

## GitLab

* Related apps should belong to the same group
* All major and minor releases must be documented in the project’s Wiki.  An entry should be made for each version release with subentries giving an overview of the included changes.  When possible attach any related files or emails.
  * 1.1.1.1
    * Added feature X
    * Fixed bug Y