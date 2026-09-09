# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 15 — File Handling

Cybersecurity professionals work with files constantly.

Examples:
- Log files
- Configuration files
- Reports
- Wordlists
- JSON files
- CSV files
- Security reports

---

## 15.1 Reading a File

Create `logs.txt` with example content:
```
Login successful
Login failed
Login failed
Login successful
```

Python:

```python
file = open("logs.txt", "r")
content = file.read()
print(content)
file.close()
```

---

## 15.2 Using With

A better approach:

```python
with open("logs.txt", "r") as file:
    content = file.read()

print(content)
```

---

## 15.3 Reading Lines

```python
with open("logs.txt", "r") as file:
    for line in file:
        print(line.strip())
```

---

## 15.4 Writing to a File

```python
with open("report.txt", "w") as file:
    file.write("Security Scan Report\n")
    file.write("Scan completed successfully\n")
```

---

## 15.5 Appending to a File

```python
with open("report.txt", "a") as file:
    file.write("New scan completed\n")
```

---

## 15.6 Failed Login Detector

```python
failed_count = 0

with open("logs.txt", "r") as file:
    for line in file:
        if "failed" in line.lower():
            failed_count += 1

print(f"Failed logins: {failed_count}")
```
