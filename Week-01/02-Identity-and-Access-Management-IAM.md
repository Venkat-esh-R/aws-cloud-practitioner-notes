# Identity and Access Management (IAM)

## What is IAM?

AWS Identity and Access Management (IAM) is a global AWS service that enables secure control over who can access AWS resources and what actions they are allowed to perform.

IAM follows the **principle of least privilege**, ensuring users receive only the permissions required to perform their tasks.

---

# Why is IAM Important?

IAM helps organizations:

- Control access to AWS resources
- Protect sensitive data
- Reduce unauthorized access
- Manage permissions centrally
- Improve cloud security

---

# IAM Components

## Root User

The root user is created when an AWS account is first created.

Characteristics:

- Has complete access to all AWS services.
- Cannot be restricted by IAM policies.
- Should only be used for initial account setup.
- Multi-Factor Authentication (MFA) should always be enabled.

---

## IAM Users

An IAM User represents an individual person or application that requires access to AWS.

Each user can have:

- Username
- Password
- Access Keys
- Individual permissions

Example:

- Administrator
- Developer
- Security Engineer

---

## IAM Groups

An IAM Group is a collection of IAM Users.

Permissions are assigned once to the group instead of individually.

Example:

Developers Group

- Alice
- Bob
- Charlie

All developers receive the same permissions.

---

## IAM Policies

IAM Policies are JSON documents that define permissions.

Policies specify:

- What actions are allowed
- Which AWS resources can be accessed
- Under what conditions access is granted

Policies can be attached to:

- Users
- Groups
- Roles

---

## Multi-Factor Authentication (MFA)

MFA provides an additional layer of security.

Instead of only using a password, users must verify their identity using another authentication factor.

Examples:

- Mobile Authenticator App
- Hardware Token

MFA is strongly recommended for all users and mandatory for the Root User.

---

# Principle of Least Privilege

Users should receive only the permissions necessary to perform their work.

Benefits:

- Reduces security risks
- Prevents accidental changes
- Limits damage if credentials are compromised

---

# Best Practices

- Never use the Root User for daily activities.
- Enable MFA on the Root User.
- Create IAM Users for everyday work.
- Assign permissions using Groups.
- Grant minimum required permissions.
- Rotate access keys regularly.

---

# Key Takeaways

- IAM controls authentication and authorization in AWS.
- Root User has unrestricted access.
- IAM Users represent individuals or applications.
- Groups simplify permission management.
- Policies define permissions.
- MFA increases account security.
- Always follow the Principle of Least Privilege.
