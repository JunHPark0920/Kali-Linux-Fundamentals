# Pipe

A pipe connects the output of one process to the input of another process.

It is used to pass the standard output (stdout) of one process to the standard input (stdin) of another process.

#### Pipe Syntax

`[first command] | [second command]`

Example: `ls -l | grep ".txt"`

When a pipe is used, the standard output of the first command is not displayed directly in the terminal. Instead, it is passed to the standard input of the second command. The output of the second command is then displayed in the terminal.

1. ls -l produces output
2. | (pipe) passes that output to grep
3. grep ".txt" filters the input and displays matching lines