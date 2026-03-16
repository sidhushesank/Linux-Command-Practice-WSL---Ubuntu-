# Linux Command Practice (WSL - Ubuntu)

## Overview

This repository documents my hands-on practice of essential Linux commands using **Windows Subsystem for Linux (WSL)** with **Ubuntu** on a Windows machine.

The goal is to gain practical knowledge of Linux terminal commands required for working with **Linux Virtual Machines (VMs)** and development environments in professional settings.

---

# Environment Setup

### Operating System

Windows

### Linux Environment

Ubuntu installed using **Windows Subsystem for Linux (WSL)**

### Installation Command

```bash
wsl --install
```

After installation and restart, Ubuntu was installed using:

```bash
wsl --install -d Ubuntu
```

A Linux user account was created:

```
username: sheshank
```

---

# Basic Linux Navigation Commands

## 1. pwd (Print Working Directory)

### Definition

Displays the full path of the current directory.

### Syntax

```bash
pwd
```

### Example Output

```
/home/sheshank
```

---

## 2. ls (List Files)

### Definition

Lists files and directories in the current location.

### Syntax

```bash
ls
```

### Example Output

```
practise
```

---

## 3. ls -l (Long Listing)

### Definition

Shows detailed information about files.

### Syntax

```bash
ls -l
```

### Example Output

```
drwxr-xr-x 2 sheshank sheshank 4096 Mar 16 practise
```

---

## 4. ls -a (Show Hidden Files)

### Definition

Displays hidden files that start with `.`

### Syntax

```bash
ls -a
```

### Example Output

```
.bashrc
.profile
.cache
```

---

## 5. ls -la (Detailed + Hidden Files)

### Definition

Shows detailed information along with hidden files.

### Syntax

```bash
ls -la
```

---

# Directory Operations

## 6. mkdir (Create Directory)

### Definition

Creates a new folder.

### Syntax

```bash
mkdir directory_name
```

### Example

```bash
mkdir practise
```

---

## 7. cd (Change Directory)

### Definition

Used to move between directories.

### Syntax

```bash
cd directory_name
```

### Example

```bash
cd practise
```

---

## 8. cd ~

### Definition

Moves to the home directory.

### Syntax

```bash
cd ~
```

---

# File Operations

## 9. touch (Create File)

### Definition

Creates an empty file.

### Syntax

```bash
touch filename
```

### Example

```bash
touch file1.txt
```

---

## 10. cat (View File Content)

### Definition

Displays file content.

### Syntax

```bash
cat filename
```

### Example

```bash
cat file1.txt
```

---

## 11. vi (Edit File)

### Definition

Linux text editor used to modify files.

### Syntax

```bash
vi filename
```

### Basic vi Commands

| Key | Action           |
| --- | ---------------- |
| i   | insert text      |
| Esc | exit insert mode |
| :w  | save             |
| :q  | quit             |
| :wq | save and quit    |

---

# File Copying

## 12. cp (Copy Files)

### Definition

Creates a duplicate of a file along with its contents.

### Syntax

```bash
cp source destination
```

### Example

```bash
cp file1.txt file2.txt
```

---

# File Renaming / Moving

## 13. mv (Move or Rename)

### Definition

Used to rename or move files.

### Syntax

```bash
mv source destination
```

### Rename Example

```bash
mv file2.txt renamed.txt
```

### Move Example

```bash
mv renamed.txt testfolder/
```

---

# Directory Structure Example

```
/home/sheshank
│
├── practise
│   ├── file1.txt
│   └── renamed.txt
│
└── testfolder
```

Example command used to move files across directories:

```bash
mv renamed.txt ../testfolder/
```

---

# Linux Path Symbols

| Symbol | Meaning           |
| ------ | ----------------- |
| .      | current directory |
| ..     | parent directory  |
| ~      | home directory    |

---

# Commands Practiced

```
pwd
ls
ls -l
ls -a
ls -la
mkdir
cd
touch
cat
vi
cp
mv
```

---

# Screenshots

Screenshots of terminal execution are included in this repository to demonstrate the command outputs and workflow.

---

# Learning Outcome

Through this practice, the following Linux concepts were understood:

* Linux directory structure
* File and directory manipulation
* File viewing and editing
* Copying and moving files
* Hidden files and permissions
* Navigation between directories

These commands form the foundation for working with **Linux servers and virtual machines in real-world development environments**.
