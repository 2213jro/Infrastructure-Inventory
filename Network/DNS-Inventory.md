# DNS Inventory

## Overview

This document maintains an inventory of domains, subdomains, and DNS-managed services supporting the infrastructure environment.

The purpose of this inventory is to document service relationships, domain ownership, platform dependencies, and public-facing infrastructure components while avoiding disclosure of sensitive configuration information.

---

## Domain Inventory

| Domain / Subdomain     | Service             | Purpose                                     | Status |
| ---------------------- | ------------------- | ------------------------------------------- | ------ |
| pschi02.com            | Primary Domain      | Primary project domain                      | Active |
| support.pschi02.com    | osTicket Platform   | Student-to-student support services         | Active |
| watchtower.pschi02.com | Monitoring Platform | Infrastructure monitoring and observability | Active |

---

## Service Directory

### pschi02.com

**Purpose**

Primary domain supporting project infrastructure and public-facing services.

**Responsibilities**

* Domain management
* Service organization
* Public access point

**Status**

Active

---

### support.pschi02.com

**Purpose**

Provides access to the student-to-student collaborative support platform.

**Services**

* Ticket Management
* Knowledge Base
* User Management
* Email Ticket Intake
* Discord Notifications

**Supporting Technologies**

* Apache HTTP Server
* PHP
* MariaDB
* osTicket

**Status**

Active

---

### watchtower.pschi02.com

**Purpose**

Provides centralized monitoring and observability services.

**Services**

* Infrastructure Monitoring
* Dashboard Visualization
* Metrics Collection
* Performance Reporting

**Supporting Technologies**

* Grafana
* Prometheus
* Node Exporter

**Status**

Active

---

## Service Relationships

```text
pschi02.com
     │
     ├──────────────► support.pschi02.com
     │                     │
     │                     ▼
     │              Support Platform
     │
     └──────────────► watchtower.pschi02.com
                           │
                           ▼
                    Monitoring Platform
```

---

## Email Services

### [support@pschi02.com](mailto:support@pschi02.com)

**Purpose**

Primary support communication address.

**Functions**

* Ticket Intake
* User Communication
* Notification Delivery
* Password Reset Messages

**Provider**

Namecheap Private Email

**Status**

Active

---

## DNS Management Providers

| Provider   | Responsibility                         |
| ---------- | -------------------------------------- |
| Cloudflare | DNS management and traffic routing     |
| Namecheap  | Domain registration and email services |

---

## Documentation Standards

The following information is intentionally excluded from public DNS documentation:

* Public IP addresses
* Internal IP addresses
* DNS zone exports
* API credentials
* Account information
* Authentication tokens
* Infrastructure recovery information

---

## Change Management

DNS inventory should be updated whenever:

* New domains are registered
* New subdomains are deployed
* Services are retired
* Providers are changed
* Email services are modified

---

## Related Documentation

* Network/Cloudflare-Configuration.md
* Network/Network-Diagrams.md
* Monitoring/Watchtower.md
* Assets/Service-Inventory.md
* Documentation/Change-Log.md

---

## Last Review

Last Updated: June 2026

Maintained By: Jose Rojas

Repository: Infrastructure-Inventory

