# Access Methods

This document describes how systems in the lab are accessed for administration, monitoring, and testing.

All examples use **sanitized placeholders** rather than real IP addresses, hostnames, or authentication details.

## Proxmox Host

| Method | Example | Purpose |
|---|---|---|
| Web Interface | `https://LAB_SERVER:PORT` | Hypervisor administration |
| SSH | `ssh ADMIN_USER@LAB_SERVER` | Command-line management |

## Ubuntu Virtual Machines

| Method | Example | Purpose |
|---|---|---|
| SSH | `ssh VM_ADMIN@LAB_VM` | Remote system administration |
| Hypervisor Console | Proxmox web console | VM troubleshooting |

## Docker-Based Services

| Method | Example | Purpose |
|---|---|---|
| Web Interface | `https://LAB_SERVICE:PORT` | Service administration |
| Local Host Access | Linux shell | Container management |

## Wazuh

| Method | Example | Purpose |
|---|---|---|
| Web Dashboard | `https://LAB_MONITORING_SERVICE` | Security event monitoring |
| System Access | `ssh ADMIN_USER@LAB_SERVICE` | Service troubleshooting |

## Uptime Kuma

| Method | Example | Purpose |
|---|---|---|
| Web Dashboard | `http://LAB_MONITORING_SERVICE` | Service availability monitoring |

## Nextcloud

| Method | Example | Purpose |
|---|---|---|
| Web Interface | `https://LAB_CLOUD_SERVICE` | File management |
| Mobile Client | Nextcloud mobile app | Manual file and photo uploads |

## Remote Lab Access

| Method | Example | Purpose |
|---|---|---|
| Secure Overlay Network | Tailnet client connection | Remote access to lab resources |
| Remote SSH | `ssh ADMIN_USER@TAILNET_NODE` | Secure command-line access |

## Security Note

This repository intentionally avoids publishing:

- real IP addresses
- hostnames
- authentication credentials
- externally reachable service endpoints

The documentation demonstrates **access patterns and administration methods** without exposing operational infrastructure details.
