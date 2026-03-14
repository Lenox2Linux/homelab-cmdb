# Network Topology

## ASCII Diagram

```text
Internet
   │
ISP Modem
   │
AX3200 Router (Personal Network)
192.168.1.0/24
   │
   │
AX50 Router (Lab Network)
192.168.50.0/24
   │
   │
GS308E Managed Switch
   │
   ├── ThinkPad T14 (Admin / Management)
   │
   ├── Mac Mini (Ubuntu Server)
   │      ├── Docker
   │      ├── Wazuh
   │      ├── Portainer
   │      ├── Uptime Kuma
   │      └── Nextcloud
   │
   ├── Lenovo M920t (Proxmox Host)
   │      ├── Ubuntu VM
   │      ├── Windows VM (Victim)
   │      └── Future VMs
   │
   └── MacBook Pro 2012 (Kali Attacker)
