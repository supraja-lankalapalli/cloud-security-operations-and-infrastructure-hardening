# CS-002 - SSH Hardening

## Objective

Strengthen SSH security by reducing unnecessary authentication methods and protecting administrative access.

## Problem

The default SSH configuration still allowed root login using SSH keys. Although password authentication was disabled, additional hardening was required to follow security best practices.

## Environment

- Amazon Linux 2023
- AWS EC2
- SSH

## What I Did

- Connected to the EC2 instance using EC2 Instance Connect.
- Reviewed the SSH configuration.
- Disabled direct root login.
- Verified that password authentication remained disabled.
- Verified that only public key authentication was enabled.
- Validated the SSH configuration.
- Reloaded the SSH service.
- Opened a second session to confirm the server remained accessible.

## Security Improvements

- Disabled root SSH login.
- Disabled password-based authentication.
- Allowed only key-based authentication.
- Verified secure access after applying the changes.

## Result

The SSH service now follows a more secure configuration while maintaining reliable administrative access.

## Status

Completed
