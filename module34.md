# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

---

# Final Practical Project — Multi-Function Cybersecurity Utility (CyberAudit)

## Overview

The final practical project integrates all core Python and cybersecurity concepts covered throughout this course into a single, modular, and professional command-line security auditing tool named **CyberAudit**.

---

## Project Objectives

By completing this capstone project, you will:
- Combine file I/O, regex, sockets, OS operations, hashlib, and network validation into an integrated tool.
- Implement a clean menu-driven or argument-based command-line interface.
- Follow defensive coding practices including robust exception handling.
- Produce structured security audit reports in both human-readable and JSON formats.

---

## Tool Architecture & Features

The **CyberAudit** utility consists of five core modules:

1. **System & Environment Reconnaissance:**
   - Detects the current operating system, Python runtime version, hostname, and working directory using `os`, `sys`, and `platform`.

2. **Log File Security Parser:**
   - Reads authentication and server log files.
   - Uses regular expressions (`re`) to extract IP addresses, timestamps, and failed login attempts.
   - Calculates failure thresholds and flags brute-force patterns.

3. **File Integrity & Hash Monitor:**
   - Generates SHA-256 hashes for target files using `hashlib`.
   - Compares hashes against a known-good baseline to detect unauthorized file tampering.

4. **Network & Port Connectivity Probe:**
   - Validates IP addresses using `ipaddress`.
   - Tests TCP reachability for essential security ports (e.g., 21, 22, 80, 443, 8080) using `socket` with custom timeouts.

5. **Audit Report Generator:**
   - Aggregates findings into structured dictionaries.
   - Saves results to `audit_report.json` and `audit_summary.txt`.

---

## Example Implementation

```python
import os
import sys
import socket
import hashlib
import json
import re
from datetime import datetime

class CyberAuditTool:
    def __init__(self):
        self.report_data = {
            "timestamp": datetime.now().isoformat(),
            "system_info": {},
            "log_analysis": {},
            "file_hashes": {},
            "port_scan_results": {}
        }

    def gather_system_info(self):
        print("[*] Gathering system information...")
        self.report_data["system_info"] = {
            "os_name": os.name,
            "current_dir": os.getcwd(),
            "python_version": sys.version.split()[0],
            "hostname": socket.gethostname()
        }
        print("    System information collected successfully.")

    def parse_log_file(self, log_path):
        print(f"[*] Analyzing log file: {log_path}")
        if not os.path.exists(log_path):
            print(f"[!] Warning: Log file '{log_path}' not found.")
            return

        failed_attempts = 0
        ip_pattern = r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})"
        flagged_ips = []

        with open(log_path, "r", encoding="utf-8") as f:
            for line in f:
                if "failed" in line.lower() or "error" in line.lower():
                    failed_attempts += 1
                    match = re.search(ip_pattern, line)
                    if match:
                        flagged_ips.append(match.group(1))

        self.report_data["log_analysis"] = {
            "file_analyzed": log_path,
            "failed_attempts": failed_attempts,
            "flagged_ips": list(set(flagged_ips))
        }
        print(f"    Found {failed_attempts} failed events across {len(set(flagged_ips))} unique IPs.")

    def generate_file_hash(self, file_path):
        print(f"[*] Computing SHA-256 for: {file_path}")
        if not os.path.exists(file_path):
            print(f"[!] File '{file_path}' does not exist.")
            return

        sha256 = hashlib.sha256()
        with open(file_path, "rb") as f:
            while chunk := f.read(4096):
                sha256.update(chunk)
        digest = sha256.hexdigest()
        self.report_data["file_hashes"][file_path] = digest
        print(f"    SHA-256: {digest}")

    def check_port(self, target_host, port, timeout=1.0):
        try:
            with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                s.settimeout(timeout)
                result = s.connect_ex((target_host, port))
                is_open = (result == 0)
                status = "OPEN" if is_open else "CLOSED"
                self.report_data["port_scan_results"][f"{target_host}:{port}"] = status
                print(f"    Port {port} on {target_host}: {status}")
                return is_open
        except Exception as e:
            print(f"[!] Error checking port {port}: {e}")
            return False

    def export_report(self, output_filename="audit_report.json"):
        print(f"[*] Exporting report to {output_filename}...")
        with open(output_filename, "w", encoding="utf-8") as f:
            json.dump(self.report_data, f, indent=4)
        print("    Audit report exported successfully.")

if __name__ == "__main__":
    print("=" * 60)
    print("    CYBERAUDIT - PRACTICAL CYBERSECURITY TOOLKIT")
    print("=" * 60)
    
    auditor = CyberAuditTool()
    auditor.gather_system_info()
    auditor.generate_file_hash("PYTHON_CYBERSECURITY.md")
    auditor.check_port("127.0.0.1", 80)
    auditor.check_port("127.0.0.1", 443)
    auditor.export_report("audit_report.json")
    print("\n[+] Audit execution complete.")
```

---

## Submission & Deliverables

1. **Source Code (`cyber_audit.py`):** Fully commented and error-handled Python script.
2. **Sample Test Data (`test_logs.txt`):** Example logs demonstrating detection of brute-force events.
3. **Execution Report (`audit_report.json`):** Output generated from testing the utility on your local test environment.
