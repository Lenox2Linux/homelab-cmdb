# Service Dependencies

This document tracks how major lab services depend on underlying systems, platforms, and network access.

## Proxmox Host

| Service / System | Depends On |
|---|---|
| Proxmox hypervisor | Lenovo M920t hardware |
| Proxmox hypervisor | Lab network connectivity |
| Virtual machines | Proxmox host storage and compute resources |

## Ubuntu Virtual Machines

| Service / System | Depends On |
|---|---|
| Ubuntu VM(s) | Proxmox host |
| Ubuntu VM(s) | Virtual networking |
| Ubuntu VM(s) | Lab router and switch connectivity |

## Docker-Based Services

| Service / System | Depends On |
|---|---|
| Docker services | Mac Mini service host |
| Docker services | Ubuntu Server / Linux host OS |
| Docker services | Network access and open service ports |

## Nextcloud

| Service / System | Depends On |
|---|---|
| Nextcloud | Docker platform |
| Nextcloud | Mac Mini service host |
| Nextcloud | Local lab network or Tailscale remote access |

## Wazuh

| Service / System | Depends On |
|---|---|
| Wazuh server | Docker platform |
| Wazuh server | Mac Mini service host |
| Wazuh monitoring | Wazuh agents installed on monitored systems |
| Wazuh alert visibility | Network communication between agents and server |

## Uptime Kuma

| Service / System | Depends On |
|---|---|
| Uptime Kuma | Docker platform |
| Uptime Kuma | Mac Mini service host |
| Uptime Kuma checks | Reachability of monitored devices and services |

## Tailscale

| Service / System | Depends On |
|---|---|
| Remote access | Tailscale client connectivity |
| Remote access | Tailnet authentication |
| Secure lab access | Reachability of internal systems through Tailscale |

## Dependency Notes

- The Proxmox host supports virtual machines used throughout the lab.
- The Mac Mini supports several Docker-based services.
- The lab router and GS308E switch support communication between devices.
- Tailscale supports remote access without exposing internal services directly to the public internet.
