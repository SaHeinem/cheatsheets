# VIM Cheatsheet
this document is intended as reference for some Vim commands. The author does not claim completeness

## Table of contents
* [Commands](#commands)
* [Modes](#modes)
* [Help, Write and Exit Vim](#help-write-and-exit-vim)
* [Cursor movement](#cursor-movement)
* [Edit](#edit)

## Commands
Make sure you're not in edit mode by hitting the `ESC` key:
|Command|Effect|
|---|---|
|/|search for everything after `/`, `n` /`N` for next / previous|
|:syntax on|self explanatory|
|:set nu / :set nonu!|show line number|
|:set rnu / :set nornu|show relative line numbers|
|:set nu!|toggle relative line numbers|

## Modes
Leave any mode by hitting the `ESC` key:
|Key|Mode|
|---|---|
|i|Insert mode|
|I|insert at beggining of line|
|a|insert (append) after cursor|
|A|insert (append) at end of line|
|v|visual mode|

## Help, Write and Exit Vim
Make sure you're not in edit mode by hitting the `ESC` key:

|Command|Effect|
|---|---|
|:q|quit|
|:q!|quit and throw unsaved changes|
|:h|help|
|:w|write|
|:wq|write and quit|

## Cursor movement
|Key(s)|Effect|
|--|--|
|h|←|
|j|↓|
|k|↑|
|l|→|
|gj|move cursor down multiple lines|
|gk|move cursor up multiple lines|
|H|move to top of screen|
|M|move to middle of screen|
|L|move to bottom of screen|
|w|jump to start of word|
|W|like w but with punctuation|
|e|jump to end of word|
|E|like e but with punctuation|
|b|jump back to start of word|
|B|like b but with punctuation|
|ge|jump back to end of word|
|gE|like ge but with punctuation|
|0|jump tp start of line|
|$|jump to end of line|
|gg|go to first line of the document|
|G|go to last line of the document|
|5gg / 5G|got to line 5|

## Edit
|Key(s)|Effect|
|---|---|
|r|replace one char|
|R|replace until `ESC` is pressed|
|u|undo|
|U|restore (undo) last changed line|
|Ctrl + r|redo|

### Mark in visual mode
|Key(s)|Effect|
|---|---|
|v|starts visual mode and starts selecting current cursor|
|V|line wise visual mode|
|o|move to other end of marked area|
|Ctrl + v|visual block mode|
|O|move to other corner of block|
|aw|mark word|

### Cut and paste
|Key(s)|Effect|
|---|---|
|yy|copy line|
|2yy|copy 2 lines|
|y$ / Y|copy to end of line|
|P|paste after cursor|
|p|paste before cursor|
|dd|delete (cut) line|
|2dd|delete (cut) 2 lines|
|dw|delete word|
|:3,5d|delete line 3 to 5|
