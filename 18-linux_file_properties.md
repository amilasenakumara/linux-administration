# 🐧 Linux File and Directory Properties

In this lecture, we learn about **Linux file and directory properties** and how to view them using commands.

---

## 1️⃣ What are File Properties? 📁

- Every file or directory in Linux has associated **properties**.
- Properties describe **type, ownership, size, creation/modification time**, etc.
- **Windows comparison:**
  - Right-click a folder → Properties → shows name, type, size, owner, creation date, etc.
  - In Linux, this information is shown using commands, not GUI.

---

## 2️⃣ Viewing Properties in Linux

### 2.1 `ls -l` Command 🔍
- Lists **all files and directories with detailed properties**.
- Example:
```bash
ls -l
-rw-r--r-- 1 iafzal iafzal 1024 Dec 29 10:30 somefile
drwxr-xr-x 2 iafzal iafzal 4096 Dec 29 11:00 Desktop
```

### 2.2 Understanding the Columns 📝

| Column | Description |
|--------|-------------|
| **1st** | File type and permissions (`d` = directory, `-` = regular file, `l` = link) |
| **2nd** | Number of hard links (for directories: subdirectories + parent + itself) |
| **3rd** | Owner of the file/directory |
| **4th** | Group that owns the file/directory |
| **5th** | Size of the file in bytes |
| **6th-8th** | Month, date, and time of creation or modification |
| **9th** | Name of the file or directory |

💡 **Example Analysis:**
- `d` in the first column → Directory
- `-` in the first column → Regular file
- `l` in the first column → Symbolic link

---

## 3️⃣ Practical Example

1. **Check current user:**
```bash
whoami  # Output: iafzal
```

2. **Check current directory:**
```bash
pwd  # Output: /home/iafzal
```

3. **List files:**
```bash
ls  # Shows file and directory names only
```

4. **List properties:**
```bash
ls -l  # Shows detailed properties
```

5. **Change directory to a folder:**
```bash
cd Desktop  # Moves to Desktop folder
ls          # List contents inside Desktop
cd ..       # Move back one level
```

6. **Try to cd into a file:**
```bash
cd somefile  # Error: Not a directory
```

---

## 4️⃣ Summary

- **Linux does not show file/folder icons** like Windows.
- Use `ls -l` to see **properties** of files and directories.
- Properties help determine:
  - File type (`d`, `-`, `l`)
  - Ownership (user and group)
  - Size and modification time
- Navigation commands (`cd`, `ls`, `pwd`) complement property viewing.

---

## 5️⃣ Exam Questions & Answers

1. **Q:** Which command shows detailed file properties?  
   **A:** `ls -l`

2. **Q:** What does `d` in the first column of `ls -l` output indicate?  
   **A:** Directory

3. **Q:** How do you check which user owns a file?  
   **A:** Check the 3rd column in `ls -l`

4. **Q:** How do you check the group of a file?  
   **A:** Check the 4th column in `ls -l`

5. **Q:** How do you know a file is a symbolic link?  
   **A:** `l` in the first column of `ls -l`

6. **Q:** How do you go into a directory?  
   **A:** `cd <directory_name>`

7. **Q:** How to list contents inside a directory?  
   **A:** `ls`

8. **Q:** What will happen if you try `cd` into a regular file?  
   **A:** Error: Not a directory

9. **Q:** Which command tells you your current directory?  
   **A:** `pwd`

10. **Q:** How do you go back one directory?  
    **A:** `cd ..`

---

## 6️⃣ Interview Questions & Answers

1. **Q:** How do you view properties of a file in Linux?  
   **A:** `ls -l`

2. **Q:** How to identify a directory in `ls -l` output?  
   **A:** `d` in the first column indicates a directory.

3. **Q:** How do you identify a regular file?  
   **A:** `-` in the first column.

4. **Q:** What does the 3rd column in `ls -l` represent?  
   **A:** Owner of the file or directory.

5. **Q:** What does the 4th column in `ls -l` represent?  
   **A:** Group owner of the file or directory.

6. **Q:** How do you determine the size of a file?  
   **A:** Check the 5th column in `ls -l`.

7. **Q:** How can you navigate into a subdirectory?  
   **A:** `cd <subdirectory_name>`

8. **Q:** What happens if you `cd` into a file?  
   **A:** Linux will return an error saying it's not a directory.

9. **Q:** How do you return to the previous directory?  
   **A:** `cd ..`

10. **Q:** How do you combine navigation and property viewing?  
    **A:** `cd <directory> && ls -l`

---

**✅ Ready for GitHub Publishing**
- Suggested file name: `Linux_File_Prop