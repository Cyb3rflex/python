# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 3 — Variables

## 3.1 What is a Variable?

A variable stores information.

Example:

```python
name = "Cyberflex"
age = 20
```

Here:
- `name` stores text.
- `age` stores a number.

---

## 3.2 Creating Variables

```python
username = "admin"
password = "password123"
ip_address = "192.168.1.10"
port = 80
```

---

## 3.3 Variable Naming Rules

Variable names:
- Can contain letters.
- Can contain numbers.
- Can contain underscores.
- Cannot start with a number.
- Should not contain spaces.
- Are case-sensitive.

**Valid:**

```python
username = "admin"
ip_address = "192.168.1.1"
port80 = 80
```

**Invalid:**

```python
2username = "admin"
user name = "admin"
```

---

## 3.4 Changing Variables

Variables can be changed.

```python
status = "offline"
status = "online"

print(status)
```

**Output:**
```
online
```
