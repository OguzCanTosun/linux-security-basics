# sudo & SUID Security Risks

## 🔹 sudo
Allows users to execute commands as root.

Risk:
- Misconfigured sudo rules can allow full root access.

Check:

sudo -l

---

## 🔹 SUID Bit
SUID allows a file to run with the owner's privileges.

Check SUID files:

find / -perm -4000 2>/dev/null

---

## 🔹 Security Impact
- Misconfigured SUID binaries can lead to privilege escalation.

---

## 🔹 Pentester Note
Always enumerate:
- sudo permissions
- SUID binaries
