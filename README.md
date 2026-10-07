# 🛠️ SOHO Infrastructure & Virtualization Lab

## 🎯 Objective
To design, deploy, and administer an enterprise-grade Small Office/Home Office (SOHO) network and virtualization environment, focusing on strict network segmentation, secure remote access, and robust identity services.

## 🧱 Core Technology Stack
* **Hypervisor:** Proxmox VE (Virtual Environment)
* **Firewall & Routing:** pfSense (Stateful packet inspection, VLAN segmentation, OpenVPN, Tailscale)
* **Directory Services & OS:** Windows Server (Active Directory Domain Services, DNS, DHCP)
* **Administration & Tooling:** PowerShell, Bash, PuTTY (SSH)

## 📐 Architecture & Network Layout
*(Briefly describe how your lab is connected. Example below:)*
* **Physical Edge:** ASUS router passing connection downstream to managed switches and the Proxmox hypervisor node.
* **Virtualization Host (Proxmox VE):** Hosts core network services and domain controllers as isolated virtual machines.
* **Firewall Gateway (pfSense):** Acts as the primary router/firewall handling inter-VLAN routing and firewall rules.

## 🚀 Key Implementations
* **Virtualization & Resource Management:** Deployed and managed virtual machines and containers on Proxmox VE, allocating hardware resources efficiently.
* **Network Security & Routing:** Configured pfSense interfaces, established firewall rules to isolate guest and management traffic, and set up secure remote access via OpenVPN and Tailscale.
* **Identity & Access Management:** Built out a Windows Server Active Directory domain environment, configuring DNS zones, DHCP scopes, and user/group policies.

## 🔍 Troubleshooting & Lessons Learned
* *Challenge:* Resolving internal DNS resolution issues between virtual subnets across the firewall.
* *Solution:* Configured proper forwarding rules and DNS overrides within pfSense and Windows Server DNS to ensure seamless domain joining.
