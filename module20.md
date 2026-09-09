# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 18 — OS Module

The `os` module allows Python to interact with the operating system.

## 18.1 Current Directory

```python
import os

print(os.getcwd())
```

---

## 18.2 List Files

```python
import os

files = os.listdir()
for file in files:
    print(file)
```

---

## 18.3 Create a Directory

```python
import os

os.mkdir("reports")
```

---

## 18.4 Check if a File Exists

```python
import os

if os.path.exists("logs.txt"):
    print("File exists")
else:
    print("File does not exist")
```

---

## 18.5 Security Example

```python
import os

for file in os.listdir():
    if file.endswith(".log"):
        print(f"Log file found: {file}")
```
