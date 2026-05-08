
---

# 🐧 Linux - Step Up 

##  1. What is a Linux Command?

A **Linux command** is an instruction you give to the operating system through the **CLI (Command Line Interface)** to perform a task.

👉 Example tasks:

* Create files
* Delete folders
* Check system info
* Manage processes

---

## 📌 2. Syntax of a Linux Command

Basic structure:

```
command [options] [arguments]
```

### 🔍 Breakdown:

### 1. Command

* The actual program or instruction you run
* Example: `ls`, `rm`, `mkdir`

### 2. Options (Flags)

* Modify the behavior of a command
* Usually start with `-` or `--`

👉 Examples:

* `-l` → long format
* `-a` → show hidden files

### 3. Arguments

* The target on which the command acts (file, directory, etc.)

👉 Example:

```
ls -l /home/user
```

| Part         | Meaning                   |
| ------------ | ------------------------- |
| `ls`         | command                   |
| `-l`         | option                    |
| `/home/user` | argument (directory path) |

---

## 📌 3. Real Example

```
rm -rf myfolder
```

| Part       | Meaning                              |
| ---------- | ------------------------------------ |
| `rm`       | remove command                       |
| `-r`       | recursive (delete folder & contents) |
| `-f`       | force (no confirmation)              |
| `myfolder` | argument (folder to delete)          |

👉 ⚠️ Important:
`rm -rf` is **dangerous** — deletes permanently.

---

# Basic Linux Commands

---

## 1. `ls` — List Files & Directories

👉 Shows contents of a directory

```
ls
```

### Common Options:

* `-l` → long format
* `-a` → show hidden files
* `-lh` → human-readable sizes

```
ls -la
```

---

## 2. `pwd` — Print Working Directory

👉 Shows current directory path

```
pwd
```

---

## 3. `cd` — Change Directory

👉 Move between directories

```
cd /home/user
```

### Shortcuts:

* `cd ..` → go back
* `cd ~` → home directory

---

## 4. `mkdir` — Create Directory

```
mkdir myfolder
```

### Options:

* `-p` → create nested directories

```
mkdir -p project/src
```

---

## 5. `rm` — Remove Files/Directories

```
rm file.txt
```

### Options:

* `-r` → recursive (for directories)
* `-f` → force delete

```
rm -rf folder
```

---

## 6. `cp` — Copy Files/Directories

```
cp file.txt backup.txt
```

### Options:

* `-r` → copy directories

```
cp -r folder backup/
```

---

## 7. `mv` — Move / Rename

```
mv file.txt newname.txt
```

👉 Also used to move:

```
mv file.txt /home/user/
```

---

## 8. `touch` — Create Empty File

```
touch file.txt
```

---

## 9. `cat` — View File Content

```
cat file.txt
```

👉 Combine files:

```
cat file1 file2
```

---

## 10. `echo` — Print Text / Write to File

```
echo "Hello Linux"
```

👉 Write to file:

```
echo "Hello" > file.txt
```

---