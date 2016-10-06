# TODO file syntax

[Sublime Text 3][st3] syntax definition and color scheme for plain text files containing lists of tasks that need to be done (i.e. ToDos) and pro/con lists. The Sublime Text color scheme is based on [FreshCut by Dayle Rees][freshcut].

![Sublime Text 3 screenshot](screenshots/sublime.png)

### Syntax

Start a block using `NAME:`, optionally followed by a title, as its first line. Finally, you can end the block using `:NAME` as the last line.

Within the block you can add items that start with a character (see below for list) followed by a whitespace.

#### TODO Block

- `!`: Task is open and important
- `-`: Task is open
- `?`: Task is uncertain, optional or a suggestion
- `o`: Task is in progress
- `/`: Task is blocked and cannot be worked on right now
- `x`: Task is done
- `#`: Task cannot be worked on (i.e. it's already done, handled by someone else or impossible to get done)

#### COMP Block

- `+`: Argument is positive
- `o`: Argument is neutral
- `-`: Argument is negative

## Installation

### Use prebuilt files

- Sublime Text
    - Copy all files in `sublime` directory into Sublime Text's `Packages/User` directory.

### Build it yourself

1. Install [syntax tools][syntax-tools]
2. Create and deploy files
    - Sublime Text: `<path-to-syntax-tools>/build todo src/sublime`

[freshcut]: https://github.com/daylerees/colour-schemes/blob/master/legacy/Contrast/FreshCut.tmTheme
[st3]: http://www.sublimetext.com/
[syntax-tools]: https://github.com/ThomasGreiner/syntax-tools
