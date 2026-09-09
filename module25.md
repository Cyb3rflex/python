# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 23 — JSON

JSON stands for JavaScript Object Notation.

JSON is commonly used for:
- APIs
- Configuration files
- Web applications
- Security tools
- Data exchange

---

## 23.1 Import JSON

```python
import json
```

---

## 23.2 Python Dictionary to JSON

```python
import json

user = {
    "username": "admin",
    "role": "administrator"
}

data = json.dumps(user)
print(data)
```

---

## 23.3 JSON to Python

```python
import json

data = '{"username": "admin", "role": "administrator"}'
user = json.loads(data)

print(user["username"])
```

---

## 23.4 Reading JSON Files

```python
import json

with open("config.json", "r") as file:
    config = json.load(file)

print(config)
```
