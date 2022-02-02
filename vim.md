# Vim cheatsheet

[Vim](https://www.vim.org) is a powerful text editor. It is an improved version of the _Vi_ editor and it is included as _vi_ with most UNIX systems and Apple OSX.

Type `vimtutor` in the terminal <img src="./images/terminal.png" alt="terminal" style="width:18px;"/> for a full tutorial or `:help [heltp.txt]` and `:help [key-notation]` inside _Vim_ for official documentation. You can also check this [FAQ](https://vimhelp.org/vim_faq.txt.html) for further help.

[Neovim](https://neovim.io/) is a _Vim-based_ text editor if you want the good parts of _Vim_ and more.

## Table of contents

- [Vim cheatsheet](#vim-cheatsheet)
  - [Table of contents](#table-of-contents)
    - [Essentials](#essentials)
      - [Cursor movement (Normal/Visual Mode)](#cursor-movement-normalvisual-mode)
      - [Editing text](#editing-text)
      - [Operators (Normal/Visual Mode)](#operators-normalvisual-mode)
      - [Marking text (visual mode)](#marking-text-visual-mode)
      - [Clipboard](#clipboard)
      - [Exiting](#exiting)
      - [Search/Replace](#searchreplace)
      - [General](#general)
    - [Advanced](#advanced)
      - [Cursor movement](#cursor-movement)
      - [Character search](#character-search)
      - [Editing text](#editing-text-1)
      - [Visual mode](#visual-mode)
      - [File Tabs](#file-tabs)
      - [Marks](#marks)
      - [Text Objects](#text-objects)
      - [General](#general-1)
    - [References](#references)

### Essentials

#### Cursor movement (Normal/Visual Mode)

| Command         | Description                          |
| :-------------- | :----------------------------------- |
| `h` `j` `k` `l` | Arrow keys                           |
| `w` / `b`       | Next/previous word                   |
| `W` / `B`       | Next/previous word (space seperated) |
| `e` / `ge`      | Next/previous end of word            |
| `0` / `$`       | Start/End of line                    |
| `^`             | First non-blank character of line    |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Editing text

| Command           | Description                                        |
| :---------------- | :------------------------------------------------- |
| `i` / `a`         | Start insert mode at/after cursor                  |
| `I` / `A`         | Start insert mode at the beginning/end of the line |
| `o` / `O`         | Add blank line below/above current line            |
| `Esc` or `Ctrl+[` | Exit insert mode                                   |
| `d`               | Delete                                             |
| `dd`              | Delete line                                        |
| `c`               | Delete, then start insert mode                     |
| `cc`              | Delete line, then start insert mode                |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Operators (Normal/Visual Mode)

You can combine operators with motions. Ex: `d0` deletes from the cursor to the start of the line. See `:help operator` and `:help motion.txt`

| Command | Description                                                               |
| :------ | :------------------------------------------------------------------------ |
| `d`     | Deletes from the cursor to the movement location                          |
| `c`     | Deletes from the cursor to the movement location, then starts insert mode |
| `y`     | Copy from the cursor to the movement location                             |
| `>`     | Indent one level                                                          |
| `<`     | Unindent one level                                                        |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Marking text (visual mode)

| Command           | Description                |
| :---------------- | :------------------------- |
| `v`               | Start visual mode          |
| `V`               | Start linewise visual mode |
| `Ctrl+v`          | Start visual block mode    |
| `Esc` or `Ctrl+[` | Exit visual mode           |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Clipboard

| Command   | Description                     |
| :-------- | :------------------------------ |
| `yy`      | Yank (copy) a line              |
| `p`       | Paste after cursor              |
| `P`       | Paste before cursor             |
| `dd`      | Delete (cut) a line             |
| `x`       | Delete (cut) current character  |
| `X`       | Delete (cut) previous character |
| `d` / `c` | Copy the deleted text           |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Exiting

| Command | Description                           |
| :------ | :------------------------------------ |
| `:w`    | Write (save) the file, but don't quit |
| `:wq`   | Write (save) and quit                 |
| `:q`    | Quit (fails if anything has changed)  |
| `:q!`   | Quit and throw away changes           |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Search/Replace

| Command          | Description                                                 |
| :--------------- | :---------------------------------------------------------- |
| `/pattern`       | Search for pattern                                          |
| `?pattern`       | Search backward for pattern                                 |
| `n`              | Repeat search in same direction                             |
| `N`              | Repeat search in opposite direction                         |
| `:%s/old/new/g`  | Replace all old with new throughout file                    |
| `:%s/old/new/gc` | Replace all old with new throughout file with confirmations |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### General

| Command  | Description |
| :------- | :---------- |
| `u`      | Undo        |
| `Ctrl+r` | Redo        |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### Advanced

#### Cursor movement

| Command           | Description                                    |
| :---------------- | :--------------------------------------------- |
| `Ctrl+d`          | Move down half a page                          |
| `Ctrl+u`          | Move up half a page                            |
| `}`               | Go forward by paragraph (the next blank line)  |
| `{`               | Go backward by paragraph (the next blank line) |
| `gg`              | Go to the top of the page                      |
| `G`               | Go the bottom of the page                      |
| `: [num] [enter]` | Go to that line in the document                |
| `ctrl+e / ctrl+y` | Scroll down/up one line                        |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Character search

| Command    | Description                            |
| :--------- | :------------------------------------- |
| `f [char]` | Move forward to the given char         |
| `F [char]` | Move backward to the given char        |
| `t [char]` | Move forward to before the given char  |
| `T [char]` | Move backward to before the given char |
| `;` / `,`  | Repeat search forwards/backwards       |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Editing text

| Command    | Description                                                                   |
| :--------- | :---------------------------------------------------------------------------- |
| `J`        | Join line below to the current one                                            |
| `r [char]` | Replace a single character with the specified char (does not use Insert mode) |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Visual mode

| Command | Description                      |
| :------ | :------------------------------- |
| `O`     | Move to other corner of block    |
| `o`     | Move to other end of marked area |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### File Tabs

| Command       | Description                |
| :------------ | :------------------------- |
| `:e filename` | Edit a file                |
| `:tabe`       | Make a new tab             |
| `gt`          | Go to the next tab         |
| `gT`          | Go to the previous tab     |
| `:vsp`        | Vertically split windows   |
| `ctrl+ws`     | Split windows horizontally |
| `ctrl+wv`     | Split windows vertically   |
| `ctrl+ww`     | Switch between windows     |
| `ctrl+wq`     | Quit a window              |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Marks

Marks allow you to jump to designated points in your code. A capital mark {A-Z} sets a global mark and will work between files

| Command  | Description                                                     |
| :------- | :-------------------------------------------------------------- |
| `m{a-z}` | Set mark {a-z} at cursor position                               |
| `'{a-z}` | Move the cursor to the start of the line where the mark was set |
| `''`     | Go back to the previous jump location                           |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

#### Text Objects

Say you have `def (arg1, arg2, arg3)`, where your cursor is somewhere in the middle of the parenthesis.

| Command | Description                                                                                     |
| :------ | :---------------------------------------------------------------------------------------------- |
| `di(`   | Deletes everything between the parenthesis. Without text objects, you would need to do `T(dt)`. |

#### General

| Command      | Description                                                      |
| :----------- | :--------------------------------------------------------------- |
| `.`          | Repeat last command                                              |
| `Ctrl+r + 0` | in insert mode inserts the last yanked text (or in command mode) |
| `gv`         | reselect (select last selected block of text, from visual mode)  |
| `%`          | jumps between matching `()` or `{}`                              |

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>

### References

- [Vim - the ubiquitous text editor](https://www.vim.org)
- [Wikipedia - Vim (text editor)](<https://en.wikipedia.org/wiki/Vim_(text_editor)>)
- [Vim help files](https://vimhelp.org)
- [Vim cheatsheet](https://devhints.io/vim)
- [Vim Cheat Sheet](https://vim.rtorr.com)
- [A Great Vim Cheat Sheet](https://vimsheet.com)

<div align="right">
  <a href="#table-of-contents">↥ Back To Top</a>
</div>
