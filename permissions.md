# File Permissions in Linux (Security Perspective)

## 🔹 What Are File Permissions?
Linux uses file permissions to control **who can read, write, or execute** a file.

Permissions are defined for:
- Owner
- Group
- Others

---

## 🔹 Permission Types
- `r` → read
- `w` → write
- `x` → execute

Example:
-rwxr-xr--

---

## 🔹 Why Permissions Matter in Security
Incorrect permissions can lead to:
- Unauthorized file access
- Credential leakage
- Privilege escalation

---

## 🔹 Common Security Issues
- World-writable files (`777`)
- Executable files owned by root but writable by users
- Sensitive files readable by non-privileged users

---

## 🔹 Example Command
ls -la
chmod 600 sensitive.txt

---

## 🔹 Security Tip
> Always follow the **principle of least privilege**.
