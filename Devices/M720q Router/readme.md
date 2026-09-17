# Overview

# Specs

Aftermarket (10Gtek) Intel X520-DA2 Dual SFP+ NIC (10G)

Aftermarket (10Gtek) Intel E1GSFPT-A (1.25G RJ45 SFP) -> To Modem (CM1200) *SEE ISSUE #1 FOR THIS TRANSCEIVER *

Aftermarket (10Gtek) SFP+ LC-SR (10G) -> To SFP+ LC port on Switch (HPSWC1)

# Function

This Device (Frodo) only runs OPNsense and functions as the home's router, and the other vms/containers I was planning on running aside it I was able to run inside of with plugins / already apart of OPNsense.
- Wireguard is built into OPNsense
- I replaced Adguard Home with a Unbound DNS with Adguard blocklist, which forwards DNS queries through DNSMASQ, which are both built into OPNsense.
- I was able to remove nginx reverse proxy from a separate VM as it is available as a community-made-plugin. "os-nginx"

# Problems / Solutions
## Problem #1
- For the Dual Intel SFP+ NIC (X520-DA2). Although proxmox, (and opnsense inside of proxmox) could find the port, and there was a status light on the port, no signal would go through the port/transceiver ( one light blinking, other light out). I had read about this when I purchased the NIC / Transceivers, but was too excited when I got my package that I didnt have the information up with me and let my phone die while working on everything (LOL).
  - I swapped everything back to the old set up of the standard 2x RJ45 Intel NIC that I had previously had installed (and knew worked) for the router and therefore internet access could be back up for the night to try again when I had all of the available information with me for the next day.
  - I am swapping the NIC to Aragorn to finish testing there instead of taking the internet down to check. Testing steps will be listed below.
    - I swapped the ports to see if it followed the SFP transceiver (it did)
    - I went through steps found online to allow unsupported SFPs, (which was very odd to me as I bought an intel coded transceiver, but decided to do it anyway.) (no change)
    - I took the SFP transceiver out, and only then did I realize that this was not a 1Gbps Rj45 SFP but a 1.25GB and was working in 1Gbps. I had read that 1.25/2.5/5 will all NOT work with X520-DA2. So i Ordered an Intel coded 10G SFP+ transceiver and will test again after it arrives.
