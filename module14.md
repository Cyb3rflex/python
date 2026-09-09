# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 12 — Dictionaries

Dictionaries store data using key-value pairs.

Example:

```python
user = {
    "username": "admin",
    "role": "administrator",
    "status": "active"
}
```

Access a value:

```python
print(user["username"])
```

---

## 12.1 Adding Values

```python
user["department"] = "IT"
```

---

## 12.2 Changing Values

```python
user["status"] = "disabled"
```

---

## 12.3 Looping Through a Dictionary

```python
for key, value in user.items():
    print(key, value)
```

---

## 12.4 Security Example

```python
system = {
    "ip": "192.168.1.10",
    "hostname": "server01",
    "os": "Linux",
    "status": "online"
}

print(system["ip"])
print(system["os"])
```
