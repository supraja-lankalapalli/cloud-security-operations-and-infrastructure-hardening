# Cloud Security Operations & Infrastructure Hardening

## Project Overview

This project is my hands-on cloud security learning journey focused on AWS. The goal is to understand how secure cloud environments are designed, deployed, and hardened using real-world security practices instead of simply launching cloud resources.

Throughout this project, I will build a secure AWS infrastructure from the ground up while documenting every step, the reasoning behind each configuration, the security risks involved, and the lessons learned.

The project is designed to simulate the work of a Cloud Security Engineer by focusing on infrastructure security, access management, monitoring, threat detection, hardening, and continuous security improvement.

---

## Project Goals

- Learn AWS cloud security through practical implementation.
- Design secure network architectures.
- Protect cloud infrastructure using security best practices.
- Document security decisions and lessons learned.
- Build a professional portfolio demonstrating cloud security skills.

---

## What I Have Completed

### AWS Environment Setup

- Created an AWS environment for the project.
- Configured the initial infrastructure required for security testing.
- Organized the environment for future security implementations.

### Secure Network Design

Built a network architecture that separates public and private resources.

Current architecture includes:

- Public Subnet
- Private Subnet
- Bastion Host
- Private Application Server
- Security Groups
- EC2 Instance Connect Endpoint

### Bastion Host

Configured a Bastion Host inside the public subnet to act as the secure administrative entry point.

Purpose:

- Avoid exposing private servers directly to the internet.
- Allow controlled administrative access.
- Reduce the attack surface.

### Private Application Server

Created an application server inside a private subnet.

Security benefits:

- No public IP address.
- Accessible only through secure internal connections.
- Protected from direct internet access.

### Security Groups

Configured Security Groups to control network traffic.

Implemented:

- SSH access using Port 22
- Restricted inbound rules
- Controlled communication between resources

### Secure Instance Access

Configured EC2 Instance Connect Endpoint to securely access the private instance without exposing it to the public internet.

Successfully connected to:

- Bastion Host
- Private Application Server

Verified secure access using Linux commands such as:

```
whoami
```

---

## Skills Practiced

- AWS EC2
- Amazon VPC
- Public and Private Subnets
- Bastion Host Architecture
- Security Groups
- EC2 Instance Connect Endpoint
- Secure SSH Access
- Linux Administration
- Cloud Infrastructure Hardening

---

## Project Structure

```
README.md

environment/
    initial-setup/
    security/

security-cases/

security-procedures/

security-improvements/
```

---

## Upcoming Work

The next stages of this project will include:

- Infrastructure hardening
- IAM security best practices
- Logging and monitoring
- Threat detection
- Incident response
- Security assessments
- Continuous security improvements
- Security case studies
- Documentation of findings and remediation

---

## Key Learning

This project is helping me understand not only how AWS services work but also why security controls are implemented. Every configuration is documented with its purpose, security impact, and real-world use case to build practical cloud security experience.

---

**Status:** In Progress
