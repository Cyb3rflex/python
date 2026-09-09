# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 20 — Subprocess

The `subprocess` module allows Python to execute external programs.

This is useful for automation.

## 20.1 Running a Command

```python
import subprocess

result = subprocess.run(
    ["whoami"],
    capture_output=True,
    text=True
)

print(result.stdout)
```

---

## 20.2 Running ip

```python
import subprocess

result = subprocess.run(
    ["ip", "addr"],
    capture_output=True,
    text=True
)

print(result.stdout)
```

---

## 20.3 Security Automation

Python can automate existing Linux security tools.

Example:

```python
import subprocess

result = subprocess.run(
    ["nmap", "-sV", "127.0.0.1"],
    capture_output=True,
    text=True
)

print(result.stdout)
```

> **Security Note:** Only scan systems you own or have explicit authorization to test.
