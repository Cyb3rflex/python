# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 7 — Conditional Statements

Conditional statements allow programs to make decisions.

## 7.1 If Statement

```python
port = 80

if port == 80:
    print("HTTP port detected")
```

---

## 7.2 If-Else

```python
port = 22

if port == 22:
    print("SSH detected")
else:
    print("Different service")
```

---

## 7.3 If-Elif-Else

```python
port = 443

if port == 80:
    print("HTTP")
elif port == 443:
    print("HTTPS")
elif port == 22:
    print("SSH")
else:
    print("Unknown service")
```

---

## 7.4 Security Example

```python
failed_attempts = 5

if failed_attempts >= 5:
    print("Possible brute-force activity")
else:
    print("Normal login activity")
```
