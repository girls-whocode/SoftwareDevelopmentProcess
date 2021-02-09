# Software Versioning

[:arrow\_backward: Documentation Scopes](Documentation_Scopes.md) | [:house: Home](../README.md) | [Source Control :arrow\_forward:](Source_Control.md)
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
  * [**Software versioning** :arrow\_backward: (Current Page)](Software_Versioning.md)
  * [Source Control](Source_Control.md)
  * [Project references](Project_References.md)

</p>
</details>

## Overview

All software released must have a version number that follows the pattern on *Major.Minor.Revision.BuildRelease.*  This build number must be incremented with each production release of the software.

### ***Major (Indicates full production release.)***

1. A large code base change has taken place.
1. Significant customer facing changes have taken place.
1. Changes have been made that prevent backwards compatibility.
1. Redirection of product has occurred.

### ***Minor***

1. Minor enhancements are made that do not effect compatibility.
1. New features are added that have minimal impact on the interface.
1. New features\functions are added that do not affect existing customers.
1. Bug fixes and error corrections are implemented.

### ***Revision (Only used for BA testing and SQA.)***

1. Each iteration of testing.

### ***Build Release (Use for developers)***

1. Development testing
