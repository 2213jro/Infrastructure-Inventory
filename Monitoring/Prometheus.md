# Prometheus

## Overview

Prometheus is the primary metrics collection and monitoring platform used within the infrastructure environment.

The platform collects, stores, and manages time-series performance data from monitored systems, providing the foundation for infrastructure visibility and observability.

Prometheus serves as the data source for Grafana dashboards and supports ongoing monitoring of production and monitoring services.

---

## Platform Information

| Item           | Value                 |
| -------------- | --------------------- |
| Software       | Prometheus            |
| Version        | 3.11.2                |
| Classification | Monitoring Platform   |
| Environment    | Production Monitoring |
| Status         | Active                |

---

## Purpose

Prometheus is responsible for collecting infrastructure metrics from monitored systems and storing historical performance data.

The platform supports:

* Infrastructure monitoring
* Performance analysis
* Capacity planning
* Service visibility
* Operational troubleshooting

---

## Monitoring Architecture

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
```

### Components

**Monitored Systems**

Linux servers providing production and monitoring services.

**Node Exporter**

Collects operating system metrics from monitored hosts.

**Prometheus**

Retrieves, stores, and manages collected metrics.

**Grafana**

Displays metrics through dashboards and visual reports.

---

## Collected Metrics

Prometheus collects and stores data related to:

### CPU Metrics

* CPU utilization
* CPU load averages
* Processor activity

### Memory Metrics

* Memory utilization
* Available memory
* Cached memory
* Buffer usage

### Disk Metrics

* Disk utilization
* Available storage
* Filesystem usage

### Network Metrics

* Network throughput
* Incoming traffic
* Outgoing traffic

### System Metrics

* Uptime
* System load
* Operating system information

---

## Data Collection Process

### Metric Scraping

Prometheus periodically requests metrics from configured monitoring targets.

### Data Storage

Collected metrics are stored as time-series data.

### Dashboard Integration

Grafana queries Prometheus to generate monitoring dashboards and visualizations.

---

## Monitoring Targets

Current monitoring targets include:

### Ubuntu Production Server

Responsibilities:

* Web hosting
* Ticket management
* Database services

### Fedora Monitoring Server

Responsibilities:

* Monitoring platform services
* Dashboard visualization
* Metrics collection

---

## Monitoring Validation

The monitoring environment has been validated through service interruption testing.

### Validation Procedure

Node Exporter was intentionally stopped on a monitored system.

### Expected Behavior

Prometheus stopped receiving metrics from the affected target.

### Recovery Test

After restarting Node Exporter:

* Metric collection resumed
* Target status returned to normal
* Dashboard visibility was restored

### Result

Prometheus successfully detected both monitoring interruption and service recovery.

---

## Operational Benefits

### Centralized Metric Collection

Provides a unified platform for infrastructure monitoring.

### Historical Performance Data

Supports trend analysis and troubleshooting.

### Capacity Planning

Provides visibility into resource utilization patterns.

### Service Monitoring

Helps identify outages and performance degradation.

---

## Operational Procedures

### Daily Review

Verify:

* Monitoring targets are reachable
* Metrics are being collected
* No collection failures exist

### Weekly Review

Review:

* Performance trends
* Resource utilization
* Storage requirements
* Monitoring health

---

## Documentation References

Related Documentation:

* Monitoring/Grafana.md
* Assets/Service-Inventory.md
* Assets/Software-Inventory.md
* Documentation/Operational-Procedures.md

---

## Last Review

Last Updated: June 2026

Maintained By: Jose Rojas

Repository: Infrastructure-Inventory

