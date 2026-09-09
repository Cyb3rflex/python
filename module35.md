# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Student Practical Exercises

This document contains hands-on practical lab exercises graded by difficulty level. These exercises reinforce core Python programming principles within realistic cybersecurity contexts.

---

## Lab Exercise 1 — Suspicious IP & IOC Extractor (Beginner)

### Objective
Write a script that reads an unformatted security alert file and extracts all valid IPv4 addresses using regular expressions.

### Requirements:
- Read input from a file named `alerts.txt`.
- Extract all IPv4 strings (`XXX.XXX.XXX.XXX`).
- Use the `ipaddress` module to filter out invalid IP strings.
- Separate private internal IPs from public routable IPs.
- Save the results into `extracted_ips.txt`.

---

## Lab Exercise 2 — Automated Password Strength Evaluator (Beginner)

### Objective
Create a function `evaluate_password(password)` that calculates a security score (0–100) and returns actionable recommendations.

### Requirements:
- Minimum length of 12 characters (+25 points).
- Contains uppercase and lowercase letters (+25 points).
- Contains numbers (+25 points).
- Contains special punctuation symbols (`!@#$%^&*()_+-=`) (+25 points).
- Penalize common password patterns such as `password`, `123456`, or `admin` by setting the score directly to 0.

---

## Lab Exercise 3 — Directory File Integrity Baseline (Intermediate)

### Objective
Create a security baseline tool that hashes every file in a specified directory and alerts when files are modified, added, or deleted.

### Requirements:
- Scan all files inside a target directory using `os.walk` or `os.listdir`.
- Compute SHA-256 for each file.
- Store results in `baseline.json` as `{"filename": "sha256_hash"}`.
- In verification mode, re-scan the folder and compare against `baseline.json`:
  - Output `[MODIFIED]` if the hash changed.
  - Output `[NEW]` if a file exists that was not in the baseline.
  - Output `[DELETED]` if a baseline file is missing.

---

## Lab Exercise 4 — TCP Service Banner Grabber (Intermediate)

### Objective
Build a lightweight Python banner grabber that connects to open ports on a lab target and captures service headers.

### Requirements:
- Prompt the user for a hostname/IP and a target port.
- Establish a socket connection with a 3-second timeout.
- Send a generic probe (e.g., `HEAD / HTTP/1.0\r\n\r\n` or `\r\n`).
- Receive up to 1024 bytes of response banner.
- Gracefully handle connection timeouts and refused connections.

---

## Lab Exercise 5 — Automated Security Advisory Fetcher (Intermediate)

### Objective
Use the `requests` and `json` libraries to query a public security API and display the latest CVE advisories.

### Requirements:
- Send an HTTP GET request with custom User-Agent headers.
- Verify status code `200 OK`.
- Parse the JSON response payload.
- Print CVE ID, Severity, CVSS Score, and Summary in a clean console table.
