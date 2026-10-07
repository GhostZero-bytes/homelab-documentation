# 🌐 pfSense Firewall & Network Segmentation Lab

## 🎯 Objective
Configure an advanced software firewall to handle routing, firewall rules, and network segmentation for a SOHO environment.

## 🛠️ Configuration Steps
1. **Initial Deployment:** Installed and configured pfSense on virtualized hardware using Proxmox VE.
2. **Interface Setup:** Defined WAN and LAN interfaces, establishing internal private subnets.
3. **Firewall Rules:** Implemented explicit stateful packet inspection rules to restrict inter-VLAN traffic and secure management access.
4. **Remote Access:** Configured secure tunneling options (OpenVPN / Tailscale) for external administrative access.

## 🔍 Verification & Testing
* Tested internal routing between subnets to verify that firewall block rules successfully isolated guest/IoT traffic from core infrastructure.
* Confirmed stable external connectivity and active VPN handshake sessions.
