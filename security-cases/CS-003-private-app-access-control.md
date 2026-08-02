# CS-003 - Private App Access Control

## Goal

Allow access to the private application server only through the Bastion Host.

## What I did

- Created a Bastion Host Security Group.
- Allowed SSH (Port 22) to the Bastion Host only from my public IP address.
- Configured the Private App Security Group.
- Allowed SSH (Port 22) only from the Bastion Host Security Group.
- Verified that the application server does not have a public IP address.
- Verified that direct internet access to the private server is blocked.

## Verification

- Bastion Host has a public IP.
- Private Application Server has only a private IP.
- SSH access to the private server is allowed only through the Bastion Host.

## Result

The application server remains isolated in the private subnet and can only be accessed securely through the Bastion Host.
