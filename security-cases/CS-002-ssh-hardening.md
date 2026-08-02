# CS-002: SSH Hardening

## Objective

The objective of this task was to make the SSH service more secure by reviewing the SSH configuration and applying security settings.

---

## Problem

The default SSH configuration allowed root login using SSH keys. I wanted to make the server more secure by disabling direct root login while keeping secure key-based authentication enabled.

---

## Environment

- AWS EC2
- Amazon Linux 2023
- App-Server-01
- SSH

---

## What I Did

- Connected to the EC2 instance.
- Checked the current SSH configuration.
- Verified the SSH authentication settings.
- Disabled root SSH login.
- Kept password authentication disabled.
- Kept public key authentication enabled.
- Validated the SSH configuration.
- Reloaded the SSH service.
- Verified the new configuration.
- Opened a second session to confirm I could still access the server.

---

## Security Improvements

- Disabled direct root login.
- Disabled password authentication.
- Allowed only public key authentication.
- Verified the server was still accessible after the changes.

---

## Status

Completed
