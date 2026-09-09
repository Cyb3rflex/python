# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 29 — Python Best Practices

Good code should be:
- Readable
- Maintainable
- Secure
- Reusable
- Well documented

---

## 29.1 Use Meaningful Variable Names

**Bad:**
```python
x = "192.168.1.10"
```

**Better:**
```python
target_ip = "192.168.1.10"
```

---

## 29.2 Use Functions

Instead of:

```python
print("Scanning")
print("Scanning")
print("Scanning")
```

Create reusable functions:

```python
def scan_message():
    print("Scanning")
```

---

## 29.3 Use Comments

```python
# Calculate SHA-256 hash
hash_value = hashlib.sha256(data).hexdigest()
```

---

## 29.4 Avoid Hardcoding Secrets

Never store passwords or API keys directly in source code.

**Bad:**
```python
password = "MySecretPassword123"
```

Better approaches include:
- Environment variables
- Secure secret managers
- Configuration files with restricted permissions

---

## 29.5 Validate Input

Never blindly trust user input.

Example:

```python
port = int(input("Enter port: "))

if 1 <= port <= 65535:
    print("Valid port")
else:
    print("Invalid port")
```
