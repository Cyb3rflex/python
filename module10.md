# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 8 — Loops

Loops allow us to repeat instructions.

## 8.1 For Loop

Example:

```python
for number in range(5):
    print(number)
```

**Output:**
```
0
1
2
3
4
```

---

## 8.2 Loop Through a List

```python
ports = [21, 22, 80, 443]

for port in ports:
    print(port)
```

---

## 8.3 While Loop

```python
counter = 0

while counter < 5:
    print(counter)
    counter += 1
```

---

## 8.4 Break

`break` stops a loop.

```python
ports = [21, 22, 80, 443]

for port in ports:
    if port == 80:
        break
    print(port)
```

---

## 8.5 Continue

`continue` skips the current iteration.

```python
ports = [21, 22, 80, 443]

for port in ports:
    if port == 22:
        continue
    print(port)
```
