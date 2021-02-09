# Document Scopes

[:arrow\_backward: Development Cycle](Dev_Cycle.md) | [:house: Home](../README.md) | [Software versioning :arrow\_forward:](Software_Versioning.md)
<details><summary>Menu Map</summary>
<p>

* [Home](../README.md)
  * [Code Reviews](Code_Reviews.md)
  * [Coding Standards](Coding_Standards.md)
  * [Development Cycle](Dev_Cycle.md)
  * [**Documentation Scopes** :arrow\_backward: (Current Page)](Documentation_Scopes.md)
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
  * [Source Control](Source_Control.md)
  * [Project references](Project_References.md)

</p>
</details>

## What is the "Wiki"

Wiki is Hawaiian for "fast; quick." Wiki was introduced into the lexicon by a computer programmer named Ward Cunningham in 1995 when he created collaborative software that he called WikiWikiWeb. As a noun, wiki means "a website that allows anyone to add, delete or revise content by using a web browser."

Wiki was intended to be used as a web based browser editor to create quick documents. Long after the birth of Wiki, special formatting has been adopted into the Wiki pages called Markdown language. John Gruber created the Markdown language in 2004 in collaboration with Aaron Swartz on the syntax, with the goal of enabling people "to write using an easy-to-read and easy-to-write plain text format, optionally convert it to structurally valid XHTML (or HTML)".

GitLab (and GitHub) uses a special form of Markdown called GFM. In 2017, GitHub released a formal specification of their GitHub Flavored Markdown (GFM) that is based on CommonMark.

Using the Wiki uses a limited GFM system that makes custom formatting nonexistent. Using MD files allows you to expand the GFM to Kramdown markdown language, which supports many more features, including custom styles and classes.

## Documents available

|   | Title | Description |
|:-:|:------|:------------|
| ![Development Doc](images/devdoc.png) | [Dev Document Explanation](Document_Design.md) | Old versions of the documentation template and Design scope. |
| ![Markdown](images/markdown.png) | [Markdown Language Guide](Markdown_Language_Guide.md) | A guide to assist in creating markdown pages for simple styling. |
| ![Markdown](images/markdown.png) | [Markdown Lint Guide](Markdown_Lint_Guide.md) | A style checker and lint tool for Markdown/CommonMark files. |
| ![Readme](images/readme.png) | [Your README.md](Create_README.md) | Create a impressive `README.md` for users to read and understand. |

## MD Files

An MD file is a text file created using one of several possible dialects of the Markdown language. It is saved in plain text format but includes inline text symbols that define how to format the text (e.g., bold, indentations, headers, table formatting). MD files are designed for authoring plain text documentation that can be easily converted to HTML.

GitLab (and GitHub) uses Kramdown for their markdown language.