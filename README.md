# Learn How to Vim inside Visual Studio Code

## Motivation
>I want to learn how to use vim<br>
>I want to learn how to use vim in VS Code

## Getting Started

- Download and install [Visual Code Studio](https://code.visualstudio.com/)
- Download and install the [VsCodeVim
  extension](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
  - You will most likely want to enable key-repeating. To enable key-repeating,
    execute the following in your Terminal if you are using a Mac machine:
    ```
    $ defaults write com.microsoft.VSCode ApplePressAndHoldEnabled -bool false              # For VS Code
    $ defaults write com.microsoft.VSCodeInsiders ApplePressAndHoldEnabled -bool false      # For VS Code Insider
    $ defaults write com.visualstudio.code.oss ApplePressAndHoldEnabled -bool false         # For VS Codium
    $ defaults write com.microsoft.VSCodeExploration ApplePressAndHoldEnabled -bool false   # For VS Codium Exploration users
    $ defaults delete -g ApplePressAndHoldEnabled      
    ```

## Vim Cheat Sheet

| key        | description                                                                     | notes                                            |
| ---------- | ------------------------------------------------------------------------------- | ------------------------------------------------ |
| j          | move cursor one space to the left                                               |                                                  |
| j          | move cursor one space down                                                      |                                                  |
| k          | move cursor one space up                                                        |                                                  |
| l          | move cursor one space to the right                                              |                                                  |
| i          | go into insert mode                                                             |                                                  |
| `<CTRL-C>` | go back to normal mode                                                          |                                                  |
| `<esc>`    | go back to normal mode                                                          |                                                  |
| w          | jump from word to word                                                          | includes letters, digits and numbers             |
| W          | jump from word to word                                                          | includes special chars (`.`, `(`, `{`, etc)      |
| b          | jump from word to word backwards                                                | includes letters, digits, and numbers            |
| B          | jump from word to word backwards                                                | includes special chars (`.`, `(`, `{`, etc)      |
| e          | jump to the end of a word                                                       | includes letters, digits, and numbers            |
| E          | jump to the end of a word                                                       | includes special chars (`.`, `(`, `{`, etc)      |
| ge         | jump to the end of the word backwards                                           | includes letters, digits, and numbers            |
| f{char}    | move to the next occurrence of a character                                      | use `;` to go to next occurrence, `,` to go back |
| t{char}    | move the cursor before the next occurrence of a character                       | ^                                                |
| F{char}    | move to the next occurrence of a character backwards                            | ^                                                |
| T{char}    | move the cursor before the next occurrence of a character backwards             | ^                                                |
| 0          | moves to the first character of a line                                          |                                                  |
| ^          | moves to the first non-blank character of a line                                |                                                  |
| $          | moves to the end of a line                                                      |                                                  |
| g_         | moves to the non-blank character at the end of a line                           |                                                  |
| }          | jumps entire paragraphs downward                                                |                                                  |
| {          | jumps entire paragraphs upwards                                                 |                                                  |
| `<CTRL-D>` | move down half a page                                                           |                                                  |
| `<CTRL-U>` | moves up half a page                                                            |                                                  |
| ?{pattern} | locates match patterns and hitting `<Enter>` will jump to first match forward   | use `n` to jump to next match                    |
| ?{pattern} | locates match patterns and hitting `<Enter>` will jump to first match backwards | ^                                                |
| {n}w       | moves n words forward                                                           | e.g, 2w => 2 words forward                       |
| {n}b       | moves n words backwards                                                         | e.g, 2b => 2 words backwards                     |
| {n}e       | jumps n end of words forward                                                    |                                                  |
| {n}ge      | jumps n end of words backwards                                                  |                                                  |
| {n}j       | changes your cursor position to n lines below                                   |                                                  |
| {n};       | jumps to the nth occurrence of a character                                      |                                                  |
| {n}/{word} | jumps to the nth occurrence of the specified word                               |                                                  |
| gd         | jump to definition                                                              |                                                  |
| gf         | jump to a file in an import                                                     |                                                  |
| gg         | go to the top of a file                                                         |                                                  |
| G          | go to the end of the file                                                       |                                                  |
| {line}gg   | go to a specific line                                                           |                                                  |
| `:{line}`  | go to a specific line                                                           | e.g., `:44` + `<enter>`                          |
| %          | jump to the matching `({[]})`                                                   |                                                  |
| c          | deletes a piece of text and then goes into insert mode                          |                                                  |
| y          | yanks or copies selected text                                                   |                                                  |
| p          | pastes copied text                                                              |                                                  |
| g~         | changes selected letter(s) from uppercase to lowercase and vice versa           |                                                  |
| gUw        | capitalizes a word                                                              |                                                  |
| >          | adds indentation                                                                |                                                  |
| <          | removes indentation                                                             |                                                  |
| =          | formats code                                                                    |                                                  |
| c/{word}   | changes everything until the first occurrence of the word                       |                                                  |
| ggyG       | copies a whole document                                                         |                                                  |
