# Hardware Inventory

## Overview

This document maintains an inventory of hardware resources used to support current infrastructure, monitoring, and operational services.

The purpose of this inventory is to provide visibility into infrastructure assets, assist with troubleshooting, support capacity planning, and establish documentation practices commonly used in professional IT environments.

---

## Asset Inventory

| Asset Name                | Asset Type                   | Purpose                                                | Status |
| ------------------------- | ---------------------------- | ------------------------------------------------------ | ------ |
| Rocky Linux Web Server    | Virtual Private Server (VPS) | Hosts support.pschi02.com and related services         | Active |
| Fedora Monitoring Server  | Virtual Private Server (VPS) | Hosts Prometheus, Grafana, and monitoring services     | Active |
| Ubuntu Application Server | Virtual Private Server (VPS) | Application testing and future infrastructure services | Active |

---

## Rocky Linux Web Server

### Purpose

Primary production server supporting the student-to-student collaborative support platform.

### Hosted Services

* Apache Web Server
* MariaDB
* PHP
* osTicket
* Namecheap Private Email Integration

### Associated Domains

* support.pschi02.com

### Status

Active Production System

---

## Fedora Monitoring Server

### Purpose

Dedicated monitoring and observability platform used to collect, visualize, and analyze infrastructure metrics.

### Hosted Services

* Grafana
* Prometheus
* Node Exporter

### Associated Domains

* watchtower.pschi02.com

### Status

Active Monitoring System

---

## Ubuntu Application Server

### Purpose

Application testing, experimentation, and future infrastructure development.

### Hosted Services

* Various testing and development services

### Status

Active Development System

---

## Inventory Management Notes

### Asset Classification

| Classification | Description                                        |
| -------------- | -------------------------------------------------- |
| Production     | Systems supporting active services                 |
| Monitoring     | Systems responsible for observability and alerting |
| Development    | Systems used for testing and experimentation       |

### Documentation Standards

All infrastructure assets should include:

* Purpose
* Operating System
* Hosted Services
* Associated Domains
* Monitoring Status
* Change History

---

## Last Review

Last Updated: June 2026

Inventory Owner: Jose Rojas

Repository: Infrastructure-Inventory

