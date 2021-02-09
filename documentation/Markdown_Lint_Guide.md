# markdownlint

A style checker and lint documentation for Markdown/CommonMark files.

## Overview

The [Markdown](https://en.wikipedia.org/wiki/Markdown) markup language is
designed to be easy to read, write, and understand. It succeeds - and its
flexibility is both a benefit and a drawback. Many styles are possible, so
formatting can be inconsistent. Some constructs don't work well in all
parsers and should be avoided. The [CommonMark](https://commonmark.org/)
specification standardizes parsers - but not authors.

`markdownlint` is a [static analysis](https://en.wikipedia.org/wiki/Static_program_analysis)
documentation with a library of rules to enforce standards and consistency for Markdown files.
It was inspired by - and heavily influenced by - Mark Harrison's
[markdownlint](https://github.com/markdownlint/markdownlint) for
[Ruby](https://www.ruby-lang.org/). The initial rules, rule documentation, and
test cases came directly from that project.

### Related

* [markdownlint-cli command-line interface for Node.js](https://github.com/igorshubovych/markdownlint-cli)
* [grunt-markdownlint for the Grunt task runner](https://github.com/sagiegurari/grunt-markdownlint)
* [vscode-markdownlint extension for VS Code](https://marketplace.visualstudio.com/items/DavidAnson.vscode-markdownlint)
* [Sublime Text markdownlint for Sublime Text](https://packagecontrol.io/packages/SublimeLinter-contrib-markdownlint)
* [linter-node-markdownlint extension for Atom](https://atom.io/packages/linter-node-markdownlint)
* [markdownlint/mdl gem for Ruby](https://rubygems.org/gems/mdl)

## Demonstration

[`markdownlint` demo](https://dlaa.me/markdownlint/), an interactive, in-browser
playground for learning and exploring.

## Rules / Aliases

* **[MD001](md_pages/rules/Rules.md#md001)** *(heading-increment/header-increment)* - Heading levels should only increment by one level at a time
* **[MD002](md_pages/rules/Rules.md#md002)** *(first-heading-h1/first-header-h1)* - First heading should be a top level heading
* **[MD003](md_pages/rules/Rules.md#md003)** *(heading-style/header-style)* - Heading style
* **[MD004](md_pages/rules/Rules.md#md004)** *(ul-style)* - Unordered list style
* **[MD005](md_pages/rules/Rules.md#md005)** *(list-indent)* - Inconsistent indentation for list items at the same level
* **[MD006](md_pages/rules/Rules.md#md006)** *(ul-start-left)* - Consider starting bulleted lists at the beginning of the line
* **[MD007](md_pages/rules/Rules.md#md007)** *(ul-indent)* - Unordered list indentation
* **[MD009](md_pages/rules/Rules.md#md009)** *(no-trailing-spaces)* - Trailing spaces
* **[MD010](md_pages/rules/Rules.md#md010)** *(no-hard-tabs)* - Hard tabs
* **[MD011](md_pages/rules/Rules.md#md011)** *(no-reversed-links)* - Reversed link syntax
* **[MD012](md_pages/rules/Rules.md#md012)** *(no-multiple-blanks)* - Multiple consecutive blank lines
* **[MD013](md_pages/rules/Rules.md#md013)** *(line-length)* - Line length
* **[MD014](md_pages/rules/Rules.md#md014)** *(commands-show-output)* - Dollar signs used before commands without showing output
* **[MD018](md_pages/rules/Rules.md#md018)** *(no-missing-space-atx)* - No space after hash on atx style heading
* **[MD019](md_pages/rules/Rules.md#md019)** *(no-multiple-space-atx)* - Multiple spaces after hash on atx style heading
* **[MD020](md_pages/rules/Rules.md#md020)** *(no-missing-space-closed-atx)* - No space inside hashes on closed atx style heading
* **[MD021](md_pages/rules/Rules.md#md021)** *(no-multiple-space-closed-atx)* - Multiple spaces inside hashes on closed atx style heading
* **[MD022](md_pages/rules/Rules.md#md022)** *(blanks-around-headings/blanks-around-headers)* - Headings should be surrounded by blank lines
* **[MD023](md_pages/rules/Rules.md#md023)** *(heading-start-left/header-start-left)* - Headings must start at the beginning of the line
* **[MD024](md_pages/rules/Rules.md#md024)** *(no-duplicate-heading/no-duplicate-header)* - Multiple headings with the same content
* **[MD025](md_pages/rules/Rules.md#md025)** *(single-title/single-h1)* - Multiple top level headings in the same document
* **[MD026](md_pages/rules/Rules.md#md026)** *(no-trailing-punctuation)* - Trailing punctuation in heading
* **[MD027](md_pages/rules/Rules.md#md027)** *(no-multiple-space-blockquote)* - Multiple spaces after blockquote symbol
* **[MD028](md_pages/rules/Rules.md#md028)** *(no-blanks-blockquote)* - Blank line inside blockquote
* **[MD029](md_pages/rules/Rules.md#md029)** *(ol-prefix)* - Ordered list item prefix
* **[MD030](md_pages/rules/Rules.md#md030)** *(list-marker-space)* - Spaces after list markers
* **[MD031](md_pages/rules/Rules.md#md031)** *(blanks-around-fences)* - Fenced code blocks should be surrounded by blank lines
* **[MD032](md_pages/rules/Rules.md#md032)** *(blanks-around-lists)* - Lists should be surrounded by blank lines
* **[MD033](md_pages/rules/Rules.md#md033)** *(no-inline-html)* - Inline HTML
* **[MD034](md_pages/rules/Rules.md#md034)** *(no-bare-urls)* - Bare URL used
* **[MD035](md_pages/rules/Rules.md#md035)** *(hr-style)* - Horizontal rule style
* **[MD036](md_pages/rules/Rules.md#md036)** *(no-emphasis-as-heading/no-emphasis-as-header)* - Emphasis used instead of a heading
* **[MD037](md_pages/rules/Rules.md#md037)** *(no-space-in-emphasis)* - Spaces inside emphasis markers
* **[MD038](md_pages/rules/Rules.md#md038)** *(no-space-in-code)* - Spaces inside code span elements
* **[MD039](md_pages/rules/Rules.md#md039)** *(no-space-in-links)* - Spaces inside link text
* **[MD040](md_pages/rules/Rules.md#md040)** *(fenced-code-language)* - Fenced code blocks should have a language specified
* **[MD041](md_pages/rules/Rules.md#md041)** *(first-line-heading/first-line-h1)* - First line in file should be a top level heading
* **[MD042](md_pages/rules/Rules.md#md042)** *(no-empty-links)* - No empty links
* **[MD043](md_pages/rules/Rules.md#md043)** *(required-headings/required-headers)* - Required heading structure
* **[MD044](md_pages/rules/Rules.md#md044)** *(proper-names)* - Proper names should have the correct capitalization
* **[MD045](md_pages/rules/Rules.md#md045)** *(no-alt-text)* - Images should have alternate text (alt text)

See [Rules.md](md_pages/rules/Rules.md) for more details.

> All rules with `heading` as part of their name are also available as `header`
> aliases (e.g. `heading-increment` is also available as `header-increment`).
> The use of `header` is deprecated and provided for backward-compatibility.

## Tags

Tags group related rules and can be used to enable/disable multiple rules at once.

* **accessibility** - MD045
* **atx** - MD018, MD019
* **atx_closed** - MD020, MD021
* **blank_lines** - MD012, MD022, MD031, MD032
* **blockquote** - MD027, MD028
* **bullet** - MD004, MD005, MD006, MD007, MD032
* **code** - MD014, MD031, MD038, MD040
* **emphasis** - MD036, MD037
* **hard_tab** - MD010
* **headers** - MD001, MD002, MD003, MD018, MD019, MD020, MD021, MD022, MD023,
  MD024, MD025, MD026, MD036, MD041, MD043
* **headings** - MD001, MD002, MD003, MD018, MD019, MD020, MD021, MD022, MD023,
  MD024, MD025, MD026, MD036, MD041, MD043
* **hr** - MD035
* **html** - MD033
* **images** - MD045
* **indentation** - MD005, MD006, MD007, MD027
* **language** - MD040
* **line_length** - MD013
* **links** - MD011, MD034, MD039, MD042
* **ol** - MD029, MD030, MD032
* **spaces** - MD018, MD019, MD020, MD021, MD023
* **spelling** - MD044
* **ul** - MD004, MD005, MD006, MD007, MD030, MD032
* **url** - MD034
* **whitespace** - MD009, MD010, MD012, MD027, MD028, MD030, MD037, MD038, MD039