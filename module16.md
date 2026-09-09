# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 14 — String Operations

Strings are extremely important in cybersecurity.

Security professionals constantly process:
- Logs
- URLs
- IP addresses
- Usernames
- File names
- HTTP requests
- Command output

---

## 14.1 Convert to Lowercase

```python
text = "ADMIN"
print(text.lower())
```

---

## 14.2 Convert to Uppercase

```python
text = "admin"
print(text.upper())
```

---

## 14.3 Remove Whitespace

```python
text = "   admin   "
print(text.strip())
```

---

## 14.4 Split Text

```python
data = "admin:password:1234"
parts = data.split(":")
print(parts)
```

---

## 14.5 Replace Text

```python
message = "Login failed"
message = message.replace("failed", "successful")
print(message)
```

---

## 14.6 Search Inside Strings

```python
log = "Login failed for user admin"

if "failed" in log:
    print("Failed login detected")
```
