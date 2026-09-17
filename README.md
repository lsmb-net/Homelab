# Homelab
repo to help organize and document my homelab journey

I am slowly filling the information of this repo, but it will probably be a constant few days behind what I'm actually doing until I get to a good solid basepoint of everything working smoothly.

# Topology
<img width="1112" height="718" alt="Copy of Homelab Topology NODMZ (5)" src="https://github.com/user-attachments/assets/adbbb15e-1067-42f0-8adf-d67962bdbe13" />






# Homelab Server/PCs Overview
PVE1 (Gandalf) is my main workhorse where I host things like wazuh, jellyfin, home assistant, and my dedicated game servers.

PVE2 (Aragorn) is my test rig, and is currently housing my test Active Directory environment. 

PVE3 (Frodo) is currently my router where OPNSense is located. Many of the services I was hosting on PVE2 (Aragorn) were able to be removed as the service or a replacement to the service was integrated into OPNSense.

PVE2 (Aragorn) is where I tested OPNSense and other networking-related services (Adguard Home, nginx) while I waited for PVE3 (Frodo) to be delivered; I was still using a TP-Link AXE75 router during this time, which is now the backup incase anything happens to PVE3 (Frodo). This is currently housing my test Active Directory environment.

# Server/PC SPECS

| Key  | Value - PVE1 | Value - PVE2 | Value - PVE3 |
| ------------- | ------------- | ------------- | ------------- |
| Name  | [Gandalf](https://github.com/lsmb-net/Homelab/tree/9580eba5cd057a2df976c069440da5c4681e75db/Devices/Gandalf%20PC1%5CPVE1)  | [Aragorn](https://github.com/lsmb-net/Homelab/tree/5d870030b4a7309de2dc9ec851bcb84c800ba97b/Devices/Aragorn%20PC2%5CPVE2)  | [Frodo](https://github.com/lsmb-net/Homelab/tree/b134eb719abf142d5d44489ae7068110ea44adc3/Devices/M720q%20Router) |
| Processor  | Intel i5-14600k  | Intel i5-7700k  | Intel i5-8400T |
| Cores/Threads  | 14c/20t  | 4c/8t  | 6c/6t |
| RAM  | 32gb DDR4 | 16GB DDR4 | 32GB SODIMM DDR4 |
| GPU  | nVidia 1660 6GB  | Intel HD Graphics 630 | Intel UHD Graphics 630 |
| Storage 1 | 1TB nVme M.2 SSD  | 1TB nVme M.2 SSD  | 128GB nVme M.2 SSD |
| Storage 2 | 4TB Seagate HDD  | X | X |
| Storage 3 | 128GB nVme M.2 SSD  | X  | X |
| Storage 4 | 128GB Sata SSD  | X  | X | X |
| Storage 5 | 128GB Sata SSD   | X  | X | X |
| Storage 6 | 128GB Sata SSD  | X  | X | X |
| Storage 7 | 128GB Sata SSD  | X  | X | X |
| IP | 192.168.1.73  | 192.168.1.143  | 192.168.1.100 |
| Net Interface 1 | Intel Motherboard Ethernet port  | Killer E2500 Gigabit LAN Port  | Intel Ethernet I219 |
| Net Interface 2 | Intel 1x NIC  | Intel 2x NIC  | Intel 2x NIC  |
| OS | Proxmox 9.2.11  | Proxmox 9.2.11  | Proxmox 9.2.11  |

# VMs and Containers

| Gandalf (PVE1) | Aragorn (PVE2) | Frodo (PVE3) |
| :-------------: | :-------------: | :-------------: |
| [Wazuh-(LXC)](https://github.com/lsmb-net/Homelab/tree/4ff2136ed5298c8b2175eac3379bf0b0ac22fe02/Proxmox/Wazuh%20(LXC)) - 102  | [Home Assistant(LXC)](https://github.com/lsmb-net/Homelab/tree/4ff2136ed5298c8b2175eac3379bf0b0ac22fe02/Proxmox/Home%20Assistant%20(LXC)) - x| [OPNsense](https://github.com/lsmb-net/Homelab/tree/4ff2136ed5298c8b2175eac3379bf0b0ac22fe02/Proxmox/OPNSense) - 700 |
| [Jellyfin](https://github.com/lsmb-net/Homelab/tree/4ff2136ed5298c8b2175eac3379bf0b0ac22fe02/Proxmox/Jellyfin%20(LXC)) - 107 | [Active Directory Test Environment](https://github.com/lsmb-net/Homelab/tree/4ff2136ed5298c8b2175eac3379bf0b0ac22fe02/Proxmox/Active%20Directory)  | x |
| [Frigate(LXC)](https://github.com/lsmb-net/Homelab/tree/4ff2136ed5298c8b2175eac3379bf0b0ac22fe02/Proxmox/Frigate%20(LXC)) - 601  | x| x |
| [Omada Controller(LXC)](https://github.com/lsmb-net/Homelab/tree/4ff2136ed5298c8b2175eac3379bf0b0ac22fe02/Proxmox/Omada%20Controller%20(LXC)) - 702 | x | x |
| [Farming Simulator server (win10)](https://github.com/lsmb-net/Homelab/tree/4ff2136ed5298c8b2175eac3379bf0b0ac22fe02/Proxmox/Dedicated%20Game%20Servers) - 105   | x | x |
| [Minecraft Server (forge) (win10)](https://github.com/lsmb-net/Homelab/tree/4ff2136ed5298c8b2175eac3379bf0b0ac22fe02/Proxmox/Dedicated%20Game%20Servers) - 106 | x  | x |


