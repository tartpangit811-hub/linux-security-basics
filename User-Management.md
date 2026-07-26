# User Management Security Guide

## What is User Management?

User management is the process of controlling who can access a system and what actions they can perform.

Proper user management improves system security and accountability.

---

## Types of Users

### Regular User

A standard account used for daily activities.

Examples:

- Browsing files
- Running applications
- Editing personal documents

---

### Administrator

An account with elevated privileges used for system administration tasks.

Administrator accounts should be used only when necessary.

---

## Principle of Least Privilege

Users should have only the permissions required to perform their tasks.

Benefits:

- Reduces security risks
- Limits accidental damage
- Improves system control

---

## Avoid Shared Accounts

Each person should have their own account.

Benefits:

- Better accountability
- Easier auditing
- Improved security

---

## Strong Password Policies

User accounts should follow strong password requirements:

- At least 12 characters
- Uppercase and lowercase letters
- Numbers
- Special characters

---

## Remove Unused Accounts

Unused accounts can become security risks.

Regularly review accounts and remove those no longer needed.

---

## Review Login Activity

Check who has logged into the system.

Examples:

```bash
who
```

```bash
last
```

---

## Account Locking

Lock accounts that are no longer in use instead of leaving them active.

This reduces unauthorized access risks.

---

## Group Management

Groups help organize permissions.

Examples:

- administrators
- developers
- users

Assign only necessary group memberships.

---

## Security Best Practices

- Use individual accounts
- Follow least privilege principles
- Use strong passwords
- Remove unused accounts
- Monitor login activity
- Review group memberships regularly

---

## Summary

Effective user management is a key part of Linux security. Proper account control helps protect systems from unauthorized access and reduces security risks.
