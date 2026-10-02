# Linux Commands Cheat Sheet

A personal Linux command reference for development and daily use.

This cheat sheet is based on commands learned and practiced using **Ubuntu on WSL2**.

---

## Table of Contents

1. [Check Current Directory](#1-check-current-directory)
2. [List Files and Directories](#2-list-files-and-directories)
3. [Change Directory](#3-change-directory)
4. [Create Directories](#4-create-directories)
5. [Create Files](#5-create-files)
6. [Write Text to Files](#6-write-text-to-files)
7. [View File Contents](#7-view-file-contents)
8. [Copy Files](#8-copy-files)
9. [Move or Rename Files](#9-move-or-rename-files)
10. [Delete Files](#10-delete-files)
11. [Open Folder in Windows Exploere](#11-open-folder-in-windows-explorer)
12. [Open Folder in VS Code](#12-open-folder-in-vs-code)
13. [Linux and Windows Paths in WSL](#13-linux-and-windows-paths-in-wsl)
14. [Check Linux Information](#14-check-linux-information)
15. [Check Current User](#15-check-current-user)
16. [Command Summary](#16-command-summary)

---

## 1. Check Current Directory

Use `pwd` to display the directory you are currently working in.

```bash
pwd
```

Example:
```text
/home/linux-practice
```

`pwd` means **Print Working Directory**.

[↑ Back to Table of Contents](#table-of-contents)

---

## 2. List Files and Directories

### Basic Listing
```bash
ls
```
Displays files and directories in the current directory.

### Detailed Listing
```bash
ls -l
```

### Show Hidden Files
```bash
ls -a
```
Hidden Linux files normally begin with `.`.

Examples:
```text
.bashrc
.profile
.gitconfig
```

### Detailed Listing Including Hidden Files
```bash
ls -la
```

[↑ Back to Table of Contents](#table-of-contents)

---

## 3. Change Directory

Use `cd` to move between directories.

`cd` means **Change Directory**.

### Enter a Directory
```bash
cd linux-practice
```

### Go Up One Directory

```bash
cd ..
```

### Go to Home Directory
```bash
cd ~
```
or:
```bash
cd
```
`~` represents your home directory.

### Return to Previous Directory
```bash
cd -
```

[↑ Back to Table of Contents](#table-of-contents)

---

## 4. Create Directories
Use `mkdir` to create a directory.
```bash
mkdir linux-practice
```

`mkdir` means **Make Directory**.

### Create Directory Path Safely
```bash
mkdir -p ~/linux-practice
```

The `-p` option crates missing parent directories if necessary and does not report an error if the directory already exists.

Then enter it:
```bash
cd ~/linux-practice
```

[↑ Back to Table of Contents](#table-of-contents)

## 5. Create Files
Use `touch` to create an empty file.

```bash
touch hello.txt
```

If the file already exists, `touch` updates its timestamp rather than deleting its contents.

---

[↑ Back to Table of Contents](#table-of-contents)

## 6. Write Text to Files
The `echo` command prints text.

```bash
echo "Hello Linux"
```

### Write Output to a File
```bash
echo "Hello Linux" > hello.txt
```

The `>` operator redirects the output into the file and **overwrites** existing content.
The `>>` operator redirects the output into the file and **appends** or add content without deleting the existing content.

---

[↑ Back to Table of Contents](#table-of-contents)


## 7. View File Contents
Use `cat` to display the contents of a file.
```bash
cat hello.txt
```
it is useful for quickly viewing small text files directly from the terminal.
---

[↑ Back to Table of Contents](#table-of-contents)

## 8. Copy Files
Use `cp` to copy a file.
```bash
cp hello.txt hello-copy.txt
```

---

[↑ Back to Table of Contents](#table-of-contents)

## 9. Move or Rename Files
`mv` for both moving and renaming.
```bash
mv hello-copy.txt linux.txt
```

---

[↑ Back to Table of Contents](#table-of-contents)

## 10. Delete Files
Use `rm` to remove a file
```bash
rm linux.txt
```

---

[↑ Back to Table of Contents](#table-of-contents)


## 11. open Folder in Windows Explorer
When using Ubuntu on WSL2, open the current Linux directory in Windows File Explorer with 
```bash
explorer.exe .
```
The `.` means **current directory**.
> **Note:** This requires Windows/WSL interoperability. It may not work from restricted environments such as Docker Desktop's internal Linux distribution.
---

[↑ Back to Table of Contents](#table-of-contents)

## 12. Open Folder in VS Code
Open the current directory in VS Code
```bash
code .
```
---

[↑ Back to Table of Contents](#table-of-contents)

## 13. Linux and Windows Paths in WSL
WSL allows Linux to access Windows drives.

---

[↑ Back to Table of Contents](#table-of-contents)

## 14. Check Linux Information
### Kernel and System Information
```bash
uname -a
```
This displays information about the Linux kernel and system architecture.

A WSL2 kernel may contain:
```text
microsoft-standard-WSL2
```

### Linux Distribution Information
```bash
cat /etc/os-release
```
For Ubuntu
```text
NAME="Ubuntu"
PRETTY_NAME="Ubuntu..."

```
---

[↑ Back to Table of Contents](#table-of-contents)

## 15. Check Current User
```bash
whoami
```
Root has extensive permissions, so everyday dev should normally be performed as a regular user.
---

[↑ Back to Table of Contents](#table-of-contents)

## 16. Command Summary
|Command|Purpose|
|---|---|
|`pwd`|Show current directory|
|`ls`| List files and directories|
|`ls -l`| Detailed file listing|
|`ls -a`| Include hidden files|
|`ls -la`| Detailed listing including hidden files|
|`cd folder`| Enter a directory|
|`cd ..`| Go up one directory|
|`cd ~`| Go to home directory|
|`cd -`| Return to previous directory|
|`mkdir foler`| Create a directory|
|`mkdir -p folder`| Create directory/parent path safety|
|`touch file.txt`| Create emptyh file/update timestamp|
|`echo "text"`| Print text|
|`>`| Redirect output and overwrite|
|`>>`| Redirect output and append|
|`cat file.txt`| Display file contents|
|`cp`| Copy|
|`mv`| Move or rename|
|`rm`| Remove|
|`whoami`| Show current user|
|`uname -a`| Show kernel/system information|
|`cat /etc/os-release`| Show Linux distribution information|
|`explorer.exe`| Open current WSL folder in Windows Explorer|
|`code .`| Open current directory in VS COde|


---

[↑ Back to Table of Contents](#table-of-contents)





























































