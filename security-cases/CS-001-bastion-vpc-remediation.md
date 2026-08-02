# CS-001: Bastion Host and Private VPC Remediation

## Objective

The goal of this security case was to securely access an EC2 instance running in a private subnet without exposing it directly to the internet.

---

## Problem

I deployed an application server inside a private subnet. Since the instance did not have a public IP address, I could not connect to it directly using EC2 Instance Connect.

This is a common security design because private instances should not be publicly accessible.

---

## Environment

- AWS EC2
- Amazon Linux 2023
- Enterprise VPC
- Public Subnet
- Private Subnet
- Bastion Host
- EC2 Instance Connect Endpoint
- Security Groups

---

## What I Did

### Step 1 - Verified the Environment

I confirmed that the application server was running inside a private subnet while the Bastion Host was deployed in the public subnet.

---

### Step 2 - Configured Secure Access

To securely access the private instance, I created an EC2 Instance Connect Endpoint inside the VPC.

This allowed secure browser-based SSH access without assigning a public IP address to the application server.

---

### Step 3 - Updated Security Groups

I reviewed the security group rules and allowed SSH (TCP Port 22) only from the Bastion Host security group.

This follows the principle of least privilege by allowing only trusted resources to connect.

---

### Step 4 - Connected to the Private Instance

After creating the EC2 Instance Connect Endpoint, I successfully connected to the private EC2 instance.

I verified the connection by running:

```bash
whoami
```

The command returned:

```bash
ec2-user
```

This confirmed that secure access to the private instance was working successfully.

---

## Security Improvements

- Kept the application server inside a private subnet.
- Avoided assigning a public IP address.
- Used a Bastion Host for administrative access.
- Used an EC2 Instance Connect Endpoint for secure connectivity.
- Restricted SSH access using security groups.

---

## Status

Completed
