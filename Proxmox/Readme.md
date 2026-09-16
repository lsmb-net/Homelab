I use Gandalf for the majority of my VMs, and for any testing I can. I try to keep the workload of Eru light as possible to keep resources available for networking

# VMS/Containers 

| Gandalf (PVE1) | Aragorn (PVE2) | Frodo (PVE3) |
| ------------- | ------------- | ------------- |
| [Wazuh](homelab/proxmox/wazuh/readme.md) - 102  | Home Assistant - x| OPNsense - 700 |
| x | x  | x |
| Frigate - 601  | x| x |
| Omada Controller - 702 | x | x |
| Farming Simulator server (win10) - 105   | x | x |
| Minecraft Server (forge) (win10) - 106 | x  | x |
| Jellyfin - 107 | x  | x |

# SPECS

| Key  | Value - PVE1 | Value - PVE2 | Value - PVE3 |
| ------------- | ------------- | ------------- | ------------- |
| Name  | Gandalf  | Eru  | Frodo |
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


