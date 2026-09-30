# Commands and Options (Fundamental)

>> **[Command] --help**: listing the available options and instructions for a command.

>> **ifconfig**: showing the network interface configuration, including the IP address of the machine.

>> **clear (Ctrl + L)**: clearing the terminal screen.

>> **ps**: listing currently running processes.

-e: listing all running processes.

-f: listing processes in full format (including UID, PID, PPID, etc.).

>> **id**: showing user and group ID information.

>> **which**: showing the path of a specific command.

>> **ping**: transmitting network packets to a specific IP address or host.

-c [number]: limiting the number of packets transmitted.

>> **pwd**: showing the current working directory.

>> **ls**: listing files and directories.

-l: listing files and directories with detailed information.

-a: listing all files, including hidden files.

>> **cd**: changing the current directory (moving to a specific directory).

>> **su**: switching to another user account.

>> **useradd**: adding a new user account.

>> **exit**: logging out of the current account or shell.

>> **vi**: executing the Vi text editor.

>> **cat**: showing the contents of a file.

>> **more**: showing the contents of a file one screen at a time. (Press the Space bar to move to the next page.)

>> **file**: showing information about a file and identifying its type.

>> **cp**: copying a file.

-r: copying a directory and its contents recursively.

>> **rm**: removing a file.

-r: removing a directory and its contents recursively.

-f: forcing removal without prompting.

>> **mv**: moving or renaming a file or directory.

>> **chmod**: changing the permissions of a file or directory.

(Types of permission targets)

- u (owner/user)
- g (group)
- o (others)
- a (all)

(Add and remove permissions)

- + (add)
- - (remove)

(Types of permissions)

- r (read)
- w (write)
- x (execute)

(Format)

Example 1: `chmod u+x [file path]`

Example 2: `chmod 762 [file path]` (In the order of user, group, and others.)

>> **find**: finding files and directories based on specific conditions.

-name: searching by name.

-size: searching by file size. (`c` = bytes, `G` = gigabytes.)

-type: searching by file type. (`f` = file, `d` = directory.)

-perm: searching by file permissions.

-user: searching by owner.

-group: searching by group.

>> **grep**: finding a specific pattern, string, or character in text.

-v: showing lines that do not contain the specified pattern or string.

>> **ssh**: connecting to a remote server through SSH.

(Format)

`ssh [account name]@[address]`

-p [port number]: specifying the SSH port number.

-i [identity file]: specifying an identity file, such as a private key.

**A command can be added at the end of the SSH command to execute it on the remote server and return its output.**

>> **sort**: sorting lines of text in a specific order.

>> **uniq**: removing adjacent duplicate lines.

-u: showing only unique lines.

>> **strings**: extracting readable strings from a binary file.

>> **tr**: translating, replacing, or deleting specific characters.

>> **diff**: comparing two files and showing their differences.

>> **base64**: encoding data using Base64.

--decode: decoding Base64-encoded data.

>> **xxd**: creating a hexadecimal dump of a file.

-r: reversing a hexadecimal dump back into its original binary form.

>> **gzip**: compressing a file using gzip compression.

>> **gunzip**: decompressing a file compressed with gzip.

>> **bzip2**: compressing a file using bzip2 compression.

-d: decompressing a bzip2-compressed file.

>> **tar**: creating or extracting tar archives.

-cf: creating a tar archive.

-xf: extracting a tar archive.

>> **nc**: connecting to a host or listening on a port to transmit and receive data.

-n: disabling DNS resolution and using numeric IP addresses.

-v: showing verbose output.

-z: scanning for listening ports without transmitting application data.

-w [seconds]: configuring a timeout.

-l: listening for incoming connections.

`nc -lnvp [port]`: listening on a specified port with numeric addresses and verbose output.

>> **openssl**: providing cryptographic functions and tools for establishing encrypted connections.

s_client: acting as an SSL/TLS client for testing and communicating with SSL/TLS services.

-connect [host]:[port]: specifying the target host and port.

-ign_eof: ignoring EOF from the input and keeping the connection open.