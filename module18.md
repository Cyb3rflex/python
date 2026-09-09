# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 16 — Exception Handling

Errors can happen when programs run.

Python allows us to handle errors using `try` and `except`.

## 16.1 Basic Exception Handling

```python
try:
    number = int(input("Enter a number: "))
    print(number)
except ValueError:
    print("Invalid number")
```

---

## 16.2 File Error

```python
try:
    with open("logs.txt", "r") as file:
        data = file.read()
except FileNotFoundError:
    print("File does not exist")
```

---

## 16.3 Finally

`finally` runs whether an error happens or not.

```python
try:
    print("Running program")
except Exception:
    print("An error occurred")
finally:
    print("Program finished")
```
