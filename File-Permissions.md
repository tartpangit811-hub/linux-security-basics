# File Permissions Security Guide

## What Are File Permissions?

File permissions control who can:

- Read files
- Modify files
- Execute files

Proper permissions help protect important data from unauthorized access.

---

## Permission Types

### Read (r)

Allows viewing file contents.

Example:

```bash
cat file.txt
```

---

### Write (w)

Allows modifying file contents.

Example:

```bash
nano file.txt
```

---

### Execute (x)

Allows running a file as a program.

Example:

```bash
./script.sh
```

---

## Viewing Permissions

Check permissions using:

```bash
ls -l
```

Example output:

```text
-rwxr-xr-x
```

---

## Permission Values

Common permission settings:

| Value | Meaning |
|---------|---------|
| 777 | Full permissions for everyone |
| 755 | Owner full access, others read and execute |
| 644 | Owner read/write, others read only |
| 600 | Owner only |

---

## Changing Permissions

Use:

```bash
chmod 755 script.sh
```

Example:

```bash
chmod 644 notes.txt
```

---

## File Ownership

Each file has an owner.

View ownership:

```bash
ls -l
```

Change ownership:

```bash
chown username filename
```

---

## Avoid Excessive Permissions

Avoid:

```bash
chmod 777
```

unless absolutely necessary.

Giving full permissions to everyone increases security risks.

---

## Protect Sensitive Files

Examples:

- SSH private keys
- Configuration files
- Backup files
- Personal documents

Restrict access whenever possible.

---

## Principle of Least Privilege

Grant only the permissions required.

Benefits:

- Reduces accidental changes
- Limits unauthorized access
- Improves system security

---

## Security Best Practices

- Review permissions regularly
- Protect sensitive files
- Avoid unnecessary write access
- Use least privilege principles
- Monitor important system files

---

## Summary

File permissions are a fundamental part of Linux security. Proper permission management helps protect systems and sensitive information from unauthorized access.
