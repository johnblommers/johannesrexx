# Wordmark Notes

## Introduction

[Wordmark](https://wordmarkapp.com/) is in active development. A huge feature is single-pane live-preview editing much like Typora provides. It also looks really good and supports the Dark Mode theme. Plus it's cross-platform, as it's based on Electron.

This note is here because Wordmark supports publishing to GitHub Pages, making it easy to quickly put up a revised document or a new one.

## Features

- Themes
- Recognizes YAML
- macOS and Linux binaries.
- WYSIWYG so no dual panes
- Outline pane
- [Issues](https://github.com/wordmark/wordmark/issues) page at Github
- [Releases](https://github.com/wordmark/wordmark/releases) page at Github
- The 3.x series if free at least while it's in beta
- Grammar checking
- Detects updates and installs them.
- Each document gets its own window
- Easily opens `Revolution.md` our 50,000-word NaNoWriMo draft novel.

## Checklist
- [x] Item 1
- [ ] Item 2
  - [ ]  sub item
  - [ ]  another sub item
- [x] Item 3

## Math Support Lacking

$f(x)=a_0 + a_1 x +a_2 x^2$
$$f(x)=a_0 + a_1 x + a_2 x^2$$

f(x) = a~0~ + a~1~ x | a~2~ x^2^

## Tables Support is Experimental
| Heading 1 | heading 2 | heading 3 |
| --------- | --------- | --------- |
| aa        | 11        | a1        |
| bb        | 22        | b2        |
| cc        | 33        | c3        |
We created the table above by first using Typora to create a table and then copy-paste. But you cannot edit anything in the table.

The cell below was hand-entered but again, once entered the table is cast in stone. You can't even delete it.
|Head | Head|
|cell | cell|
## Links

[Go to](#Math Support) Math Support while recognized as a link[^FN] will not move the cursor to that heading.

[^FN]: Footnotes may be supported.

## Bugs and Omissions

We have [posted](https://github.com/wordmark/wordmark/issues) all of these points at Wordmark's github page.

- No export to any other file format
- **Tables**
-   Tables are an experimental feature but the current implementation imports the second row, the one that determines how the text in the column is justified, as data in a cell.
-   Tables once entered cannot be edited nor deleted.
- No LaTeX support so we can't enter math formulas.
- Superscripts and Subscripts are not supported in the Markdown.
- Please document exactly what features of Markdown you support.
- **TODO** Never finishes opening a 200,000-page text file.
- No Markdown menus or acceleration keyboard shortcuts. You have to type in Markdown text yourself. Not even Command+b will bold text.
- Does not recognize HTML characters such as &pi; 
- **TODO** **Outliner**
  - The outline does not recognize that H2 headings following H1 headings are subordinate. H2 headings should be rendered under a disclosure rectangle for the H1 headings, indented and in a little smaller font size. We have a document with 15 chapters and 110 scenes and it's hard to navigate using the outline.
  - When you click on a heading in the outline, the text does not scroll predictably. The heading should be scrolled to the top of the window.
  - - You cannot drag and drop in the outline so you cannot easily rearrange the sections in your text. This is not what an outliner is supposed to be. It's really a navigation tool.
- **TODO** When you click over text that is underlined in red - indicating a spelling mistake - you don't get a popup with suggested correct spellings.
- There is no documentation about what is contained in the "usage information." Please document in your privacy policy exactly what information Wordmark transmits.
- The Menu -> File -> Open Recent never lists any of the recent files.