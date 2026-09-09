# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 9 — Lists

Lists store multiple values.

```python
ports = [21, 22, 80, 443]
```

## 9.1 Accessing List Items

```python
ports = [21, 22, 80, 443]
print(ports[0])
```

**Output:**
```
21
```

---

## 9.2 Adding Items

```python
ports.append(8080)
```

---

## 9.3 Removing Items

```python
ports.remove(22)
```

---

## 9.4 List Length

```python
print(len(ports))
```

---

## 9.5 Security Example

```python
suspicious_ips = [
    "192.168.1.20",
    "10.0.0.15",
    "172.16.0.5"
]

for ip in suspicious_ips:
    print(f"Investigate: {ip}")
```
