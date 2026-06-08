# Ubuntu Production Server

## Overview

The Ubuntu Production Server hosts the primary support platform and related infrastructure services.

The server provides web hosting, database services, ticket management functionality, email integration, and notification services supporting the student-to-student collaborative support environment.

---

## Server Information

| Item               | Value                          |
| ------------------ | ------------------------------ |
| Server Role        | Ubuntu Production Server       |
| Operating System   | Ubuntu 24.04.4 LTS             |
| Purpose            | Production Application Hosting |
| Status             | Active                         |
| CPU Allocation     | 1 vCPU                         |
| Memory Allocation  | 2 GB                           |
| Storage Allocation | 48 GB SSD                      |

---

## Primary Responsibilities

The Ubuntu Production Server is responsible for:

* Web hosting
* Ticket management
* Knowledge base services
* Database operations
* Email integration
* Notification services

---

## Installed Software

| Software           | Version     | Purpose                    |
| ------------------ | ----------- | -------------------------- |
| Ubuntu Server      | 24.04.4 LTS | Operating System           |
| Apache HTTP Server | 2.4.58      | Web Hosting                |
| MariaDB Server     | 10.11.14    | Database Services          |
| PHP                | 8.3.6       | Application Processing     |
| osTicket           | 1.18.2      | Ticket Management Platform |
| Git                | 2.43.0      | Version Control            |
| Nano               | 7.2         | Text Editing               |

---

## Hosted Services

### support.pschi02.com

Provides:

* Ticket Management
* Knowledge Base
* User Support Services
* User Authentication

---

### Email Integration

Provides:

* Ticket Intake
* User Notifications
* Password Reset Messages

---

### Discord Integration

Provides:

* Ticket Notifications
* Operational Visibility
* Workflow Awareness

---

## Service Relationships

```text
Users
   │
   ▼
Cloudflare
   │
   ▼
support.pschi02.com
   │
   ▼
Ubuntu Production Server
   │
   ├── Apache
   ├── PHP
   ├── MariaDB
   ├── osTicket
   ├── Email Integration
   └── Discord Notifications
```

---

## Operational Benefits

### Centralized Support Platform

Provides a single location for support services and knowledge management.

### Database Services

Maintains application and user data.

### Communication Services

Supports email and notification workflows.

### Documentation Platform

Supports knowledge sharing and troubleshooting documentation.

---

## Skills Demonstrated

* Linux Administration
* Apache Administration
* MariaDB Administration
* PHP Configuration
* osTicket Deployment
* Email Integration
* Discord Integration
* Infrastructure Documentation
* Troubleshooting

---

## Related Documentation

* Assets/Hardware-Inventory.md
* Assets/Service-Inventory.md
* Assets/Software-Inventory.md
* Network/DNS-Inventory.md
* Documentation/Operational-Procedures.md

---

## Last Review

Last Updated: June 2026

Maintained By: Jose Rojas

Repository: Infrastructure-Inventory

