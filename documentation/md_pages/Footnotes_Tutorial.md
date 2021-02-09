[:arrow\_backward: Lists](Lists_Tutorial) | [Home](home) | [Markdown Language Guide](Markdown_Language_Guide) | [Horizontal Rules :arrow\_forward:](Horizontal_Ruiles_Tutorial)

## Footnotes
Footnotes allow you to add notes and references without cluttering the body of the document. When you create a footnote, a superscript number with a link appears where you added the footnote reference. Readers can click the link to jump to the content of the footnote at the bottom of the page.

To create a footnote reference, add a caret and an identifier inside brackets ([\^1]). Identifiers can be numbers or words, but they can’t contain spaces or tabs. Identifiers only correlate the footnote reference with the footnote itself — in the output, footnotes are numbered sequentially.

Add the footnote using another caret and number inside brackets with a colon and text ([\^1]: My footnote.). You don’t have to put footnotes at the end of the document. You can put them anywhere except inside other elements like lists, block quotes, and tables.

| **Markdown** | **HTML** | **Rendered Output** |
|:------------:|:--------:|:-------------------:|
| Here's a simple footnote,[\^1] | | Here's a simple footnote.[^1] |
| here's a longer one.[\^bignote] | | here's a longer one.[^bignote] |

[:arrow\_backward: Back to Table of Contents](Markdown_Language_Guide)

[^1]: This is the first footnote.
[^bignote]: Here's one with multiple paragraphs and code.<br>
    Indent paragraphs to include them in the footnote.<br>
    `{ my code }`<br>
    Add as many paragraphs as you like.