# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 28 — Debugging

Debugging is the process of finding and fixing errors in programs.

## 28.1 Syntax Errors

Example:

```python
print("Hello"
```

*The closing parenthesis is missing.*

---

## 28.2 Runtime Errors

Example:

```python
number = int("hello")
```

*This produces a `ValueError`.*

---

## 28.3 Logic Errors

A program can run successfully but produce the wrong result.

Example:

```python
a = 10
b = 5

result = a - b
print(result)
```

*If you intended to add the values, the program has a logic error.*

---

## 28.4 Debugging Techniques

Useful techniques include:
- Reading error messages carefully.
- Using `print()`.
- Checking variable values.
- Testing small sections of code.
- Using `try`/`except`.
- Using Python's debugger (`pdb`).
- Searching official documentation.
- Reproducing errors consistently.
