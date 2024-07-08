# Markdown

## What is Markdown?

**Markdown** is a lightweight markup language that you can use to add formatting
elements to plaintext text documents. Created by John Gruber in 2004, Markdown
allows you to format text easily without using complex HTML tags.

## Basic Syntax

### Headings

To create a heading, add a hash (`#`) symbol in front of a word or phrase.
Markdown supports six levels of headings, corresponding to `<h1>` to `<h6>` in
HTML.

```markdown
# Heading level 1

## Heading level 2

### Heading level 3

#### Heading level 4

##### Heading level 5

###### Heading level 6
```

### Paragraphs

Simply write your text on separate lines to create paragraphs.

```markdown
I really like using Markdown.

I think I'll use it to format all of my documents from now on.
```

### Line Breaks

To create a line break, end a line with two or more spaces and press `Enter`.

```markdown
This is the first line.  
And this is the second line.
```

### Bold Text

To make text bold, wrap it with two asterisks (`**`) or underscores (`__`).

```markdown
I just love **bold text**. I just love **bold text**.
```

### Italic Text

To italicize text, wrap it with one asterisk (`*`) or underscore (`_`).

```markdown
I just love _italic text_. I just love _italic text_.
```

### Bold and Italic Text

To make text bold and italic, wrap it with three asterisks (`***`) or
underscores (`___`).

```markdown
I just love **_bold and italic text_**. I just love **_bold and italic text_**.
```

### Blockquotes

To create a blockquote, add a `>` in front of a paragraph.

```markdown
> Dorothy followed her through many of the beautiful rooms in her castle.
```

### Ordered Lists

To create an ordered list, preface each item with a number followed by a period.

```markdown
1. First item
2. Second item
3. Third item
4. Fourth item
```

### Unordered Lists

To create an unordered list, preface each item with a dash (`-`), asterisk
(`*`), or plus sign (`+`).

```markdown
- First item
- Second item
- Third item
- Fourth item
```

### Code Blocks

To create a code block, indent each line of the block by at least four spaces or
one tab. Alternatively, you can use triple backticks (```) before and after the
code block.

```html
<html>
  <head>
    <title>Test</title>
  </head>
  <body>
    <h1>This is a heading</h1>
  </body>
</html>
```

### Inline Code

To denote a word or phrase as code, wrap it with backticks (`` ` ``).

```markdown
Use the `printf()` function.
```

### Images

To add an image, use the following syntax: `![alt text](image URL)`.

```markdown
![Markdown Logo](../assets/markdown.png)
```

### Horizontal Rules

To create a horizontal rule, use three or more dashes (`---`), asterisks
(`***`), or underscores (`___`) on a line by themselves.

```markdown
---
```

### Links

To create a link, enclose the link text in brackets (`[]`) and then enclose the
URL in parentheses (`()`).

```markdown
[GitHub](https://github.com/)
```

### Tables

To create a table, use pipes (`|`) to separate columns and hyphens (`-`) to
create the header row.

```markdown
| Syntax    | Description | Test Text     |
| --------- | ----------- | ------------- |
| Header    | Title       | Here's this   |
| Paragraph | Text        | And more text |
```

### Combined Example

Here’s an example that combines many of these elements:

````markdown
# My Project

Welcome to my project. Below is a list of features:

## Features

1. **Easy to Use**
   - Simple and intuitive
2. _Fast_
   - Optimized for performance

## Code Example

```html
<html>
  <head>
    <title>Sample Code</title>
  </head>
  <body>
    <p>This is a sample code block.</p>
  </body>
</html>
```
````

## Additional Information

For more details, visit the [documentation](https://www.markdownguide.org/).

![Sample Image](../assets/linux.png)
