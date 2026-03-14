# Asset Inventory

This document provides a higher-level inventory of physical devices and infrastructure roles within the lab.

## Physical Devices

### Lenovo M920t
- Asset Name: LAB_SERVER
- Type: Small form factor workstation / server
- Role: Proxmox hypervisor host
- Purpose: Hosts virtual machines for security and infrastructure testing
- Network Placement: Lab network
- Notes: Primary virtualization platform

### Mac Mini
- Asset Name: LAB_SERVICE
- Type: Small form factor service host
- Role: Docker and service platform
- Purpose: Hosts Wazuh, Nextcloud, Uptime Kuma, Portainer, and related services
- Network Placement: Lab network
- Notes: Central service platform for self-hosted tools

### ThinkPad T14
- Asset Name: LAB_ADMIN
- Type: Laptop
- Role: Administrative workstation
- Purpose: SSH management, web administration, documentation, Git/GitHub work
- Network Placement: Personal network and lab management access
- Notes: Main operator system

### MacBook Pro 2012
- Asset Name: LAB_ATTACK
- Type: Laptop
- Role: Attack simulation system
- Purpose: Kali Linux testing, Nmap scans, traffic generation, offensive security practice
- Network Placement: Lab network
- Notes: Used to simulate attacker activity in the home lab

### AX3200 Router
- Asset Name: HOME_ROUTER
- Type: Router
- Role: Personal / primary network router
- Purpose: Supports non-lab home network connectivity
- Network Placement: Personal network
- Notes: Separate from isolated lab environment

### AX50 Router
- Asset Name: LAB_ROUTER
- Type: Router
- Role: Lab network gateway
- Purpose: Segments lab traffic from personal/home traffic
- Network Placement: Lab network
- Notes: Supports isolated security testing environment

### Netgear GS308E
- Asset Name: LAB_SWITCH
- Type: Managed switch
- Role: Layer 2 network switching
- Purpose: Connects lab systems to the lab network
- Network Placement: Lab network
- Notes: Supports switch-level documentation and future VLAN-style learning

## Virtual Infrastructure

### Ubuntu Virtual Machine(s)
- Asset Name: LAB_VM
- Type: Virtual machine
- Role: Server and monitoring targets
- Purpose: Linux administration, SSH practice, monitoring agent deployment, service testing
- Host Platform: Proxmox
- Notes: Used for multiple lab scenarios

### Windows Virtual Machine(s)
- Asset Name: LAB_WINDOWS_VM
- Type: Virtual machine
- Role: Test endpoint / victim machine
- Purpose: Security simulations, logging, monitoring, and blue-team practice
- Host Platform: Proxmox
- Notes: Supports future investigation and attack/defense exercises

## Asset Inventory Notes

- This repository uses sanitized naming conventions for public documentation.
- Real IP addresses, credentials, and identifying details are intentionally excluded.
- This inventory is designed to reflect enterprise-style asset documentation practices.
