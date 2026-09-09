# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Beginner Cybersecurity Projects

The following projects are designed for beginner cybersecurity students.

---

## Project 1 — Failed Login Detector

### Objective
Create a Python program that reads a log file and counts failed login attempts.

**Example log (`logs.txt`):**
```
Login successful
Login failed
Login failed
Login successful
Login failed
```

**Expected output:**
```
Failed login attempts: 3
```

### Skills Practiced
- File handling
- Strings
- Loops
- Conditions
- Variables

---

## Project 2 — File Hash Generator

### Objective
Create a Python program that generates the SHA-256 hash of a file.

**Example:**
```
File: report.txt

SHA-256:
aabbccddeeff...
```

### Skills Practiced
- File handling
- `hashlib`
- Binary data
- Functions

---

## Project 3 — Password Strength Checker

### Objective
Create a program that evaluates a password based on characteristics such as:
- Length
- Uppercase characters
- Lowercase characters
- Numbers
- Special characters

**Example:**
```
Enter password: Example123!

Password strength: Strong
```

### Example Implementation

```python
import re

password = input("Enter password: ")

score = 0

if len(password) >= 8:
    score += 1

if re.search(r"[A-Z]", password):
    score += 1

if re.search(r"[a-z]", password):
    score += 1

if re.search(r"[0-9]", password):
    score += 1

if re.search(r"[^A-Za-z0-9]", password):
    score += 1

if score >= 4:
    print("Strong password")
elif score >= 3:
    print("Moderate password")
else:
    print("Weak password")
```

> **Note:** This is an educational strength-checking exercise. It is not a substitute for a password manager or a modern enterprise password policy.

---

## Project 4 — IP Address Analyzer

### Objective
Create a program that accepts an IP address and determines:
- Whether it is valid.
- Whether it is private.
- Whether it is global.
- Its version.

**Example:**
```
Enter IP address: 192.168.1.10

Valid IP
Private: True
Version: IPv4
```

---

## Project 5 — Basic Port Checker

### Objective
Create a simple TCP port checker for a system you own or are authorized to test.

The program should:
- Ask for a target.
- Ask for a port.
- Attempt a TCP connection.
- Report whether the port is reachable.

### Skills Practiced
- Sockets
- Networking
