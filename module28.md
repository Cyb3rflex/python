# Python Programming for Cybersecurity

**Course:** Python Programming for Cybersecurity  
**Level:** Beginner  
**Instructor:** Cyberflex  
**Focus:** Python Programming, Cybersecurity Automation, Networking, Security Tools and Practical Labs

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
