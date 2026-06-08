# Software Inventory

## Overview

This document maintains an inventory of software installed throughout the infrastructure environment.

The purpose of this inventory is to document software packages, versions, installation locations, and operational purposes. Maintaining a software inventory supports troubleshooting, patch management, security reviews, change management, and infrastructure planning.

---

## Software Inventory

| Software           | Version            | Server Role              | Purpose                    | Status |
| ------------------ | ------------------ | ------------------------ | -------------------------- | ------ |
| Ubuntu Server      | 24.04.4 LTS        | Ubuntu Production Server | Operating System           | Active |
| Apache HTTP Server | 2.4.58             | Ubuntu Production Server | Web Hosting                | Active |
| MariaDB Server     | 10.11.14           | Ubuntu Production Server | Database Services          | Active |
| PHP                | 8.3.6              | Ubuntu Production Server | Application Processing     | Active |
| osTicket           | 1.18.2             | Ubuntu Production Server | Ticket Management Platform | Active |
| Git                | 2.43.0             | Ubuntu Production Server | Version Control            | Active |
| Nano               | 7.2                | Ubuntu Production Server | Text Editing               | Active |
| Fedora Linux       | 43 (Cloud Edition) | Fedora Monitoring Server | Operating System           | Active |
| Grafana            | 10.2.6             | Fedora Monitoring Server | Dashboard Visualization    | Active |
| Prometheus         | 3.11.2             | Fedora Monitoring Server | Metrics Collection         | Active |
| Node Exporter      | 1.11.1             | Fedora Monitoring Server | System Monitoring          | Active |
| Git                | 2.54.0             | Fedora Monitoring Server | Version Control            | Active |
| Nano               | 8.5                | Fedora Monitoring Server | Text Editing               | Active |

---

## Ubuntu Production Server

### Installed Software

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

## Fedora Monitoring Server

### Installed Software

| Software      | Version            | Purpose                 |
| ------------- | ------------------ | ----------------------- |
| Fedora Linux  | 43 (Cloud Edition) | Operating System        |
| Grafana       | 10.2.6             | Dashboard Visualization |
| Prometheus    | 3.11.2             | Metrics Collection      |
| Node Exporter | 1.11.1             | System Monitoring       |
| Git           | 2.54.0             | Version Control         |
| Nano          | 8.5                | Text Editing            |

---

## Software Categories

### Operating Systems

* Ubuntu Server 24.04.4 LTS
* Fedora Linux 43 (Cloud Edition)

### Web Services

* Apache HTTP Server 2.4.58
* PHP 8.3.6

### Database Platforms

* MariaDB Server 10.11.14

### Monitoring Platforms

* Grafana 10.2.6
* Prometheus 3.11.2
* Node Exporter 1.11.1

### Administration Tools

* Git
* Nano

---

## Software Lifecycle Management

Software should be reviewed regularly to ensure:

* Current versions are documented
* Security updates are applied
* Unsupported software is identified
* Upgrade opportunities are evaluated

Version information should be updated following upgrades, migrations, or major configuration changes.

---

## Last Review

Last Updated: June 2026

Inventory Owner: Jose Rojas

Repository: Infrastructure-Inventory
