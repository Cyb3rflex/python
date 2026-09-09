# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 5 — Input and Output

## 5.1 Output

Use `print()`.

```python
print("Hello")
```

Multiple values:

```python
name = "John"
age = 20

print(name)
print(age)
```

---

## 5.2 User Input

Use `input()`.

```python
name = input("Enter your name: ")
print("Hello", name)
```

---

## 5.3 Converting Input

Input is normally returned as a string.

Example:

```python
age = input("Enter your age: ")
age = int(age)
print(age)
```

Or:

```python
age = int(input("Enter your age: "))
```

---

## 5.4 F-Strings

F-strings make it easier to combine text and variables.

```python
name = "Cyberflex"
print(f"Welcome, {name}")
```

Example:

```python
ip = "192.168.1.1"
port = 443
print(f"Connecting to {ip} on port {port}")
```
