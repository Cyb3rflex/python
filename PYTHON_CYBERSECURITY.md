# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Table of Contents

1. [Course Overview](#course-overview)
2. [Learning Objectives](#learning-objectives)
3. [Module 1 — Introduction to Python](#module-1--introduction-to-python)
4. [Module 2 — Python Syntax](#module-2--python-syntax)
5. [Module 3 — Variables](#module-3--variables)
6. [Module 4 — Data Types](#module-4--data-types)
7. [Module 5 — Input and Output](#module-5--input-and-output)
8. [Module 6 — Operators](#module-6--operators)
9. [Module 7 — Conditional Statements](#module-7--conditional-statements)
10. [Module 8 — Loops](#module-8--loops)
11. [Module 9 — Lists](#module-9--lists)
12. [Module 10 — Tuples](#module-10--tuples)
13. [Module 11 — Sets](#module-11--sets)
14. [Module 12 — Dictionaries](#module-12--dictionaries)
15. [Module 13 — Functions](#module-13--functions)
16. [Module 14 — String Operations](#module-14--string-operations)
17. [Module 15 — File Handling](#module-15--file-handling)
18. [Module 16 — Exception Handling](#module-16--exception-handling)
19. [Module 17 — Modules and Imports](#module-17--modules-and-imports)
20. [Module 18 — OS Module](#module-18--os-module)
21. [Module 19 — SYS Module](#module-19--sys-module)
22. [Module 20 — Subprocess](#module-20--subprocess)
23. [Module 21 — Regular Expressions](#module-21--regular-expressions)
24. [Module 22 — Hashing](#module-22--hashing)
25. [Module 23 — JSON](#module-23--json)
26. [Module 24 — HTTP Requests](#module-24--http-requests)
27. [Module 25 — Socket Programming](#module-25--socket-programming)
28. [Module 26 — IP Address Handling](#module-26--ip-address-handling)
29. [Module 27 — Automation](#module-27--automation)
30. [Module 28 — Debugging](#module-28--debugging)
31. [Module 29 — Python Best Practices](#module-29--python-best-practices)
32. [Module 30 — Ethical and Legal Use](#module-30--ethical-and-legal-use)
33. [Beginner Cybersecurity Projects](#beginner-cybersecurity-projects)
34. [Final Practical Project](#final-practical-project)
35. [Student Practical Exercises](#student-practical-exercises)
36. [Suggested 4-Week Teaching Plan](#suggested-4-week-teaching-plan)
37. [Course Learning Outcomes](#course-learning-outcomes)

---

# Course Overview

Python is one of the most widely used programming languages in cybersecurity.

Security professionals use Python to automate repetitive tasks, analyze files, process logs, communicate with network services, inspect data, build security tools, and perform authorized security testing.

This course introduces students to Python programming from the beginning and gradually connects programming concepts to cybersecurity.

The course assumes that students have little or no previous programming experience.

---

# Learning Objectives

By the end of this course, students should be able to:

- Understand basic Python programming concepts.
- Write and execute Python programs.
- Work with variables and different data types.
- Use conditional statements.
- Use loops to automate repetitive tasks.
- Work with lists, tuples, sets, and dictionaries.
- Create reusable functions.
- Read and write files.
- Handle errors and exceptions.
- Import and use Python modules.
- Interact with the operating system using Python.
- Execute system commands safely.
- Use regular expressions to search and analyze text.
- Generate file hashes.
- Work with JSON data.
- Send HTTP requests.
- Perform basic socket programming.
- Work with IP addresses.
- Automate cybersecurity tasks.
- Build simple cybersecurity tools.
- Apply Python responsibly and ethically.

---

# Module 1 — Introduction to Python

## 1.1 What is Python?

Python is a high-level, general-purpose programming language known for its simple syntax and readability.

Python was created by Guido van Rossum and first released in 1991.

Python is commonly used for:

- Web development
- Data analysis
- Artificial intelligence
- Machine learning
- Automation
- System administration
- Networking
- Cybersecurity

---

## 1.2 Why Python is Important in Cybersecurity

Cybersecurity involves many repetitive tasks.

Python allows security professionals to automate these tasks.

Examples include:

- Log analysis
- File analysis
- Password auditing
- Network scanning
- IP address processing
- Hash generation
- Security monitoring
- Report generation
- Data extraction
- API interaction

Instead of manually performing a task hundreds of times, Python can automate it.

---

## 1.3 Advantages of Python

Python is popular because it is:

- Easy to learn
- Easy to read
- Cross-platform
- Open source
- Highly extensible
- Supported by many libraries
- Useful for automation
- Useful for networking
- Useful for security tools

---

## 1.4 Running Python

Check whether Python is installed:

```bash
python --version
# or:
python3 --version
```

Start the Python interactive interpreter:

```bash
python3
```

Example:

```python
print("Hello, Cybersecurity!")
```

Exit Python:

```python
exit()
```

---

## 1.5 Creating a Python File

Create a file:

```bash
nano hello.py
```

Add:

```python
print("Hello, Cybersecurity Students!")
```

Run it:

```bash
python3 hello.py
```

---

# Module 2 — Python Syntax

## 2.1 What is Syntax?

Syntax refers to the rules used to write Python programs correctly.

For example:

```python
print("Hello World")
```

Python uses indentation to define blocks of code.

Example:

```python
if True:
    print("This is inside the if statement")
```

Incorrect indentation can cause an error.

---

## 2.2 Comments

Comments are ignored by Python.

Single-line comment:

```python
# This is a comment
print("Hello")
```

Comments are useful for explaining code.

Example:

```python
# Ask the user for their username
username = input("Username: ")
```

---

## 2.3 Multi-Line Comments

Python does not have a dedicated multi-line comment syntax.

Triple quotes can be used for documentation strings:

```python
"""
This is a multi-line
documentation string.
"""
```

---

# Module 3 — Variables

## 3.1 What is a Variable?

A variable stores information.

Example:

```python
name = "Cyberflex"
age = 20
```

Here:
- `name` stores text.
- `age` stores a number.

---

## 3.2 Creating Variables

```python
username = "admin"
password = "password123"
ip_address = "192.168.1.10"
port = 80
```

---

## 3.3 Variable Naming Rules

Variable names:
- Can contain letters.
- Can contain numbers.
- Can contain underscores.
- Cannot start with a number.
- Should not contain spaces.
- Are case-sensitive.

**Valid:**

```python
username = "admin"
ip_address = "192.168.1.1"
port80 = 80
```

**Invalid:**

```python
2username = "admin"
user name = "admin"
```

---

## 3.4 Changing Variables

Variables can be changed.

```python
status = "offline"
status = "online"

print(status)
```

**Output:**
```
online
```

---

# Module 4 — Data Types

Python has several built-in data types.

Common types include:
- String
- Integer
- Float
- Boolean
- List
- Tuple
- Set
- Dictionary

---

## 4.1 Strings

Strings contain text.

```python
username = "admin"
```

Another example:

```python
message = "Welcome to cybersecurity"
```

Check the type:

```python
print(type(username))
```

---

## 4.2 Integers

Integers are whole numbers.

```python
port = 443
attempts = 5
```

---

## 4.3 Floats

Floats are numbers containing decimal values.

```python
temperature = 36.5
```

---

## 4.4 Booleans

Boolean values are `True` or `False`.

Example:

```python
is_logged_in = True
```

---

## 4.5 Checking Data Types

Use `type()`:

```python
username = "admin"
print(type(username))
```

**Output:**
```
<class 'str'>
```

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

---

# Module 6 — Operators

Operators are symbols used to perform operations.

## 6.1 Arithmetic Operators

| Operator | Description |
| :--- | :--- |
| `+` | Addition |
| `-` | Subtraction |
| `*` | Multiplication |
| `/` | Division |
| `%` | Modulus |
| `**` | Exponent |
| `//` | Floor division |

Example:

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a % b)
```

---

## 6.2 Comparison Operators

| Operator | Description |
| :--- | :--- |
| `==` | Equal |
| `!=` | Not equal |
| `>` | Greater than |
| `<` | Less than |
| `>=` | Greater than or equal |
| `<=` | Less than or equal |

Example:

```python
port = 443
print(port == 443)
```

**Output:**
```
True
```

---

## 6.3 Logical Operators

Python has:
- `and`
- `or`
- `not`

Example:

```python
username = "admin"
password = "1234"

if username == "admin" and password == "1234":
    print("Login successful")
```

---

# Module 7 — Conditional Statements

Conditional statements allow programs to make decisions.

## 7.1 If Statement

```python
port = 80

if port == 80:
    print("HTTP port detected")
```

---

## 7.2 If-Else

```python
port = 22

if port == 22:
    print("SSH detected")
else:
    print("Different service")
```

---

## 7.3 If-Elif-Else

```python
port = 443

if port == 80:
    print("HTTP")
elif port == 443:
    print("HTTPS")
elif port == 22:
    print("SSH")
else:
    print("Unknown service")
```

---

## 7.4 Security Example

```python
failed_attempts = 5

if failed_attempts >= 5:
    print("Possible brute-force activity")
else:
    print("Normal login activity")
```

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

---

# Module 10 — Tuples

Tuples are similar to lists but cannot normally be changed after creation.

```python
ports = (21, 22, 80, 443)
```

Access an item:

```python
print(ports[0])
```

Tuples are useful when data should remain unchanged.

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

---

# Module 12 — Dictionaries

Dictionaries store data using key-value pairs.

Example:

```python
user = {
    "username": "admin",
    "role": "administrator",
    "status": "active"
}
```

Access a value:

```python
print(user["username"])
```

---

## 12.1 Adding Values

```python
user["department"] = "IT"
```

---

## 12.2 Changing Values

```python
user["status"] = "disabled"
```

---

## 12.3 Looping Through a Dictionary

```python
for key, value in user.items():
    print(key, value)
```

---

## 12.4 Security Example

```python
system = {
    "ip": "192.168.1.10",
    "hostname": "server01",
    "os": "Linux",
    "status": "online"
}

print(system["ip"])
print(system["os"])
```

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

---

# Module 14 — String Operations

Strings are extremely important in cybersecurity.

Security professionals constantly process:
- Logs
- URLs
- IP addresses
- Usernames
- File names
- HTTP requests
- Command output

---

## 14.1 Convert to Lowercase

```python
text = "ADMIN"
print(text.lower())
```

---

## 14.2 Convert to Uppercase

```python
text = "admin"
print(text.upper())
```

---

## 14.3 Remove Whitespace

```python
text = "   admin   "
print(text.strip())
```

---

## 14.4 Split Text

```python
data = "admin:password:1234"
parts = data.split(":")
print(parts)
```

---

## 14.5 Replace Text

```python
message = "Login failed"
message = message.replace("failed", "successful")
print(message)
```

---

## 14.6 Search Inside Strings

```python
log = "Login failed for user admin"

if "failed" in log:
    print("Failed login detected")
```

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

---

# Module 17 — Modules and Imports

Modules allow us to use code written by others or organize our own code.

## 17.1 Importing a Module

```python
import os
```

---

## 17.2 Importing Specific Functions

```python
from math import sqrt
```

---

## 17.3 Random Module

```python
import random

number = random.randint(1, 100)
print(number)
```

---

## 17.4 Useful Cybersecurity Modules

Some useful Python modules include:
- `os`
- `sys`
- `subprocess`
- `socket`
- `re`
- `hashlib`
- `json`
- `requests`
- `ipaddress`
- `datetime`
- `logging`

---

# Module 18 — OS Module

The `os` module allows Python to interact with the operating system.

## 18.1 Current Directory

```python
import os

print(os.getcwd())
```

---

## 18.2 List Files

```python
import os

files = os.listdir()
for file in files:
    print(file)
```

---

## 18.3 Create a Directory

```python
import os

os.mkdir("reports")
```

---

## 18.4 Check if a File Exists

```python
import os

if os.path.exists("logs.txt"):
    print("File exists")
else:
    print("File does not exist")
```

---

## 18.5 Security Example

```python
import os

for file in os.listdir():
    if file.endswith(".log"):
        print(f"Log file found: {file}")
```

---

# Module 19 — SYS Module

The `sys` module provides access to Python runtime information and command-line arguments.

## 19.1 Python Version

```python
import sys

print(sys.version)
```

---

## 19.2 Command-Line Arguments

Create `script.py`:

```python
import sys

print(sys.argv)
```

Run:

```bash
python script.py hello
```

---

## 19.3 Security Tool Example

```python
import sys

if len(sys.argv) < 2:
    print("Usage: python scanner.py <target>")
    sys.exit()

target = sys.argv[1]
print(f"Target: {target}")
```

---

# Module 20 — Subprocess

The `subprocess` module allows Python to execute external programs.

This is useful for automation.

## 20.1 Running a Command

```python
import subprocess

result = subprocess.run(
    ["whoami"],
    capture_output=True,
    text=True
)

print(result.stdout)
```

---

## 20.2 Running ip

```python
import subprocess

result = subprocess.run(
    ["ip", "addr"],
    capture_output=True,
    text=True
)

print(result.stdout)
```

---

## 20.3 Security Automation

Python can automate existing Linux security tools.

Example:

```python
import subprocess

result = subprocess.run(
    ["nmap", "-sV", "127.0.0.1"],
    capture_output=True,
    text=True
)

print(result.stdout)
```

> **Security Note:** Only scan systems you own or have explicit authorization to test.

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

---

# Module 22 — Hashing

Hashing is extremely important in cybersecurity.

A hash function converts data into a fixed-length value.

Common hashing algorithms include:
- MD5
- SHA-1
- SHA-256
- SHA-512

Modern applications should generally prefer stronger algorithms such as SHA-256 or better-suited password hashing algorithms such as Argon2 or bcrypt for passwords.

---

## 22.1 SHA-256

Python provides hashing through `hashlib`.

```python
import hashlib

text = "Hello Cybersecurity"

hash_value = hashlib.sha256(
    text.encode()
).hexdigest()

print(hash_value)
```

---

## 22.2 Hashing a File

```python
import hashlib

filename = "example.txt"
sha256 = hashlib.sha256()

with open(filename, "rb") as file:
    while True:
        data = file.read(4096)
        if not data:
            break
        sha256.update(data)

print(sha256.hexdigest())
```

---

## 22.3 Why Hashes Are Useful

Hashes can help with:
- File integrity
- Malware analysis
- Evidence verification
- Download verification
- Digital forensics
- Detecting file modifications

---

# Module 23 — JSON

JSON stands for JavaScript Object Notation.

JSON is commonly used for:
- APIs
- Configuration files
- Web applications
- Security tools
- Data exchange

---

## 23.1 Import JSON

```python
import json
```

---

## 23.2 Python Dictionary to JSON

```python
import json

user = {
    "username": "admin",
    "role": "administrator"
}

data = json.dumps(user)
print(data)
```

---

## 23.3 JSON to Python

```python
import json

data = '{"username": "admin", "role": "administrator"}'
user = json.loads(data)

print(user["username"])
```

---

## 23.4 Reading JSON Files

```python
import json

with open("config.json", "r") as file:
    config = json.load(file)

print(config)
```

---

# Module 24 — HTTP Requests

Cybersecurity professionals often interact with web applications and APIs.

Python can send HTTP requests using the `requests` library.

**Install:**

```bash
pip install requests
```

---

## 24.1 GET Request

```python
import requests

response = requests.get("https://example.com")
print(response.status_code)
```

---

## 24.2 Response Content

```python
import requests

response = requests.get("https://example.com")
print(response.text)
```

---

## 24.3 Request Headers

```python
import requests

headers = {
    "User-Agent": "CyberSecurity-Lab"
}

response = requests.get(
    "https://example.com",
    headers=headers
)

print(response.status_code)
```

---

## 24.4 Checking Status Codes

Common HTTP status codes:
- **200** — OK
- **301** — Redirect
- **302** — Redirect
- **400** — Bad Request
- **401** — Unauthorized
- **403** — Forbidden
- **404** — Not Found
- **500** — Server Error

Example:

```python
import requests

response = requests.get("https://example.com")

if response.status_code == 200:
    print("Website is accessible")
elif response.status_code == 403:
    print("Access forbidden")
else:
    print(f"Status: {response.status_code}")
```

> **Security Note:** Use HTTP automation only against websites, APIs, and systems you are authorized to test.

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

---

# Module 26 — IP Address Handling

Python provides the `ipaddress` module for working with IP addresses and networks.

## 26.1 Import IP Address

```python
import ipaddress
```

---

## 26.2 Check an IP

```python
import ipaddress

ip = ipaddress.ip_address("192.168.1.10")
print(ip)
```

---

## 26.3 Check Whether an IP is Private

```python
import ipaddress

ip = ipaddress.ip_address("192.168.1.10")
print(ip.is_private)
```

---

## 26.4 Network Information

```python
import ipaddress

network = ipaddress.ip_network("192.168.1.0/24")

print(network)
print(network.network_address)
print(network.broadcast_address)
```

---

## 26.5 List Hosts

```python
import ipaddress

network = ipaddress.ip_network("192.168.1.0/30")

for host in network.hosts():
    print(host)
```

---

# Module 27 — Automation

One of Python's greatest advantages in cybersecurity is automation.

Automation allows security professionals to reduce repetitive manual work.

Examples include:
- Log analysis
- File scanning
- Hash generation
- Report generation
- Network checks
- System information collection

---

## 27.1 Automated File Scanner

```python
import os

directory = "."

for filename in os.listdir(directory):
    path = os.path.join(directory, filename)
    if os.path.isfile(path):
        print(f"File: {filename}")
```

---

## 27.2 Automated Hash Generator

```python
import hashlib
import os

directory = "."

for filename in os.listdir(directory):
    path = os.path.join(directory, filename)
    
    if os.path.isfile(path):
        sha256 = hashlib.sha256()
        with open(path, "rb") as file:
            while True:
                data = file.read(4096)
                if not data:
                    break
                sha256.update(data)
                
        print(f"{filename}: {sha256.hexdigest()}")
```

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

---

# Module 29 — Python Best Practices

Good code should be:
- Readable
- Maintainable
- Secure
- Reusable
- Well documented

---

## 29.1 Use Meaningful Variable Names

**Bad:**
```python
x = "192.168.1.10"
```

**Better:**
```python
target_ip = "192.168.1.10"
```

---

## 29.2 Use Functions

Instead of:

```python
print("Scanning")
print("Scanning")
print("Scanning")
```

Create reusable functions:

```python
def scan_message():
    print("Scanning")
```

---

## 29.3 Use Comments

```python
# Calculate SHA-256 hash
hash_value = hashlib.sha256(data).hexdigest()
```

---

## 29.4 Avoid Hardcoding Secrets

Never store passwords or API keys directly in source code.

**Bad:**
```python
password = "MySecretPassword123"
```

Better approaches include:
- Environment variables
- Secure secret managers
- Configuration files with restricted permissions

---

## 29.5 Validate Input

Never blindly trust user input.

Example:

```python
port = int(input("Enter port: "))

if 1 <= port <= 65535:
    print("Valid port")
else:
    print("Invalid port")
```

---

# Module 30 — Ethical and Legal Use

Cybersecurity knowledge must be used responsibly.

Python can be used to build powerful security tools. However, using those tools against systems without authorization can be illegal and harmful.

### Authorized Security Testing

Students should only perform security testing against:
- Their own computers.
- Their own networks.
- Intentionally vulnerable labs.
- Capture-the-Flag (CTF) environments.
- Systems where they have explicit written permission.

### Unauthorized Activities

Do **NOT** use these techniques to:
- Attack websites without permission.
- Steal credentials.
- Access private systems.
- Deploy malware.
- Damage systems.
- Evade security controls.
- Conduct unauthorized scanning.

### Responsible Security Principle

> **"Learn how attacks work so you can build better defenses."**

---

# Beginner Cybersecurity Projects

The following projects are designed for beginner cybersecurity students.

---

## Project 1 — Failed Login Detector

### Objective
Create a Python program that reads a log file and counts failed login attempts.

**Example log (`logs.txt`):**
```
Login successful
Login failed
Login failed
Login successful
Login failed
```

**Expected output:**
```
Failed login attempts: 3
```

### Skills Practiced
- File handling
- Strings
- Loops
- Conditions
- Variables

---

## Project 2 — File Hash Generator

### Objective
Create a Python program that generates the SHA-256 hash of a file.

**Example:**
```
File: report.txt

SHA-256:
aabbccddeeff...
```

### Skills Practiced
- File handling
- `hashlib`
- Binary data
- Functions

---

## Project 3 — Password Strength Checker

### Objective
Create a program that evaluates a password based on characteristics such as:
- Length
- Uppercase characters
- Lowercase characters
- Numbers
- Special characters

**Example:**
```
Enter password: Example123!

Password strength: Strong
```

### Example Implementation

```python
import re

password = input("Enter password: ")

score = 0

if len(password) >= 8:
    score += 1

if re.search(r"[A-Z]", password):
    score += 1

if re.search(r"[a-z]", password):
    score += 1

if re.search(r"[0-9]", password):
    score += 1

if re.search(r"[^A-Za-z0-9]", password):
    score += 1

if score >= 4:
    print("Strong password")
elif score >= 3:
    print("Moderate password")
else:
    print("Weak password")
```

> **Note:** This is an educational strength-checking exercise. It is not a substitute for a password manager or a modern enterprise password policy.

---

## Project 4 — IP Address Analyzer

### Objective
Create a program that accepts an IP address and determines:
- Whether it is valid.
- Whether it is private.
- Whether it is global.
- Its version.

**Example:**
```
Enter IP address: 192.168.1.10

Valid IP
Private: True
Version: IPv4
```

---

## Project 5 — Basic Port Checker

### Objective
Create a simple TCP port checker for a system you own or are authorized to test.

The program should:
- Ask for a target.
- Ask for a port.
- Attempt a TCP connection.
- Report whether the port is reachable.

### Skills Practiced
- Sockets
- Networking
