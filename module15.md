# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 13 — Functions

Functions allow us to create reusable pieces of code.

## 13.1 Creating a Function

```python
def greet():
    print("Welcome to cybersecurity")
```

Call the function:

```python
greet()
```

---

## 13.2 Functions With Parameters

```python
def greet(name):
    print(f"Hello {name}")
```

Call:

```python
greet("Cyberflex")
```

---

## 13.3 Returning Values

```python
def add(a, b):
    return a + b

result = add(10, 5)
print(result)
```

---

## 13.4 Security Example

```python
def check_port(port):
    if port == 22:
        return "SSH"
    elif port == 80:
        return "HTTP"
    elif port == 443:
        return "HTTPS"
    else:
        return "Unknown"

print(check_port(443))
```
