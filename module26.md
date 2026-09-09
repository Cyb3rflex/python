# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

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
