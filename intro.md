## What is Linux?
Linux is a free, open-source operating system that serves as an alternative to Windows and macOS. To understand what this means, let's break it down:

Operating System: Just like Windows or macOS, Linux is the fundamental software that manages your computer's hardware and provides a platform for other programs to run.

Free: Linux costs absolutely nothing to download, install, or use. There are no license fees, subscription costs, or hidden charges.

Open-Source: The source code (the programming instructions) is freely available for anyone to view, modify, and distribute. This transparency ensures security and enables continuous improvement.

Think of Linux as the engine of a car. Just as different car manufacturers use the same type of engine but create different vehicles, various organizations take the Linux "engine" and build complete operating systems around it. These complete packages are called "distributions" or "distros."

## Why we use Linux ? 

Linux is used because it provides a stable, secure, and efficient environment for running systems, especially in servers and cloud infrastructure. Its open-source nature allows full customization, while its lightweight design ensures better performance with minimal resources. Linux also has a strong permission-based security model and integrates seamlessly with modern DevOps tools like Docker and Kubernetes. Due to its reliability, scalability, and widespread support across cloud platforms, it has become the industry standard for backend systems and production deployments.

![Linux Deployment Flow](/assets/mermaid-diagram.png)

## Architecture of the Linux ?

Linux architecture can be understood as a layered system that connects the user to the hardware in a controlled and efficient way. At the top, users interact with the system through applications or the shell (command line). When you type a command like ls, it doesn’t directly talk to the hardware. Instead, the shell sends that request to the kernel, which is the core part of Linux. The kernel acts like a manager that understands the request and decides how to execute it properly.

The kernel then communicates with the hardware (CPU, memory, disk, etc.) to perform the task and sends the result back up to the user. This separation is important because it ensures security, stability, and performance—applications cannot directly access hardware, which prevents misuse and system crashes. In simple terms, the flow is: User → Shell → Kernel → Hardware → back to User, making Linux reliable and efficient for real-world systems.

### Shell:
The shell is a command-line interface where you type commands to interact with the system. It takes your input and sends it to the kernel.

### Kernel:
The kernel is the core of Linux that manages hardware, memory, and processes. It receives requests from the shell and communicates with the hardware to perform tasks.

### Workflow:
User → Shell → Kernel → Hardware → Result back to user

![linux Arch](/assets/linux_arch.png)

## What is Command ? 

A command in Linux is a simple instruction that you type in the terminal to tell the system to perform a specific task. Instead of clicking buttons like in a graphical interface, you use commands such as ls to list files or cd to change directories. These commands are interpreted by the shell and passed to the system to execute, making it a fast and efficient way to interact with the operating system, especially for tasks like managing files, running programs, or automating processes.

## Lets Start With a Basic Commands 

### 1. 📂 `ls` (List files)

**What it does:**
Shows files and folders in a directory

**Syntax:**

```bash
ls
```

**Example:**

```bash
ls -l
```

**Use Case:**
Check what files exist in your project folder before deployment

---

### 2. 📍 `pwd` (Print Working Directory)

**What it does:**
Shows your current location in the system

**Syntax:**

```bash
pwd
```

**Use Case:**
Confirm you're in the correct directory before running commands

---

### 3. 📁 `cd` (Change Directory)

**What it does:**
Moves you from one folder to another

**Syntax:**

```bash
cd folder_name
```

**Example:**

```bash
cd /var/www
```

**Use Case:**
Navigate to your application folder on a server

---

### 4. 📁 `mkdir` (Make Directory)

**What it does:**
Creates a new folder

**Syntax:**

```bash
mkdir folder_name
```

**Example:**

```bash
mkdir project
```

**Use Case:**
Create a directory for a new project or logs

---

### 5. ❌ `rm` (Remove)

**What it does:**
Deletes files or folders

**Syntax:**

```bash
rm file_name
```

**Example:**

```bash
rm test.txt
```

⚠️ Dangerous:

```bash
rm -rf folder_name
```

**Use Case:**
Remove old build files before redeployment

---

### 6. 📄 `cat` (View File Content)

**What it does:**
Displays file content

**Syntax:**

```bash
cat file.txt
```

**Use Case:**
Quickly check configuration files

---

### 7. 📄 `cp` (Copy)

**What it does:**
Copies files or directories

**Syntax:**

```bash
cp source destination
```

**Example:**

```bash
cp app.js backup.js
```

**Use Case:**
Create backup before modifying files

---

### 8. 🔄 `mv` (Move / Rename)

**What it does:**
Moves or renames files

**Syntax:**

```bash
mv old_name new_name
```

**Example:**

```bash
mv file.txt newfile.txt
```

**Use Case:**
Rename config files during deployment

---

### 9. 👀 `top` (System Monitor)

**What it does:**
Shows running processes and CPU usage

**Syntax:**

```bash
top
```

**Use Case:**
Check if your app is consuming too much CPU

---

### 10. 🌐 `ping` (Check Network)

**What it does:**
Checks connectivity to a server

**Syntax:**

```bash
ping google.com
```

**Use Case:**
Verify if your server has internet access

---

