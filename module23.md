# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 21 — Regular Expressions

Regular expressions, commonly called regex, allow us to search and extract patterns from text.

Python provides the `re` module.

## 21.1 Import Regex

```python
import re
```

---

## 21.2 Search for an IP Address

```python
import re

text = "Server IP: 192.168.1.10"
pattern = r"\d+\.\d+\.\d+\.\d+"

match = re.search(pattern, text)

if match:
    print(match.group())
```

---

## 21.3 Find Multiple IP Addresses

```python
import re

text = """
192.168.1.10
10.0.0.5
172.16.0.20
"""

pattern = r"\d+\.\d+\.\d+\.\d+"
ips = re.findall(pattern, text)

for ip in ips:
    print(ip)
```

---

## 21.4 Regex for Email Addresses

```python
import re

text = "Contact admin@example.com"
pattern = r"[\w\.-]+@[\w\.-]+\.\w+"

emails = re.findall(pattern, text)
print(emails)
```
