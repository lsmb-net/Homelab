# Overview
## Firewall
## Interfaces
## VLANs
# Services
## Outbound DNS
## Wireguard
## nginx
## DNSMASQ + DHCP
# Specs
# Function

# Problems/ Solutions

## Problem #1
- I had tested OPNsense behind a router before deploying it. The previous gateway was 192.168.0.1 and opnsense's was 192.168.1.1. I had my cluster removed from each other, but still in a cluster (all had new ips), gateway and DNS settings were now wrong having no devices hit the internet
  - 1.) I fixed the IP addresses for the proxmox nodes/network adapters for proxmox
    - "nano /etc/network/interfaces" and "nano /etc/hosts"
    - as well as for the network ports/bridges for each proxmox node
    - Correcting IPs to new subnet of 192.168.1.x for their IP addresses
  - 2.) Next was removing all of the old cluster info so they could be rejoined together.
    - stop corosync and cluster services "systemctl stop pve-cluster corosync"
    - Start in localmode "pmxcfs -l"
    - remove the configs "rm -f /etc/pve/corosync.conf" and "rm -rf /etc/corosync/*"
      -(also went in with winscp and verified this, cleaning up any remaing pieces of other nodes)
    - stop localmode "killall pmxcfs"
    - restart service "systemctl start pve-cluster"
      - I was still not fully able to join the nodes back together because you cant join nodes that have VMs on it, so I had to back up the VMs/Containers, remove them, join cluster, and then restore them from the backup.
  - 3.) The DNS issues I was having was from everything being pointed to 192.168.0.85, which was previously my Adguard Home server ran on PVE1(Gandalf), but it now had a new IP. Instead of using this server again I decided to give the DNS options available on OPNsense a try and went with Outbound DNS
