# Markdown cheatsheet

[Markdown](https://en.wikipedia.org/wiki/Markdown) is a lightweight markup language for creating formatted text using a plain-text editor.

## Table of contents

- [Markdown cheatsheet](#markdown-cheatsheet)
  - [Table of contents](#table-of-contents)
    - [Headings](#headings)
    - [Paragraphs](#paragraphs)
    - [Line Breaks](#line-breaks)
    - [Emphasis](#emphasis)
      - [Bold](#bold)
      - [Italic](#italic)
      - [Bold and Italic](#bold-and-italic)
    - [Blockquotes](#blockquotes)
      - [Blockquotes with Multiple Paragraphs](#blockquotes-with-multiple-paragraphs)
      - [Nested Blockquotes](#nested-blockquotes)
      - [Blockquotes with Other Elements](#blockquotes-with-other-elements)
    - [Lists](#lists)
      - [Ordered Lists](#ordered-lists)
      - [Unordered Lists](#unordered-lists)
    - [Code](#code)
      - [Code Blocks](#code-blocks)
    - [Horizontal Rules](#horizontal-rules)
    - [Links](#links)
    - [Images](#images)
      - [Linking Images](#linking-images)
    - [References](#references)

### Headings

| Markdown          | Rendered Output          |
| :---------------- | :----------------------- |
| # Heading level 1 | <h1>Heading level 1</h1> |
| # Heading level 2 | <h2>Heading level 2</h2> |
| # Heading level 3 | <h3>Heading level 3</h3> |
| # Heading level 4 | <h4>Heading level 4</h4> |
| # Heading level 5 | <h5>Heading level 5</h5> |
| # Heading level 6 | <h6>Heading level 6</h6> |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text.

| Markdown                                         | Rendered Output                                  |
| :----------------------------------------------- | :----------------------------------------------- |
| Don't add tabs or spaces in front of paragraphs. | Don't add tabs or spaces in front of paragraphs. |
| Keep lines left-aligned like this.               | Keep lines left-aligned like this.               |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Line Breaks

To create a line break or new line `<br>`, end a line with two or more spaces, and then type return.

| Markdown                                                | Rendered Output                                         |
| :------------------------------------------------------ | :------------------------------------------------------ |
| This is the first line.<br>And this is the second line. | This is the first line.<br>And this is the second line. |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Emphasis

#### Bold

| Markdown                  | Rendered Output       |
| :------------------------ | :-------------------- |
| I am a \*\*bold text\*\*. | I am a **bold text**. |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Italic

| Markdown                | Rendered Output       |
| :---------------------- | :-------------------- |
| I am a \_italic text\_. | I am a _italic text_. |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Bold and Italic

| Markdown                                 | Rendered Output                    |
| :--------------------------------------- | :--------------------------------- |
| I am a \*\*\_bold and italic text\_\*\*. | I am a **_bold and italic text_**. |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Blockquotes

    > To create a blockquote, add a > in front of a paragraph.

Rendered output:

> To create a blockquote, add a > in front of a paragraph.

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Blockquotes with Multiple Paragraphs

    > Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs.
    >
    > Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs.

Rendered output:

> Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs.
>
> Blockquotes can contain multiple paragraphs. Add a > on the blank lines between the paragraphs.

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Nested Blockquotes

    > Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.
    >
    >> Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.

Rendered output:

> Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.
>
> > Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Blockquotes with Other Elements

    > #### Blockquotes can contain other Markdown formatted elements.
    >
    > - Not all elements can be used
    > - Not all elements can be used
    >
    >_you’ll_ need to experiment to see **which ones work**.

Rendered output:

> ##### Blockquotes can contain other Markdown formatted elements.
>
> - Not all elements can be used
> - Not all elements can be used
>
> _you’ll_ need to experiment to see **which ones work**.

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Lists

#### Ordered Lists

| Markdown                                                           | Rendered Output                                                    |
| :----------------------------------------------------------------- | :----------------------------------------------------------------- |
| 1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item | 1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Unordered Lists

| Markdown                                                                                                                                             | Rendered Output                                                                                                                              |
| :--------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------- |
| - First item<br>- Second item<br>- Third item<br>- Fourth item                                                                                       | <ul><li>First item</li><li>Second item</li><li>Third item</li><li>Fourth item</li></ul>                                                      |
| - First item<br>- Second item<br>- Third item<br>&nbsp;&nbsp;&nbsp;&nbsp;- Indented item<br>&nbsp;&nbsp;&nbsp;&nbsp;- Indented item<br>- Fourth item | <ul><li>First item</li><li>Second item</li><li>Third item<ul><li>Indented item</li><li>Indented item</li></ul></li><li>Fourth item</li></ul> |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Code

| Markdown                                    | Rendered Output                         |
| :------------------------------------------ | :-------------------------------------- |
| At the command prompt, type \`nano\`.       | At the command prompt, type `nano`.     |
| \`\`Use \`code\` in your Markdown file.\`\` | `` Use `code` in your Markdown file. `` |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Code Blocks

To create code blocks, indent every line of the block by at least four spaces or one tab.

```
    <html>
      <head>
      </head>
    </html>
```

Rendered output:

    <html>
      <head>
      </head>
    </html>

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Horizontal Rules

```
***

---

_________________
```

Rendered output:

---

---

---

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Links

| Markdown                                                            | Rendered Output                                                    |
| :------------------------------------------------------------------ | :----------------------------------------------------------------- |
| \[Cheatsheets Vault](https://github.com/dreibona/cheatsheets-vault) | [Cheatsheets Vault](https://github.com/dreibona/cheatsheets-vault) |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Images

| Markdown                             | Rendered Output                    |
| :----------------------------------- | :--------------------------------- |
| \!\[Terminal](./images/terminal.png) | ![Terminal](./images/terminal.png) |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Linking Images

| Markdown                                                                        | Rendered Output                                                              |
| :------------------------------------------------------------------------------ | :--------------------------------------------------------------------------- |
| \[\!\[An old rock in the desert](./images/terminal.png)](./images/terminal.png) | [![An old rock in the desert](./images/terminal.png)](./images/terminal.png) |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### References

- [Daring Fireball](https://daringfireball.net/projects/markdown/)
- [Markdown - Wikipedia](https://en.wikipedia.org/wiki/Markdown)
- [GitHub Docs](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Markdown Guide](https://www.markdownguide.org)

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>
