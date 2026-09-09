# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 19 — SYS Module

The `sys` module provides access to Python runtime information and command-line arguments.

## 19.1 Python Version

```python
import sys

print(sys.version)
```

---

## 19.2 Command-Line Arguments

Create `script.py`:

```python
import sys

print(sys.argv)
```

Run:

```bash
python script.py hello
```

---

## 19.3 Security Tool Example

```python
import sys

if len(sys.argv) < 2:
    print("Usage: python scanner.py <target>")
    sys.exit()

target = sys.argv[1]
print(f"Target: {target}")
```
