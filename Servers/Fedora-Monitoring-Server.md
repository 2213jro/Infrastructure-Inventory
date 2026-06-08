# Fedora Monitoring Server

## Overview

The Fedora Monitoring Server provides centralized monitoring and observability services for the infrastructure environment.

The server hosts the monitoring stack responsible for collecting, storing, and visualizing infrastructure metrics, allowing administrators to monitor system performance, resource utilization, and service availability.

---

## Server Information

| Item               | Value                           |
| ------------------ | ------------------------------- |
| Server Role        | Fedora Monitoring Server        |
| Operating System   | Fedora Linux 43 (Cloud Edition) |
| Purpose            | Monitoring and Observability    |
| Status             | Active                          |
| CPU Allocation     | 1 vCPU                          |
| Memory Allocation  | 512 MB                          |
| Storage Allocation | 8 GB SSD                        |

---

## Primary Responsibilities

The Fedora Monitoring Server is responsible for:

* Infrastructure monitoring
* Metrics collection
* Dashboard visualization
* Performance reporting
* Monitoring validation
* Operational visibility

---

## Installed Software

| Software      | Version            | Purpose                 |
| ------------- | ------------------ | ----------------------- |
| Fedora Linux  | 43 (Cloud Edition) | Operating System        |
| Grafana       | 10.2.6             | Dashboard Visualization |
| Prometheus    | 3.11.2             | Metrics Collection      |
| Node Exporter | 1.11.1             | System Monitoring       |
| Git           | 2.54.0             | Version Control         |
| Nano          | 8.5                | Text Editing            |

---

## Monitoring Stack

### Grafana

Provides infrastructure dashboards and visualization.

**Responsibilities**

* Dashboard creation
* Performance reporting
* Infrastructure visibility

---

### Prometheus

Provides metrics collection and storage.

**Responsibilities**

* Metric collection
* Time-series storage
* Monitoring target management

---

### Node Exporter

Provides operating system metrics.

**Responsibilities**

* CPU monitoring
* Memory monitoring
* Disk monitoring
* Network monitoring
* Uptime monitoring

---

## Monitored Resources

The monitoring platform collects metrics related to:

### Performance

* CPU utilization
* System load
* Resource consumption

### Memory

* Memory utilization
* Available memory
* Cache usage

### Storage

* Disk utilization
* Filesystem usage
* Available capacity

### Network

* Incoming traffic
* Outgoing traffic
* Network throughput

### Availability

* System uptime
* Monitoring target health
* Service visibility

---

## Monitoring Validation

The monitoring environment has been validated through controlled testing procedures.

### Test Performed

A monitored Node Exporter service was intentionally stopped.

### Result

* Metric collection interruption detected
* Dashboard visibility affected
* Monitoring target status changed

### Recovery Validation

After restarting the service:

* Metric collection resumed
* Dashboards updated normally
* Monitoring visibility was restored

### Outcome

The monitoring platform successfully detected both service interruption and recovery events.

---

## Operational Benefits

### Centralized Visibility

Provides a single platform for reviewing infrastructure health.

### Troubleshooting Support

Assists with identifying performance and availability issues.

### Historical Analysis

Provides historical data for trend analysis and capacity planning.

### Monitoring Validation

Supports testing and verification of monitoring workflows.

---

## Related Services

| Service                | Function                |
| ---------------------- | ----------------------- |
| watchtower.pschi02.com | Monitoring Platform     |
| Grafana                | Dashboard Visualization |
| Prometheus             | Metrics Collection      |
| Node Exporter          | System Monitoring       |

---

## Documentation References

Related Documentation:

* Monitoring/Grafana.md
* Monitoring/Prometheus.md
* Monitoring/Watchtower.md
* Assets/Hardware-Inventory.md
* Assets/Software-Inventory.md
* Documentation/Operational-Procedures.md

---

## Last Review

Last Updated: June 2026

Maintained By: Jose Rojas

Repository: Infrastructure-Inventory

