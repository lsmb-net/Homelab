# Homelab
repo to help organize and document my homelab journey

# Topology
Putting photo of network topology here.

# Homelab Server/PCs
PVE1 (Gandalf) is my main workhorse where I host things like wazuh, jellyfin, home assistant, and my dedicated game servers.

PVE2 (Aragorn) is my test rig, and is currently housing my test Active Directory environment. 

PVE3 (Frodo) is currently my router where OPNSense is located. Many of the services I was hosting on PVE2 (Aragorn) were able to be removed as the service or a replacement to the service was integrated into OPNSense.

PVE2 (Aragorn) is where I tested OPNSense and other networking-related services (Adguard Home, nginx) while I waited for PVE3 (Frodo) to be delivered; I was still using a TP-Link AXE75 router during this time, which is now the backup incase anything happens to PVE3 (Frodo). This is currently housing my test Active Directory environment.

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
| IP | 192.168.0.73  | 192.168.0.143  | 192.168.0.150 |
| Net Interface 1 | Intel Motherboard Ethernet port  | Killer E2500 Gigabit LAN Port  | Intel Ethernet I219 |
| Net Interface 2 | Intel 1x NIC  | Intel 2x NIC  | Intel 2x NIC  |
| OS | Proxmox 9.2.11  | Proxmox 9.2.11  | Proxmox 9.2.11  |



