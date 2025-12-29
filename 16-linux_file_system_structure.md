# 🐧 Linux File System Structure Lecture Notes

In this lecture, we are going to cover the **Linux file system**, its directories, and their purposes.

---

## 1️⃣ Overview of Linux File System

- Linux file system is divided into multiple **directories**, each with a specific purpose.
- Directories are organized hierarchically starting from the **root `/` directory**.
- 💡 Analogy: Think of directories as folders in a well-organized cabinet.

---

## 2️⃣ Important Linux Directories and Their Purpose

### 2.1 `/boot` 🔧
- Contains files for the **boot loader** (e.g., `grub.cfg`).
- Used by the OS to determine which OS/version to start.
- First directory checked during system boot.

### 2.2 `/root` 👑
- Home directory for the **root user**.
- Not to be confused with `/` (root of file system).

### 2.3 `/dev` 💽
- Contains **device files** representing hardware such as disks, CD-ROMs, keyboards, speakers, and USB drives.

### 2.4 `/etc` ⚙️
- Stores all **system and application configuration files**.
- Examples: `sendmail.cf`, DNS configuration files.
- ⚠️ Always backup files before modifying.

### 2.5 `/bin` & `/usr/bin` 📂
- `/bin` contains **basic user commands** (e.g., `ls`, `pwd`).
- In newer systems, `/bin` is linked to `/usr/bin`.

### 2.6 `/sbin` 🛠️
- Contains **system commands** for managing the file system, disks, and other administrative tasks.
- Linked to `/usr/bin`.

### 2.7 `/opt` 💼
- Used for **optional third-party applications** (e.g., Oracle, SAP).
- Not for OS default applications.

### 2.8 `/proc` 📄
- Contains files representing **running processes**.
- Dynamic directory created by the kernel.
- Empty when system is shut down.

### 2.9 `/lib` & `/usr/lib` 📚
- Stores **C/C++ libraries** required by commands and applications.
- Essential for program execution.

### 2.10 `/tmp` 📝
- Directory for **temporary files**.
- Scratch space for files to be deleted later.

### 2.11 `/home` 🏠
- Contains **home directories of regular users**.
- Example: `/home/user1`, `/home/seinfeld`.

### 2.12 `/var` 📜
- Stores **system and application logs**.
- Useful for troubleshooting issues: `/var/log`.

### 2.13 `/run` 🏃
- Stores **temporary runtime files** such as PIDs.
- Used by system daemons at early boot stages.
- Cleared on shutdown.

### 2.14 `/mnt` 🖇️
- Directory used to **mount external file systems**.
- Example: NFS mount points.

### 2.15 `/media` 💿
- Mount point for **CD-ROMs or virtual ISO images**.
- CD-ROM or virtual media appears here when mounted.

---

## 3️⃣ Summary of Linux File System

- Linux file system is **hierarchical** and well-structured.
- Each directory has a **specific purpose** to make management easier.
- Important directories: `/boot`, `/root`, `/dev`, `/etc`, `/bin`, `/sbin`, `/opt`, `/proc`, `/lib`, `/tmp`, `/home`, `/var`, `/run`, `/mnt`, `/media`.
- 💡 Remember: `/root` is root user home, `/` is root directory.

---

## 4️⃣ Exam Questions & Answers

1. **Q:** What is the purpose of `/boot`?  
   **A:** Contains boot loader files like `grub.cfg` for system startup.

2. **Q:** How does `/root` differ from `/`?  
   **A:** `/root` is the home directory of the root user; `/` is the root of the entire file system.

3. **Q:** Which directory stores device files?  
   **A:** `/dev`

4. **Q:** Where are Linux configuration files typically stored?  
   **A:** `/etc`

5. **Q:** What is the purpose of `/opt`?  
   **A:** Holds optional third-party applications.

6. **Q:** Which directory contains running process files?  
   **A:** `/proc`

7. **Q:** Where are system and application logs stored?  
   **A:** `/var`

8. **Q:** Which directory is used for temporary files?  
   **A:** `/tmp`

9. **Q:** What is the role of `/run`?  
   **A:** Stores temporary runtime files like PIDs used by system daemons.

10. **Q:** Where are CD-ROMs or mounted virtual media shown?  
    **A:** `/media`

---

## 5️⃣ Interview Questions & Answers

1. **Q:** Explain the difference between `/root` and `/home`.  
   **A:** `/root` is the root user's home, `/home` stores regular users' home directories.

2. **Q:** What is the function of `/dev`?  
   **A:** Contains device files for hardware peripherals.

3. **Q:** How does `/proc` differ from `/var`?  
   **A:** `/proc` contains temporary files for running processes; `/var` stores persistent logs.

4. **Q:** Where would you find system configuration files?  
   **A:** `/etc`

5. **Q:** What directory is used for optional software installations?  
   **A:** `/opt`

6. **Q:** Why is `/tmp` important?  
   **A:** Provides temporary storage for files that are not meant to be permanent.

7. **Q:** What is the significance of `/sbin`?  
   **A:** Contains system-level commands for administrative purposes.

8. **Q:** How does the kernel interact with `/proc`?  
   **A:** The kernel dynamically creates files in `/proc` to represent running processes.

9. **Q:** Explain the purpose of `/mnt`.  
   **A:** Mount point for external or network file systems.

10. **Q:** How is `/media` different from `/mnt`?  
    **A:** `/media` is used for removable media like CD-ROMs or ISO images, `/mnt` is for manually mounted filesystems.

---

