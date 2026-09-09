# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Suggested 4-Week Teaching Plan

This syllabus provides a structured, 4-week instructional roadmap for teaching Python for Cybersecurity to beginners.

---

## Curriculum Overview

- **Total Duration:** 4 Weeks
- **Pacing:** 5 Days per Week, 2–3 Hours per Day (Lecture + Hands-on Lab)
- **Target Audience:** Cybersecurity students, IT professionals, and beginners with zero prior coding experience.

---

## Week 1: Python Fundamentals & Control Flow

| Day | Modules Covered | Topics & Core Concepts | Practical Lab / Activity |
|---|---|---|---|
| **Day 1** | Module 1 & 2 | What is Python in Cyber, Environment Setup (VS Code/IDLE), Syntax, Comments | Install Python, create `hello_security.py`, practice syntax |
| **Day 2** | Module 3 & 4 | Variables, Data Types (str, int, float, bool), Type Checking & Casting | Create variable profiles for IP addresses, ports, and threat flags |
| **Day 3** | Module 5 & 6 | User Input (`input()`), Output Formatting (F-Strings), Arithmetic & Logic Operators | Build interactive credential prompter and subnet calculator logic |
| **Day 4** | Module 7 | Conditional Statements (`if`, `elif`, `else`), Nested Conditions | Build a firewall rule evaluator and port authorization decision tree |
| **Day 5** | Module 8 | Loops (`for`, `while`), `break`, `continue`, Loop Automation | Write a port loop scanner stub and automated retry loop |

---

## Week 2: Data Structures, Functions & File Operations

| Day | Modules Covered | Topics & Core Concepts | Practical Lab / Activity |
|---|---|---|---|
| **Day 6** | Modules 9, 10, 11 | Lists, Tuples, Sets, Deduplication, Indexing & Slicing | Deduplicate blocked IP lists and manage static protocol tuples |
| **Day 7** | Module 12 | Dictionaries, Key-Value Lookups, Nested Dictionaries | Build an asset inventory dictionary (hostname -> IP/OS/Status) |
| **Day 8** | Modules 13 & 14 | Functions (`def`, arguments, `return`), String Methods (`split`, `strip`, `replace`) | Create reusable string sanitizers and MAC address formatters |
| **Day 9** | Module 15 | File Handling (`open()`, `with`, read/write/append modes), File Pointers | Build a failed login log parser reading from `auth.log` |
| **Day 10** | Module 16 | Exception Handling (`try`, `except`, `finally`, `raise`), Defensive Programming | Refactor log parser to safely handle missing files and corrupted lines |

---

## Week 3: System Utilities, Regex, Hashing & Data Interchange

| Day | Modules Covered | Topics & Core Concepts | Practical Lab / Activity |
|---|---|---|---|
| **Day 11** | Modules 17, 18, 19 | Imports, `os` Module, `sys` Module, CLI Arguments (`sys.argv`) | Build a CLI tool that takes a directory path and lists file permissions |
| **Day 12** | Module 20 | Subprocess Module (`subprocess.run`, `capture_output`), Executing System Commands Safely | Automate system `ping` probes and network interface status checks |
| **Day 13** | Module 21 | Regular Expressions (`re` module, patterns, match, search, findall) | Extract emails, hashes, and IPv4 addresses from raw text dumps |
| **Day 14** | Module 22 | Cryptographic Hashing (`hashlib`, MD5, SHA-1, SHA-256), Binary Reads | Build a file integrity verification script comparing checksums |
| **Day 15** | Module 23 | JSON Data Handling (`json.loads`, `json.dumps`, file serialization) | Export and load security audit configurations in JSON format |

---

## Week 4: Networking, Security Automation & Capstone Project

| Day | Modules Covered | Topics & Core Concepts | Practical Lab / Activity |
|---|---|---|---|
| **Day 16** | Modules 24 & 26 | HTTP Requests (`requests` library), Status Codes, `ipaddress` Validation | Query Threat Intelligence APIs and classify IP subnets |
| **Day 17** | Module 25 | Socket Programming, TCP Sockets, `connect_ex`, Timeouts | Build a multi-port TCP connectivity checker |
| **Day 18** | Modules 27, 28, 29 | Automation Workflows, Debugging Techniques (`pdb`, logging), PEP 8 & Best Practices | Build an automated system hygiene script with logging and error handling |
| **Day 19** | Module 30 & Module 33 | Ethical & Legal Boundaries (CFAA, Authorization), Beginner Projects 1–5 | Implement Projects 1 through 5 in guided lab sessions |
| **Day 20** | Module 34, 35, 37 | Capstone Project Implementation (CyberAudit), Final Code Review & Outcomes | Final Project presentations, peer code reviews, and graduation wrap-up |
