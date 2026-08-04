# CS-003 - Private Application Access Control

## Objective

Protect the application server by ensuring it is accessible only through trusted administrative resources.

## Problem

The application server was designed to remain private, so I needed to verify that administrative access was restricted and that the server was not exposed to the internet.

## Environment

- AWS EC2
- Security Groups
- Amazon VPC

## What I Did

- Reviewed the Bastion Host Security Group.
- Reviewed the Private Application Security Group.
- Verified that SSH access to the Bastion Host was restricted.
- Configured the Private Application Security Group to accept SSH only from the Bastion Host Security Group.
- Verified that the application server did not have a public IP address.
- Confirmed that direct internet access was blocked.

## Security Improvements

- Restricted administrative access using Security Groups.
- Protected the application server from direct internet exposure.
- Applied the principle of least privilege for network access.

## Result

The private application server can now be accessed only through the trusted Bastion Host, significantly reducing the attack surface.

## Status

Completed
