[:arrow\_backward: Documenting](Documentation Scopes) | [Home](home) | [Markdown Language Guide](Markdown_Language_Guide) | [Paragraphs :arrow\_forward:](Paragraphs_Tutorial)

## Headings Overview
To create a heading, add number signs (\#) in front of a word or phrase. The number of number signs you use should correspond to the heading level. For example, to create a heading level three (\<h3>), use three number signs (e.g., \#\#\# My Header).

| **Markdown** | **HTML** | **Rendered Output** | **Notes** |
|:-------------|:---------|:--------------------|:----------|
| #·Heading level 1 | \<h1>Heading level 1\</h1> | <h1>Heading level 1</h1> | H1 Header |
| #··········foo·········· | \<h1>foo\</h1> | <h1>foo</h1> | Trailing spacing is ignored |
| ···# foo | \<h1>foo\</h1> | <h1>foo</h1> | Up to 3 spaces are ignored |
| ##·Heading level 2 | \<h2>Heading level 2\</h2> | <h2>Heading level 2</h2> | H2 Header |
| ###·Heading level 3 | \<h3>Heading level 3\</h3> | <h3>Heading level 3</h3> | H3 Header |
| ####·Heading level 4 | \<h4>Heading level 4\</h4> | <h4>Heading level 4</h4> | H4 Header |
| #####·Heading level 5 | \<h5>Heading level 5\</h5> | <h5>Heading level 5</h5> | H5 Header |
| ######·Heading level 6 | \<h6>Heading level 6\</h6> | <h6>Heading level 6</h6> | H6 Header |

## Incorrect header formats

| **Text** | **HTML** | **Rendered Output**| **What is wrong?** |
|:---------|:---------|:-------------------|:-------------------|
| #######·Heading | \<p>#######·Heading\</p> | ####### Heading | Using more then six \# characters will not be a heading |
| #5·heading | \<p>#5·heading \</p> | #5 heading | At least one space is required between the # characters and the heading’s contents, unless the heading is empty. |
| #hashtag | \<p>#hashtag\</p> | #hashtag | At least one space is required between the # characters and the heading’s contents, unless the heading is empty. |
| \##·foo | \<p>## foo\</p> | ## foo | Escape cannot be used at the beginning of # character |
| ····# foo | \<code>foo\</code> | <code>foo</code> | 4 or more spaces will not work |

[:arrow\_backward: Back to Table of Contents](Markdown_Language_Guide)