# Data Stream

The operating system manages communication between users, programs, and hardware.

Data received by a process is called input, and data produced by a process is called output.

Linux provides three standard streams for processes: standard input, standard output, and standard error.

They are called standard input (stdin), standard output (stdout), and standard error (stderr).

* Standard input (stdin): data received by a process, usually from the keyboard, a file, or another process.

* Standard output (stdout): normal output produced by a process.

* Standard error (stderr): error messages and diagnostic output produced by a process.

Standard input, output, and error are accessed by processes through file descriptors (FDs).

In simple terms, a file descriptor is an ID used by a process to refer to an open input/output resource.

### FD

- FD `0` = stdin
- FD `1` = stdout
- FD `2` = stderr