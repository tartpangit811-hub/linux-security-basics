# SSH Security Guide

## What is SSH?

SSH (Secure Shell) is a secure protocol used to remotely access Linux systems.

SSH encrypts communication between devices.

---

## Why SSH Security Is Important

An unsecured SSH service may allow unauthorized access to a system.

Proper SSH security helps protect:

- Servers
- Personal computers
- Virtual machines
- Network devices

---

## Use Strong Passwords

Always use strong passwords for SSH accounts.

Avoid:

- 123456
- password
- admin

Use unique passwords for each account.

---

## Use SSH Keys

SSH keys are more secure than passwords.

Generate a key pair:

```bash
ssh-keygen -t ed25519
```

Or:

```bash
ssh-keygen -t rsa -b 4096
```

---

## Protect Private Keys

Never share:

```text
id_rsa
id_ed25519
```

Only share the public key:

```text
id_rsa.pub
id_ed25519.pub
```

---

## Verify Server Identity

Before connecting, verify the server fingerprint.

This helps prevent man-in-the-middle attacks.

---

## Use Trusted Networks

Avoid accessing important systems from unknown public networks whenever possible.

Use secure and trusted internet connections.

---

## Keep SSH Software Updated

Update OpenSSH regularly.

Termux:

```bash
pkg update
pkg upgrade
```

Linux:

```bash
sudo apt update
sudo apt upgrade
```

---

## Monitor Login Activity

Review logs for suspicious login attempts.

Examples:

```bash
last
```

```bash
who
```

---

## Security Best Practices

- Use strong passwords
- Use SSH keys
- Protect private keys
- Keep software updated
- Monitor login activity
- Verify server identity
- Use trusted networks

---

## Summary

SSH is one of the most important tools in Linux administration. Proper SSH security helps protect systems from unauthorized access and reduces security risks.
