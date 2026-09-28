# Path

In a Linux environment, many tasks are performed in the terminal, so understanding file paths is important.

There are two main ways to specify a file path.

They are absolute paths and relative paths.

## Absolute Path

An absolute path starts from the root directory (/) and ends at the target directory or file.

For example, if we want to read a text file named test.md in the test user's home directory, we can use `cat /home/test/test.md`.

This means that `cat` reads `test.md`, which is located in the `test` user's home directory (`/home/test/`).

*Except for the first /, which represents the root directory, the other / characters act as separators between directories.*

## Relative Path

A relative path starts from the current working directory and points to the target directory or file.

For example, if the current working directory is `/home/test/` and test.md is inside it, we can use: `cat ./test.md` because we are already in the directory where `test.md` is located.

`./` represents the current directory, and `../` represents the parent directory.

*The wildcard * can be used to match multiple file and directory names.*

Example: `ls ./test/*`

## Examples

Current location: '`/home/test/my_test/`

---

Absolute Path: '`ls /home/test/`'

Relative Path: '`ls ../`'

---

Absolute Path: '`cat /home/test/my_test/hello.md`'

Relative Path: '`cat ./hello.md`'

---

Absolute Path: '`ls /home/`'

Relative Path: '`ls ../../`'

---

Absolute Path: '`cd /home/test/game/haha/`'

Relative Path: '`cd ../game/haha/`