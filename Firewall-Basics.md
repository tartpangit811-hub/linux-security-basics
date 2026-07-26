# Firewall Basics Guide

## What is a Firewall?

A firewall is a security system that monitors and controls network traffic.

It helps protect devices and servers from unauthorized access.

---

## Why Firewalls Are Important

A firewall can:

- Block unwanted connections
- Reduce security risks
- Protect network services
- Help prevent unauthorized access

---

## How a Firewall Works

A firewall uses rules to decide whether to:

- Allow traffic
- Block traffic

Rules are based on:

- IP addresses
- Ports
- Protocols

---

## Common Network Ports

| Port | Service |
|--------|---------|
| 22 | SSH |
| 80 | HTTP |
| 443 | HTTPS |
| 21 | FTP |
| 25 | SMTP |

---

## Allow Only Required Services

Only open ports that are actually needed.

Unused services should remain blocked.

---

## Verify Open Ports

Check listening services:

```bash
netstat -tuln
```

Or:

```bash
ss -tuln
```

---

## Monitor Network Activity

Review active network connections:

```bash
netstat -an
```

---

## Keep Systems Updated

Regularly install updates:

Termux:

```bash
pkg update
pkg upgrade
```

Ubuntu:

```bash
sudo apt update
sudo apt upgrade
```

---

## Public Network Safety

When using public networks:

- Avoid sensitive activities when possible
- Use secure connections
- Verify website security

---

## Security Best Practices

- Open only required ports
- Monitor network activity
- Keep software updated
- Disable unused services
- Review firewall rules regularly

---

## Summary

A firewall is an important layer of defense that helps protect Linux systems from unauthorized network access. Proper firewall management improves overall system security.
