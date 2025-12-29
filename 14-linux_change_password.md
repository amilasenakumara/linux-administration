
# Changing User Password in Linux 🔑

In this lesson, we will cover how to **change the user password** in Linux, either as a root user or as yourself. Password management is a crucial part of Linux system administration.

---

## 1️⃣ When to Change Password

- 💡 **First-time login:** Change your initial password provided by the system.  
- 🔄 **Password not provided:** System may prompt to create a new password automatically.  
- 👤 **As yourself:** Change your own password anytime for security.  
- 👑 **As root:** Force a password change for any user account.

---

## 2️⃣ The `passwd` Command

- **Command syntax:**  
  ```bash
  passwd [username]
  ```
- ⚠ Important: Command is `passwd`, **not** `password`.  
- **Purpose:** Change passwords for yourself or another user (if root).  

### 2.1 Changing Your Own Password

- Type `passwd` and press Enter.  
- System prompts for:
  1. **Current password** – verify identity.
  2. **New password** – enter desired password.
  3. **Confirm new password** – retype to avoid typos.  
- Example:
  ```bash
  passwd
  ```
- System feedback:
  - Password too short → enter at least 8 characters.
  - Dictionary check failed → avoid common words or sequences.  
- Once accepted:
  ```
  passwd: all authentication tokens updated successfully
  ```  

### 2.2 Changing Another User's Password (Root Only)

- Command syntax:
  ```bash
  sudo passwd username
  ```
- Only root can specify a username to change another user's password.  
- Example:
  ```bash
  sudo passwd iafzel
  ```
- Follow prompts to enter the new password for that user.

---

## 3️⃣ Rules for Creating a Strong Password

- ✅ Minimum 8 characters.  
- ✅ Avoid dictionary words.  
- ✅ Avoid sequences like `12345678`.  
- ✅ Mix letters, numbers, and symbols for stronger security.  

---

## 4️⃣ Procedure Summary 📝

1. Open Linux terminal.  
2. Decide if changing **your own password** or **another user's**.  
3. Run `passwd` or `sudo passwd username`.  
4. Enter current password (if changing your own).  
5. Enter new password.  
6. Confirm new password.  
7. Check for errors (too short, dictionary check).  
8. Password updated successfully message confirms the change.  

---

## 5️⃣ Quick Tips 💡

- Resize terminal for better visibility when following steps.  
- Practice changing passwords in multiple ways to understand prompts.  
- Always choose secure, non-dictionary passwords.  

---

## 6️⃣ Exam Questions & Answers 🎓

1. **Q:** What command is used to change a password in Linux?  
   **A:** `passwd`

2. **Q:** Can a normal user change another user's password?  
   **A:** No, only root can change another user's password.

3. **Q:** What is the minimum recommended password length in Linux?  
   **A:** 8 characters

4. **Q:** What happens if your password fails the dictionary check?  
   **A:** The system rejects it; you need to choose a non-dictionary password.

5. **Q:** How can root change the password of a user named `john`?  
   **A:** `sudo passwd john`

6. **Q:** True or False: The command to change a password is `password`.  
   **A:** False. The correct command is `passwd`.

7. **Q:** What are the three prompts when changing your own password?  
   **A:** Current password, new password, confirm new password.

8. **Q:** Why is it important to confirm a new password?  
   **A:** To avoid mistakes or typos in the password.

9. **Q:** Can you change your password without knowing the current password?  
   **A:** Only root can change another user's password without the current password.

10. **Q:** What is a secure practice when creating a password?  
    **A:** Use a mix of letters, numbers, symbols, and avoid common words.

---

## 7️⃣ Interview Questions & Answers 💼

1. **Q:** Explain the difference between changing your own password and another user's password in Linux.  
   **A:** Normal users can only change their own password using `passwd`. Root can change any user's password using `sudo passwd username`.

2. **Q:** Why does Linux enforce a dictionary check for passwords?  
   **A:** To prevent weak passwords that are easy to guess.

3. **Q:** How do you change the root user's password?  
   **A:** Log in as root or use `sudo passwd` to change root's password.

4. **Q:** What is the purpose of confirming the new password during change?  
   **A:** To ensure the password was typed correctly and avoid errors.

5. **Q:** What happens if the new password is too short?  
   **A:** The system rejects it and asks for a longer password.

6. **Q:** Can a password be changed without logging into the terminal?  
   **A:** No, you must use a terminal session to execute `passwd`.

7. **Q:** What are best practices for creating a Linux password?  
   **A:** Minimum 8 characters, mix of letters, numbers, symbols, avoid dictionary words.

8. **Q:** How does root specify which user’s password to change?  
   **A:** By typing `sudo passwd username`.

9. **Q:** Why should you change the initial password immediately after first login?  
   **A:** For security, since the initial password may be known or weak.

10. **Q:** Explain the steps root takes to change a user's password.  
    **A:** Run `sudo passwd username`, enter new password, confirm new password, ensure compliance with security checks.

