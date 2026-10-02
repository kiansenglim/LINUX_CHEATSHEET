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
echo ""
```

---

[↑ Back to Table of Contents](#table-of-contents)



































































