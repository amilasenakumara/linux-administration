# 🐧 Navigating Linux File System Lecture Notes

In this lecture, we will learn how to **navigate a Linux file system** using basic commands.

---

## 1️⃣ Key Commands for Navigation

Linux requires **explicit commands** to navigate, unlike Windows. The three essential commands are:

- **`cd`** → Change Directory
- **`pwd`** → Print Working Directory
- **`ls`** → List directory contents

💡 Without these three commands, you cannot effectively navigate Linux.

---

## 2️⃣ Understanding the Commands

### 2.1 `cd` (Change Directory) 🔄
- Moves you from one directory to another.
- Examples:
  ```bash
  cd /         # Go to root directory
  cd /boot     # Go to boot directory
  cd ..        # Go one directory up
  cd           # Go to home directory
  ```

### 2.2 `pwd` (Print Working Directory) 📍
- Shows the **current directory path**.
- Example:
  ```bash
  pwd
  /var/log
  ```

### 2.3 `ls` (List Directory Contents) 📂
- Lists files and subdirectories.
- Common options:
  - `ls -l` → Long format (shows permissions, owner, size, date, etc.)
  - `ls -ltr` → Long format, sorted by modification time, oldest first

---

## 3️⃣ Comparison: Windows vs Linux Navigation

| Feature                     | Windows                          | Linux                          |
|------------------------------|---------------------------------|--------------------------------|
| Open directory               | Double-click                    | `cd` command                   |
| See contents                 | Automatically shows files        | `ls` command                   |
| Know current location        | Address bar                      | `pwd` command                  |
| Go up one directory          | Back button                      | `cd ..`                        |
| Go to home/root directory    | Click on user folder             | `cd` (home) / `cd /root` (root)|

💡 In Windows, one action often does **three things at once** (change directory, list contents, show path). In Linux, you perform these actions **one by one** using `cd`, `ls`, and `pwd`.

---

## 4️⃣ Practical Navigation Examples

1. **Go to root directory and list contents**
```bash
cd /
pwd    # Output: /
ls -l  # Lists all directories and files in /
```

2. **Navigate to `/var/log` directory**
```bash
cd /var
pwd       # Output: /var
ls -l
cd log
pwd       # Output: /var/log
ls -l
```

3. **Move back to parent directory**
```bash
cd ..      # Moves up one directory
pwd        # Check current directory
```

4. **Go directly to home directory**
```bash
cd         # Takes you to /root if logged in as root, or /home/user for regular user
pwd
```

---

## 5️⃣ Tips for Efficient Navigation

- Use **tab completion** to auto-complete directory names.
- Combine `cd` and `ls` for quick exploration:
```bash
cd /etc && ls -l
```
- Use `pwd` frequently to avoid getting lost.
- Remember `..` to go one step back and `/` for root.

---

## 6️⃣ Summary

- **`cd`** → Move between directories.
- **`pwd`** → Know your current directory.
- **`ls`** → List files and directories.
- Linux navigation is **command-driven**, unlike Windows GUI.
- Practice navigating directories to gain confidence.

---

## 7️⃣ Exam Questions & Answers

1. **Q:** Which command is used to change directories?  
   **A:** `cd`

2. **Q:** How do you check your current directory?  
   **A:** `pwd`

3. **Q:** Which command lists files in long format?  
   **A:** `ls -l`

4. **Q:** How do you move one directory up?  
   **A:** `cd ..`

5. **Q:** What does `cd /` do?  
   **A:** Takes you to the root directory.

6. **Q:** How do you go to the home directory?  
   **A:** `cd`

7. **Q:** What does `ls -ltr` do?  
   **A:** Lists files in long format, sorted by modification time (oldest first).

8. **Q:** How do you navigate to `/var/log` from root?  
   **A:** `cd /var/log`

9. **Q:** How can you combine commands to go to a directory and list its contents?  
   **A:** `cd /etc && ls -l`

10. **Q:** Which Linux command is similar to double-clicking a folder in Windows?  
    **A:** `cd <directory>`

---

## 8️⃣ Interview Questions & Answers

1. **Q:** How do you navigate the Linux file system?  
   **A:** Using `cd` to change directories, `pwd` to know current directory, and `ls` to list contents.

2. **Q:** What command shows the absolute path of your current directory?  
   **A:** `pwd`

3. **Q:** How do you list all files including hidden ones in a directory?  
   **A:** `ls -a`

4. **Q:** Explain the purpose of `cd ..`.  
   **A:** Moves one directory up to the parent directory.

5. **Q:** How do you move directly to the root directory?  
   **A:** `cd /`

6. **Q:** What is the difference between `ls` and `ls -l`?  
   **A:** `ls` lists file names; `ls -l` provides detailed information.

7. **Q:** Can you combine multiple commands in Linux? How?  
   **A:** Yes, using `&&` or `;` e.g., `cd /etc && ls -l`

8. **Q:** How do Linux navigation commands compare to Windows GUI navigation?  
   **A:** Linux requires explicit commands (`cd`, `ls`, `pwd`), while Windows combines changing directory, listing, and path display automatically.

9. **Q:** What is the command to list files sorted by modification time?  
   **A:** `ls -lt`

10. **Q:** How do you navigate to a subdirectory named `sysconfig` inside `/etc`?  
    **A:** `cd /etc/sysconfig`

---

**✅ Ready for GitHub Publishing**
- Suggested file name: `Linux_File_System_Navigation.md`
- Ideal for repository: `Operating-Systems/Documentation`

