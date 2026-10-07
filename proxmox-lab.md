# 🖥️ Proxmox VE Homelab

## 🎯 Objective
Deploy and configure a Type-1 hypervisor environment to host multi-tier infrastructure, virtual switches, and isolated guest networks.

## 🛠️ Configuration Steps
1. **Hypervisor Deployment:** Installed Proxmox VE, configuring local storage pools (ZFS/LVM) and managing node network interfaces.
2. **Virtual Bridge Setup:** Created dedicated Linux Bridges (`vmbr0` for WAN/Management, `vmbr1` for internal VLAN trunks) to handle virtual machine traffic separation.
3. **Resource Allocation:** Provisioned virtual machines and Linux containers (LXC) for core services, balancing CPU cores, memory limits, and disk storage.
4. **Backup & Snapshot Strategy:** Configured automated Proxmox Backup Server (PBS) integration and manual snapshot checkpoints prior to major configuration changes.

## 🔍 Verification & Testing
* Verified node accessibility and resource health metrics via the Proxmox Web UI dashboard.
* Tested inter-VM connectivity and confirmed that virtual bridge rules successfully isolated guest traffic from the management network.
