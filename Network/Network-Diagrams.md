# Network Diagrams

## Overview

This document provides high-level network and service relationship diagrams for the infrastructure environment.

The diagrams are intended to illustrate service flow, platform dependencies, and infrastructure relationships while excluding sensitive information such as IP addresses, hostnames, credentials, and internal configurations.

---

# Infrastructure Overview

```text
Internet Users
       │
       ▼
  Cloudflare DNS
       │
       ▼
   pschi02.com
       │
       ├──────────────┐
       ▼              ▼
support.pschi02.com  watchtower.pschi02.com
       │              │
       ▼              ▼
Ubuntu Production   Fedora Monitoring
      Server            Server
```

---

# Support Platform Architecture

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
Apache Web Server
  │
  ▼
PHP Application Layer
  │
  ▼
osTicket
  │
  ▼
MariaDB
```

### Components

* Cloudflare DNS
* Apache HTTP Server
* PHP
* osTicket
* MariaDB

### Purpose

Provides a student-to-student support platform including ticket management, knowledge base resources, and user support services.

---

# Monitoring Platform Architecture

```text
Monitored Systems
        │
        ▼
   Node Exporter
        │
        ▼
    Prometheus
        │
        ▼
      Grafana
        │
        ▼
Watchtower Dashboards
```

### Components

* Node Exporter
* Prometheus
* Grafana
* Watchtower

### Purpose

Provides infrastructure monitoring, performance visibility, and operational reporting.

---

# Ticket Notification Workflow

```text
User Creates Ticket
          │
          ▼
       osTicket
          │
          ├─────────────► Email Notification
          │
          ▼
 Discord Notification
```

### Components

* osTicket
* Email Services
* Discord Integration

### Purpose

Provides multiple communication channels for ticket awareness and support operations.

---

# DNS Relationship Diagram

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

### Purpose

Illustrates the relationship between the primary domain and supporting services.

---

# Monitoring Data Flow

```text
Ubuntu Production Server
           │
           ▼
      Node Exporter
           │
           ▼
       Prometheus
           │
           ▼
        Grafana
           │
           ▼
       Dashboards
```

### Purpose

Illustrates how infrastructure metrics move through the monitoring environment.

---

# Security Considerations

The following information is intentionally excluded from public network diagrams:

* Public IP addresses
* Internal IP addresses
* Server hostnames
* Firewall rules
* API keys
* Authentication details
* VPN configurations
* Administrative access methods

---

# Documentation References

Related Documentation:

* Network/DNS-Inventory.md
* Network/Cloudflare-Configuration.md
* Monitoring/Grafana.md
* Monitoring/Prometheus.md
* Monitoring/Watchtower.md
* Assets/Service-Inventory.md

---

# Last Review

Last Updated: June 2026

Maintained By: Jose Rojas

Repository: Infrastructure-Inventory

