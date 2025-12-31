# Virtualization-Cloud-Architecture
Enterprise-style virtualization and cloud architecture project
## Overview

This project presents an enterprise-ready Azure virtualization and cloud architecture designed using Microsoft best practices. The architecture was developed as a final assessment for a university-level virtualization and cloud computing course and reflects real-world design considerations for security, scalability, and operational resilience.

The environment is structured to support Production, QA/Training, and Dev/Test workloads, each implemented using a consistent three-tier model consisting of Web, Application, and Database subnets.

## Architecture Design

The architecture incorporates the following core Azure services:

- Microsoft Entra ID for centralized identity, MFA, RBAC, and conditional access
- Site-to-site VPN for hybrid connectivity with on-premises users
- Azure Virtual Networks with segmented Web, App, and Database subnets
- Azure Application Gateway with Web Application Firewall (WAF)
- Azure Virtual Machines hosting web, application, and database workloads
- SQL Server Availability Groups for high availability
- Azure Storage for VM disks, diagnostics, and application data
- Azure Backup and Azure Site Recovery for disaster recovery
- Azure Monitor for logging, metrics, and alerting

This layered approach aligns with Microsoft’s Zero Trust model and the Well-Architected Framework.

## Architecture Diagram

![Virtualization Cloud Architecture](diagrams/architecture_diagram.png)

## Environment Separation

Three isolated environments are deployed to support the full development lifecycle:

- **Production** – Live workloads protected by WAF, NSGs, and monitoring
- **QA / Training** – Isolated testing and instructional environment
- **Dev / Test** – Development and experimentation without production risk

Each environment mirrors the same network and compute structure to ensure consistency and reduce configuration drift.

## Security and Reliability

Security is enforced through subnet segmentation, Network Security Groups, Entra ID integration, and Application Gateway WAF. High availability and disaster recovery are achieved using SQL Availability Groups, Azure Backup, and Azure Site Recovery.

## Monitoring and Operations

Azure Monitor provides centralized visibility into virtual machines, networks, gateways, and applications. Metrics, logs, and alerts support proactive operational management.

## Alignment with Best Practices

This design follows guidance from Microsoft Learn documentation, Exam Ref AZ-104, Exam Ref AZ-900, and the Microsoft Well-Architected Framework, demonstrating how enterprise virtualization architectures are deployed in practice.

## Skills Demonstrated

This project demonstrates hands-on skills aligned with enterprise cloud and virtualization roles, including:

- Azure virtual network design with segmented Web, Application, and Database tiers
- Hybrid connectivity using site-to-site VPN
- Identity and access management using Microsoft Entra ID (RBAC, MFA, conditional access)
- Secure application delivery using Azure Application Gateway with Web Application Firewall (WAF)
- Virtual machine deployment and high availability using SQL Server Availability Groups
- Environment separation for Production, QA/Training, and Dev/Test workloads
- Backup and disaster recovery planning using Azure Backup and Azure Site Recovery
- Monitoring and operational visibility using Azure Monitor
- Alignment with Microsoft Zero Trust principles and the Azure Well-Architected Framework

## Closing Summary

This repository reflects a real-world Azure virtualization architecture designed using Microsoft best practices. It highlights both technical depth and architectural decision-making relevant to enterprise cloud, infrastructure, and security-focused roles.




