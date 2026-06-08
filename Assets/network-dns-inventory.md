# DNS Inventory

## Overview

This document maintains an inventory of public-facing domains, subdomains, and DNS-managed services that support the infrastructure environment.

The purpose of this inventory is to document domain ownership, service relationships, DNS dependencies, and platform responsibilities while avoiding disclosure of sensitive infrastructure details.

---

## Domain Inventory

| Domain / Subdomain     | Purpose                               | Service                             | Status |
| ---------------------- | ------------------------------------- | ----------------------------------- | ------ |
| pschi02.com            | Primary project domain                | Website and infrastructure services | Active |
| support.pschi02.com    | Student-to-student support platform   | osTicket                            | Active |
| watchtower.pschi02.com | Monitoring and observability platform | Grafana / Prometheus                | Active |

---

## Service Mapping

| Service                 | Associated Domain      | Function                              |
| ----------------------- | ---------------------- | ------------------------------------- |
| osTicket                | support.pschi02.com    | Ticket management and knowledge base  |
| Grafana                 | watchtower.pschi02.com | Infrastructure monitoring dashboards  |
| Prometheus              | watchtower.pschi02.com | Metrics collection and storage        |
| Namecheap Private Email | pschi02.com            | Email communication and notifications |

---

## DNS Providers

| Provider   | Responsibility                                       |
| ---------- | ---------------------------------------------------- |
| Cloudflare | DNS management, SSL services, and traffic protection |
| Namecheap  | Domain registration and email services               |

---

## Production Services

### support.pschi02.com

**Purpose**

Provides a collaborative student-to-student support platform built on osTicket.

**Services**

* Ticket Management
* Knowledge Base
* User Management
* Email Ticket Intake
* Discord Notifications

**Status**

Active

---

### watchtower.pschi02.com

**Purpose**

Provides centralized infrastructure monitoring and observability.

**Services**

* Grafana Dashboards
* Prometheus Metrics Collection
* Node Exporter Monitoring
* Infrastructure Visibility

**Status**

Active

---

## Email Services

### [support@pschi02.com](mailto:support@pschi02.com)

**Purpose**

Primary support communication address.

**Responsibilities**

* Ticket Intake
* User Communication
* Notification Delivery
* Password Reset Messages

**Provider**

Namecheap Private Email

**Status**

Active

---

## DNS Management Standards

The following information should be maintained internally and excluded from public documentation:

* Public IP addresses
* Private IP addresses
* Internal hostnames
* API keys
* Webhook URLs
* Authentication credentials
* DNS provider account information
* Infrastructure recovery procedures

---

## Change Management

DNS changes should be documented whenever:

* New domains are added
* New subdomains are deployed
* Services are migrated
* DNS providers are changed
* SSL configurations are modified

---

## Last Review

Last Updated: June 2026

Inventory Owner: Jose Rojas

Repository: Infrastructure-Inventory
