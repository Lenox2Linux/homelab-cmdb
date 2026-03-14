# Configuration Management Database (CMDB)

## Physical Infrastructure

|Asset Name|Type|Model|Role|Management IP|Status|Notes|
|-|-|-|-|-|-|-|
|LAB\_SERVER|Server|Lenovo M920t|Hypervisor|Sanitized|Active|Primary VM host|
|LAB\_SERVICE|Server|Mac Mini|Docker / Services|Sanitized|Active|Hosts containers|
|LAB\_ADMIN|Laptop|ThinkPad T14|Admin Workstation|Sanitized|Active|Management system|
|LAB\_ATTACK|Laptop|MacBook Pro 2012|Kali / Attacker|Sanitized|Active|Attack simulation|
|LAB\_ROUTER|Router|TP-LINK AX50|Lab Gateway|Sanitized|Active|Isolated lab network router|
|LAB\_SWITCH|Managed Switch|Netgear GS308E|Layer 2 Switching|Sanitized|Active|Distributes lab network connections|

## Virtual Machines

|VM Name|Host|OS|Role|IP Address|Status|Notes|
|-|-|-|-|-|-|-|
|LAB\_VM|LAB\_SERVER|Ubuntu Server|Monitoring target|Sanitized|Running|Wazuh agent / Linux administration|
|LAB\_WINDOWS\_VM|LAB\_SERVER|Windows|Test endpoint|Sanitized|Planned|Future security simulations|

## Containers / Services

|Service|Host|Platform|Port|Access Method|Status|Notes|
|-|-|-|-|-|-|-|
|Wazuh|LAB\_SERVICE|Docker|Sanitized|Web|Active|SIEM|
|Uptime-Kuma|LAB\_SERVICE|Docker|Sanitized|Web|Active|Monitoring|
|nextcloud|LAB\_SERVICE|Docker|Sanitized|Web / Tailnet|Active|Private cloud|
|portainer|LAB\_SERVICE|Docker|Sanitized|Web|Active|Container management|



