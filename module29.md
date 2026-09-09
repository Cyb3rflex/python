# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 27 — Automation

One of Python's greatest advantages in cybersecurity is automation.

Automation allows security professionals to reduce repetitive manual work.

Examples include:
- Log analysis
- File scanning
- Hash generation
- Report generation
- Network checks
- System information collection

---

## 27.1 Automated File Scanner

```python
import os

directory = "."

for filename in os.listdir(directory):
    path = os.path.join(directory, filename)
    if os.path.isfile(path):
        print(f"File: {filename}")
```

---

## 27.2 Automated Hash Generator

```python
import hashlib
import os

directory = "."

for filename in os.listdir(directory):
    path = os.path.join(directory, filename)
    
    if os.path.isfile(path):
        sha256 = hashlib.sha256()
        with open(path, "rb") as file:
            while True:
                data = file.read(4096)
                if not data:
                    break
                sha256.update(data)
                
        print(f"{filename}: {sha256.hexdigest()}")
```
