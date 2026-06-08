# Service Inventory

## Overview

This document maintains an inventory of services currently deployed throughout the infrastructure environment.

The purpose of this inventory is to document service ownership, functionality, dependencies, and operational status while supporting troubleshooting, maintenance, and infrastructure planning.

---

## Service Inventory

| Service                 | Purpose                               | Platform             | Status |
| ----------------------- | ------------------------------------- | -------------------- | ------ |
| Apache Web Server       | Website and application hosting       | Rocky Linux          | Active |
| MariaDB                 | Database services                     | Rocky Linux          | Active |
| PHP                     | Web application processing            | Rocky Linux          | Active |
| osTicket                | Ticket management platform            | Rocky Linux          | Active |
| Namecheap Private Email | Email communication and ticket intake | Private Email        | Active |
| Prometheus              | Metrics collection and monitoring     | Fedora               | Active |
| Grafana                 | Dashboard visualization and reporting | Fedora               | Active |
| Node Exporter           | Linux system metrics collection       | Rocky Linux / Fedora | Active |
| Cloudflare DNS          | DNS management and security services  | Cloudflare           | Active |

---

## Service Details

### Apache Web Server

**Purpose**

Hosts web applications and websites.

**Responsibilities**

* Serves support.pschi02.com
* Processes incoming web requests
* Supports PHP-based applications

**Status**

Active

---

### MariaDB

**Purpose**

Provides database services for hosted applications.

**Responsibilities**

* Stores application data
* Supports osTicket operations
* Maintains user and ticket records

**Status**

Active

---

### PHP

**Purpose**

Processes server-side application logic.

**Responsibilities**

* Supports osTicket functionality
* Generates dynamic web content

**Status**

Active

---

### osTicket

**Purpose**

Ticketing and support management platform.

**Responsibilities**

* Ticket creation
* Ticket assignment
* User management
* Knowledge base management
* Support workflow tracking

**Associated Domain**

support.pschi02.com

**Status**

Active

---

### Namecheap Private Email

**Purpose**

Business email platform supporting support operations.

**Responsibilities**

* Email communication
* Ticket intake
* User notifications
* Password reset notifications

**Associated Address**

[support@pschi02.com](mailto:support@pschi02.com)

**Status**

Active

---

### Prometheus

**Purpose**

Infrastructure monitoring and metric collection.

**Responsibilities**

* Collects system metrics
* Stores monitoring data
* Supports Grafana dashboards

**Associated Domain**

watchtower.pschi02.com

**Status**

Active

---

### Grafana

**Purpose**

Visualization and reporting platform.

**Responsibilities**

* Dashboard creation
* Infrastructure visibility
* Performance monitoring
* Service health monitoring

**Associated Domain**

watchtower.pschi02.com

**Status**

Active

---

### Node Exporter

**Purpose**

Linux server metric collection.

**Responsibilities**

* CPU monitoring
* Memory monitoring
* Disk monitoring
* Network monitoring
* Uptime monitoring

**Status**

Active

---

### Cloudflare DNS

**Purpose**

DNS management and security services.

**Responsibilities**

* Domain resolution
* DNS record management
* SSL support
* Traffic protection

**Associated Domains**

* pschi02.com
* support.pschi02.com
* watchtower.pschi02.com

**Status**

Active

---

## Service Classification

| Classification | Description                                        |
| -------------- | -------------------------------------------------- |
| Production     | Services supporting active users and applications  |
| Monitoring     | Services responsible for infrastructure visibility |
| Communication  | Services supporting email and notifications        |
| Infrastructure | Core services supporting platform operations       |

---

## Change Management

All service additions, removals, upgrades, and configuration changes should be documented within the repository change log.

---

## Last Review

Last Updated: June 2026

Inventory Owner: Jose Rojas

Repository: Infrastructure-Inventory

