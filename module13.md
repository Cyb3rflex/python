# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 11 — Sets

Sets store unique values.

```python
ips = {
    "192.168.1.1",
    "192.168.1.2",
    "192.168.1.1"
}

print(ips)
```

The duplicate IP address is removed.

Sets are useful for removing duplicates from security logs.

Example:

```python
logged_ips = [
    "10.0.0.1",
    "10.0.0.2",
    "10.0.0.1",
    "10.0.0.3"
]

unique_ips = set(logged_ips)
print(unique_ips)
```
