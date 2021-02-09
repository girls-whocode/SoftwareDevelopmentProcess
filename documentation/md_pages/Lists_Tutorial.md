[:arrow\_backward: Syntax Highlighted Code](Syntax_Highlighted_Code_Tutorial) | [Home](home) | [Markdown Language Guide](Markdown_Language_Guide) | [Footnotes :arrow\_forward:](Footnotes_Tutorial)

## Lists
You can organize items into ordered and unordered lists.

### Ordered Lists
To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but the list should start with the number one.

| **Markdown** | **HTML** | **Rendered Output** |
|:-------------|:---------|:--------------------|
| 1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item | \<ol><br>\<li>First Item\</li><br>\<li>Second Item\</li><br>\<li>Third Item\</li><br>\<li>Fourth Item\</li><br>\</ol> | <ol><li>First Item</li><li>Second Item</li><li>Third Item</li><li>Fourth Item</li></ol> |
| 1. First item<br>1. Second item<br>1. Third item<br>1. Fourth item | \<ol><br>\<li>First Item\</li><br>\<li>Second Item\</li><br>\<li>Third Item\</li><br>\<li>Fourth Item\</li><br>\</ol> | <ol><li>First Item</li><li>Second Item</li><li>Third Item</li><li>Fourth Item</li></ol> |
| 1. First item<br>8. Second item<br>5. Third item<br>2. Fourth item | \<ol><br>\<li>First Item\</li><br>\<li>Second Item\</li><br>\<li>Third Item\</li><br>\<li>Fourth Item\</li><br>\</ol> | <ol><li>First Item</li><li>Second Item</li><li>Third Item</li><li>Fourth Item</li></ol> |

### Unordered Lists
To create an unordered list, add dashes (-), asterisks (*), or plus signs (+) in front of line items. Indent one or more items to create a nested list.

| **Markdown** | **HTML** | **Rendered Output** |
|:-------------|:---------|:--------------------|
| - First item<br>- Second item<br>- Third item<br>- Fourth item | \<ul><br>\<li>First Item\</li><br>\<li>Second Item\</li><br>\<li>Third Item\</li><br>\<li>Fourth Item\</li><br>\</ul> | <ul><li>First Item</li><li>Second Item</li><li>Third Item</li><li>Fourth Item</li></ul> |
| * First item<br>* Second item<br>* Third item<br>* Fourth item | \<ul><br>\<li>First Item\</li><br>\<li>Second Item\</li><br>\<li>Third Item\</li><br>\<li>Fourth Item\</li><br>\</ul> | <ul><li>First Item</li><li>Second Item</li><li>Third Item</li><li>Fourth Item</li></ul> |
| + First item<br>- Second item<br>* Third item<br>+ Fourth item | \<ul><br>\<li>First Item\</li><br>\<li>Second Item\</li><br>\<li>Third Item\</li><br>\<li>Fourth Item\</li><br>\</ul> | <ul><li>First Item</li><li>Second Item</li><li>Third Item</li><li>Fourth Item</li></ul> |

## Task Lists
Task lists allow you to create a list of items with checkboxes. In Markdown applications that support task lists, checkboxes will be displayed next to the content. To create a task list, add dashes (-) and brackets with a space (`[ ]`) in front of task list items. To select a checkbox, add an x in between the brackets (`[x]`).

```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

The rendered output looks like this:
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

[:arrow\_backward: Back to Table of Contents](Markdown_Language_Guide)