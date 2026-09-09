# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Module 25 — Socket Programming

Sockets allow programs to communicate over networks.

Python provides socket functionality through the `socket` module.

## 25.1 Import Socket

```python
import socket
```

---

## 25.2 Get Local Hostname

```python
import socket

hostname = socket.gethostname()
print(hostname)
```

---

## 25.3 Get Local IP

```python
import socket

hostname = socket.gethostname()
ip = socket.gethostbyname(hostname)

print(ip)
```

---

## 25.4 Basic Port Checker

A socket can be used to determine whether a TCP service is accepting connections.

Example:

```python
import socket

target = "127.0.0.1"
port = 80

sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
sock.settimeout(1)

result = sock.connect_ex((target, port))

if result == 0:
    print(f"Port {port} is open")
else:
    print(f"Port {port} is closed")

sock.close()
```

---

## 25.5 Simple Port Checker

```python
import socket

target = "127.0.0.1"
ports = [21, 22, 25, 53, 80, 110, 443]

for port in ports:
    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
    sock.settimeout(0.5)
    
    result = sock.connect_ex((target, port))
    
    if result == 0:
        print(f"[OPEN] {port}")
    else:
        print(f"[CLOSED] {port}")
        
    sock.close()
```

> **Security Note:** Port scanning must only be performed on systems you own or have permission to test.
