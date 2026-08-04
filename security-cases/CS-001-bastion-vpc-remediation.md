# CS-001 - Bastion VPC Remediation

## Objective

Build a secure network architecture that allows administrative access to a private EC2 instance without exposing it directly to the internet.

## Problem

While configuring the environment, I discovered that the Bastion Host and the Application Server were deployed in different VPCs. Because of this, the security groups could not communicate, preventing secure SSH access to the private instance.

## Environment

- AWS EC2
- Amazon VPC
- Security Groups
- Amazon Linux 2023

## What I Did

- Reviewed the network configuration.
- Verified the VPC associated with both EC2 instances.
- Identified that the Bastion Host was deployed in the wrong VPC.
- Created a new Bastion Host in the correct Enterprise VPC.
- Configured the required Security Groups.
- Verified secure connectivity between the Bastion Host and the private Application Server.
- Removed the incorrectly deployed Bastion Host after validation.

## Security Improvements

- Maintained network segmentation using public and private subnets.
- Ensured administrative access was provided through a dedicated Bastion Host.
- Prevented direct internet access to the private application server.

## Result

The infrastructure now follows a secure network architecture where administrative access is controlled while the application server remains isolated inside the private subnet.

## Status

Completed
