# Configuration Management Database (CMDB)

## Physical Infrastructure

| Asset Name | Type | Model | Role | Management IP | Status | Notes |
|---|---|---|---|---|---|---|
| proxmox-920 | Server | Lenovo M920t | Hypervisor |  | Active | Primary VM host |
| macmini-srv | Server | Mac Mini | Docker / Services |  | Active | Hosts containers |
| t14-admin | Laptop | ThinkPad T14 | Admin Workstation |  | Active | Management system |
| attacker-mbp | Laptop | MacBook Pro 2012 | Kali / Attacker |  | Active | Attack simulation |

## Virtual Machines

| VM Name | Host | OS | Role | IP Address | Status | Notes |
|---|---|---|---|---|---|---|
| ubuntu-soc | proxmox-920 | Ubuntu Server | Monitoring target |  | Running | Wazuh agent |
| windows-victim | proxmox-920 | Windows | Test endpoint |  | Planned | For simulations |

## Containers / Services

| Service | Host | Platform | Port | Access Method | Status | Notes |
|---|---|---|---|---|---|---|
| wazuh | macmini-srv | Docker | 443 | Web | Active | SIEM |
| uptime-kuma | macmini-srv | Docker | 3001 | Web | Active | Monitoring |
| nextcloud | macmini-srv | Docker |  | Web / Tailscale | Active | Private cloud |
| portainer | macmini-srv | Docker | 9443 | Web | Active | Container management |
