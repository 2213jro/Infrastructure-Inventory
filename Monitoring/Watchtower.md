# Watchtower

## Overview

Watchtower is the centralized monitoring and observability platform supporting the infrastructure environment.

The platform was developed to provide visibility into system performance, resource utilization, service availability, and infrastructure health through the integration of Grafana, Prometheus, and Node Exporter.

Watchtower serves as the operational monitoring hub for production services and supporting infrastructure.

---

## Platform Information

| Item             | Value                              |
| ---------------- | ---------------------------------- |
| Platform Name    | Watchtower                         |
| Classification   | Infrastructure Monitoring Platform |
| Purpose          | Monitoring and Observability       |
| Status           | Active                             |
| Monitoring Stack | Grafana, Prometheus, Node Exporter |

---

## Objectives

The Watchtower platform was created to:

* Monitor infrastructure health
* Track resource utilization
* Improve operational visibility
* Support troubleshooting efforts
* Validate monitoring functionality
* Develop hands-on infrastructure monitoring experience

---

## Architecture

```text
Monitored Servers
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

---

## Core Components

### Grafana

Provides dashboard visualization and reporting.

**Responsibilities**

* Dashboard creation
* Data visualization
* Infrastructure reporting
* Performance analysis

---

### Prometheus

Provides metrics collection and storage.

**Responsibilities**

* Metric collection
* Time-series database management
* Monitoring target management

---

### Node Exporter

Provides operating system metrics from monitored Linux servers.

**Responsibilities**

* CPU monitoring
* Memory monitoring
* Disk monitoring
* Network monitoring
* System uptime tracking

---

## Monitored Resources

The platform provides visibility into:

### System Performance

* CPU utilization
* System load
* Process activity

### Memory Utilization

* Memory consumption
* Available memory
* Cached memory

### Storage Utilization

* Disk usage
* Filesystem capacity
* Available storage

### Network Activity

* Incoming traffic
* Outgoing traffic
* Network throughput

### Availability

* System uptime
* Monitoring target status
* Service visibility

---

## Validation Testing

The monitoring environment was validated through controlled service interruption testing.

### Test Procedure

A monitored Node Exporter service was intentionally stopped.

### Expected Result

* Metrics would stop being collected
* Dashboard visibility would be affected
* Monitoring status would indicate service interruption

### Recovery Test

After restarting the service:

* Metric collection resumed
* Dashboard data returned
* Monitoring visibility was restored

### Outcome

Watchtower successfully detected both the service interruption and recovery event, validating the monitoring workflow.

---

## Operational Benefits

### Centralized Visibility

Provides a single location for reviewing infrastructure health and performance.

### Troubleshooting Support

Helps identify performance bottlenecks and operational issues.

### Historical Analysis

Provides historical metrics for trend analysis and capacity planning.

### Monitoring Validation

Allows monitoring systems to be tested and verified regularly.

---

## Skills Demonstrated

* Linux Administration
* Infrastructure Monitoring
* Grafana Administration
* Prometheus Configuration
* Node Exporter Deployment
* Troubleshooting
* Service Validation Testing
* Performance Monitoring
* Technical Documentation

---

## Related Documentation

* Monitoring/Grafana.md
* Monitoring/Prometheus.md
* Assets/Hardware-Inventory.md
* Assets/Service-Inventory.md
* Assets/Software-Inventory.md
* Documentation/Operational-Procedures.md

---

## Future Enhancements

Potential future improvements include:

* Additional monitoring targets
* Alerting and notification workflows
* Expanded dashboard coverage
* Infrastructure trend analysis
* Monitoring automation

---

## Last Review

Last Updated: June 2026

Maintained By: Jose Rojas

Repository: Infrastructure-Inventory
