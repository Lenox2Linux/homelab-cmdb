# Network Addressing (Sanitized Example)

## Network Segments

| Network Name | CIDR Range | Purpose |
|---|---|---|
| LAB_NET | 192.168.x.0/24 | Home lab systems |
| MGMT_NET | 10.x.x.0/24 | Management network |
| VPN_NET | 100.x.x.x | Tailscale overlay network |

## Example Device Assignments

| Device | Address | Role |
|---|---|---|
| LAB_ROUTER | 192.168.x.1 | Lab gateway |
| LAB_SWITCH | 192.168.x.2 | Managed switch |
| LAB_SERVER | 192.168.x.10 | Virtualization host |
| LAB_SERVICE | 192.168.x.20 | Service server |

Note: Real addressing is intentionally not published.
