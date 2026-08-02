# CS-002 - SSH Hardening

## Goal

Secure SSH access to the EC2 instances.

## What I did

- Connected to the Bastion Host using EC2 Instance Connect.
- Checked the SSH configuration.
- Verified that root login is disabled.
- Verified that password authentication is disabled.
- Verified that public key authentication is enabled.

## Verification

I confirmed the following settings:

- PermitRootLogin no
- PasswordAuthentication no
- PubkeyAuthentication yes

## Result

SSH access is secured using key-based authentication only. Root login and password authentication are disabled to reduce unauthorized access.
