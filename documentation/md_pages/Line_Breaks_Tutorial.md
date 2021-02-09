[:arrow\_backward: Paragraphs](Paragraphs_Tutorial) | [Home](home) | [Markdown Language Guide](Markdown_Language_Guide) | [Emphasis :arrow\_forward:](Emphasis_Tutorial)

## Line Breaks

To create a line break (`<br>`), end a line with two or more spaces, and then type return.

| **Markdown** | **HTML** | **Rendered Output** |
|:------------:|:--------:|:-------------------:|
| The first line··The second line·· | \<p>The first line\<br>The second line\<br>\</p> | The first line<br>The second line<br> |
| The first line\<br>The second line\<br> | \<p>The first line\<br>The second line\<br>\</p> | The first line<br>The second line<br> |

> **NOTE:** The character `·` represents a space.

## HTML vs. Markdown

By entering 2 spaces after a line, will generate a ```<br>``` in markdown, when there is are any ascii character under the line above.

#### For example

```markdown
This is the first line of text··
This is the second line of text
```

#### Will render

This is the first line of text  
This is the second line of text

#### Caveats

When inside a table, the spaces will not generate a new line. A HTML `<br>` will be required to generate a new line. This will generate a style lint error **MD033** - *(Inline HTML)*, this is an unavoidable style config.

[:arrow\_backward: Back to Table of Contents](Markdown_Language_Guide)