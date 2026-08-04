# Cloud Security Operations & Infrastructure Hardening

## Project Overview

This project is a hands-on AWS cloud security project that I built to gain practical experience with infrastructure security and cloud hardening.

Instead of only learning AWS services, I focused on understanding how cloud environments are secured in real-world scenarios by building, configuring, testing, and validating security controls.

Throughout this project, I encountered real configuration issues, investigated the root cause, applied the appropriate remediation, and verified that each solution worked before documenting it.

The goal of this project was not simply to deploy AWS resources, but to build a secure environment using cloud security best practices.

---

## Technologies Used

- Amazon EC2
- Amazon VPC
- Security Groups
- EC2 Instance Connect Endpoint
- AWS CloudTrail
- Amazon Linux 2023
- SSH
- GitHub

---

## What I Built

I designed a secure AWS environment that includes:

- Enterprise VPC
- Public Subnet
- Private Subnet
- Bastion Host
- Private Application Server
- Security Groups
- EC2 Instance Connect Endpoint
- CloudTrail Monitoring

The environment follows a layered security approach where administrative access is controlled while the application server remains isolated from direct internet access.

---

## Security Work Performed

During this project I:

- Built a segmented VPC using public and private subnets.
- Configured a Bastion Host for secure administrative access.
- Deployed an application server without a public IP address.
- Configured Security Groups using the principle of least privilege.
- Hardened SSH by disabling root login and password authentication.
- Verified secure access using EC2 Instance Connect.
- Reviewed CloudTrail event history to validate AWS management activity.
- Investigated and resolved networking issues during deployment.
- Validated every security configuration after implementation.

---

## Security Cases

This repository documents the security tasks completed during the project.

### CS-001 — Bastion VPC Remediation

Identified and resolved a Bastion Host deployment in the wrong VPC. Rebuilt the infrastructure in the correct VPC and verified secure connectivity.

### CS-002 — SSH Hardening

Reviewed and secured the SSH configuration by disabling root login and password authentication while keeping secure key-based authentication enabled.

### CS-003 — Private Application Access Control

Configured Security Groups to ensure the private application server accepts SSH connections only from the Bastion Host.

### CS-004 — Monitoring and Logging

Verified AWS CloudTrail management events and confirmed AWS account activity was successfully recorded for monitoring and auditing.

---

## Skills Demonstrated

- AWS Infrastructure Security
- VPC Design
- Network Segmentation
- SSH Hardening
- Security Group Management
- CloudTrail Monitoring
- Linux Administration
- Troubleshooting
- Security Validation
- Cloud Security Best Practices

---

## Project Outcome

This project helped me understand how cloud security is applied beyond simply deploying AWS resources.

I gained practical experience building a secure environment, troubleshooting security issues, validating configurations, and documenting the work performed.

Each security case included investigation, implementation, verification, and final validation to ensure the environment was functioning as expected.
