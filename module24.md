# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 22 — Hashing

Hashing is extremely important in cybersecurity.

A hash function converts data into a fixed-length value.

Common hashing algorithms include:
- MD5
- SHA-1
- SHA-256
- SHA-512

Modern applications should generally prefer stronger algorithms such as SHA-256 or better-suited password hashing algorithms such as Argon2 or bcrypt for passwords.

---

## 22.1 SHA-256

Python provides hashing through `hashlib`.

```python
import hashlib

text = "Hello Cybersecurity"

hash_value = hashlib.sha256(
    text.encode()
).hexdigest()

print(hash_value)
```

---

## 22.2 Hashing a File

```python
import hashlib

filename = "example.txt"
sha256 = hashlib.sha256()

with open(filename, "rb") as file:
    while True:
        data = file.read(4096)
        if not data:
            break
        sha256.update(data)

print(sha256.hexdigest())
```

---

## 22.3 Why Hashes Are Useful

Hashes can help with:
- File integrity
- Malware analysis
- Evidence verification
- Download verification
- Digital forensics
- Detecting file modifications
