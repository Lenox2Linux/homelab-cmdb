\# Lab Network Architecture



```mermaid

flowchart TD



Internet\[Internet]

HomeRouter\[HOME\_ROUTER]

LabRouter\[LAB\_ROUTER]

Switch\[LAB\_SWITCH - GS308E]



Admin\[LAB\_ADMIN - ThinkPad T14]

Service\[LAB\_SERVICE - Mac Mini]

Server\[LAB\_SERVER - Proxmox Host]

Attack\[LAB\_ATTACK - Kali System]



VM1\[LAB\_VM - Ubuntu]

VM2\[LAB\_WINDOWS\_VM - Windows]



Internet --> HomeRouter

HomeRouter --> LabRouter

LabRouter --> Switch



Switch --> Admin

Switch --> Service

Switch --> Server

Switch --> Attack



Server --> VM1

Server --> VM2

