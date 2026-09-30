# VI Text Editor

VI is commonly used in Linux environments, so it is useful to know the basic commands.

VI is a text editor, similar to Notepad, Emacs, and VS Code.

### To launch the VI text editor

>> **vi** or **vi [filename]**: opens an existing text file or creates a new file in VI.

### In VI

>> **i**: enters Insert mode.

>> **Esc**: returns to Command mode.

### In Command mode

>> `:w [filename]`: saves the file.

If the file is new, a filename can be specified.

>> `:q`: quits VI.

>> `[command]!`: forces the command.

Example: `:q!`

>> `/[target string]`: searches for and highlights a target string.

Controls:

`n`: moves to the next matching result.

`Shift + N`: moves to the previous matching result.

>> `:[line number]`: moves to a specific line.

>> `[optional number]dd`: deletes one or more lines.

Example: `3dd` deletes three lines.

>> `:set shell=[path of the shell]`: configures the shell used by VI.

>> `:sh`: opens the configured shell from VI.

### In the `more` reader

>> `v`: opens the current file in VI.