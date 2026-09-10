# CURRENT
Updates from previous version
- I was given a 42u rail kit (front and back mount, U shape instead of L shape) from my work.
    - I moved the old rails to the back of the rack to mount storage shelves, PDUs, ETC.
- Bought a M720Q Tiny
    - Using spare parts I had lying around It now has 16gb DDR4 SODIMM ram, 6c/6t 8400t, and 128GB M.2 SSD.
    - I bought a m720q riser and 2 port Intel NIC card as this will be used as my router.
- Moved the Server rack down to the basement (more room to work with and much lower year round temperature)
    - As the basement can periodically flood, I installed wheels onto the bottom of the server rack, which required me to shorten the frame down a bit to fit in the basement.
- Moved the modem, old router and all of the cabling (old runs and the coax cable in from ISP) into this section of the basement
- Closed the Server rack's sides with cabinet-grade plywood 1/4"
- Replaced the old router (TP-LINK AXE75) with the Lenovo m720q Tiny running OPNSense inside of a Proxmox node(Frodo)
  - I replaced the Wi-Fi function of the router with two TP-Link Omada APs; EAP225(Indoor) and Eap603(Outdoor)
    - At the time of writing this, they are both set up but not placed in their final positions, 225 = Main floor on top of bookshelf, 603 Outside of back end of house.

| Server Rack Layout  |
| :-------------: |
| 2u Solid Cover plate <br><br> |
| 1u 7 port PDU (PDU1)  |
| 1u Solid Cover plate  |
| 1u 7 port PDU (PDU2) |
| 1u Solid Cover plate  |
| 24 Port Patch Panel (Patch1/P1)  |
| HP 2530-24G J9854A (PoE+, SFP+)
| Cisco 3750x |
| Unmanaged 24port TP Link switch  |
| 24 Port Patch Panel (Patch2/P2)  |
| <br><br><br> 7U Shelf for Modem + M720q Router <br><br><br><br> |
| 1u Open shelf for Camera NVR system / keyboard + mouse  |
| 1u Brush plate |
|<br> 3U PC case (GANDALF) <br><br> |
| 1u Brush plate |
|<br> 3U PC case (Aragorn(previously Eru)) <br><br> |
|<br> 2 2u vented cover plates, shelf behind/ under open spot for UPS  <br><br><br>|
|<br> 3u Cover plate <br><br> |
|<br> 3u vented panel with intake fans <br><br> |
|<br> 3u vented panel with intake fans <br><br> |
| 2u Solid Cover plate <br><br> |

# BUILD
-I built a 42u rack server rack out of 2x4s and one-side-finished plywood. 

-I was in between purchasing a used 42u rack, or building; But because of cost and transporting of a full sized server rack, I decided to go with just building it.

-I built the frame first with a shelf for my personal PC and Gandalf (Which was still running Windows 10 and VMWare Workstation at the time). The materials for the frame cost around 100$, and I already had all of the tools to build it.

-Material list was 6 2x4s and one 4x4 sheet of ply, one box of Torx head construction screws, and a 12u rack rail kit.

# Version 1
<img width="150" height="400" alt="First Server Rack version" src="https://github.com/user-attachments/assets/b56ea93b-79c8-46b0-aee2-6774764df645" />

-I was keeping my Patch cables plugged into patch panel + Switch to keep from losing or damaging them.

-The Mini-PCs were not functional and I ended up returning them as I had plenty of spare PC parts from previous upgrading of my family and I's PCs

-This first version was built to the size of a 42u so that i could expand it to that size if needed/when funds allowed it.

The shelf had both of my Pcs on it.
| Server Rack Layout  |
| :-------------: |
| Shelf for PCs (above rack rails) |
| Camera NVR + Audio Interface   |
| 24 Port Patch Panel  |
| Unmanaged 24port TP Link switch  |
| 7 Plug PDU  |
|<br><br> 5u Shelf for audio equpiment <br><br><br>|
| 1U Shelf for Mini-PCs |
| 2u Shelf for storage <br><br> |


# Version 2
Changes
- I bought an old Cisco Catalyst 3750x Layer 3 switch

  -- I read complaints about the fan noise, but didn't think an issue of it as I normally have fans on in the room 24/7 and enjoy the white noise.
  
  -- However I did not realize the amount of heat that this switch would generate even with 0 PoE Devices or PoE enabled. I ended up keeping this switch to have for practice/testing with a cisco switch but purchased a different managed switch not long after.
  
- Purchased 7 port PDU with voltage/amperage display.

- Purchased 2x brush plates to help clean up cabling.

- Purchased a 20u rack rail kit (Now at 32U total)

- Took Gandalf out of normal desktop PC case and into a test bench case (already owned) with [3d printed brackets](https://makerworld.com/en/models/2766625-rack-ears-for-joyjom-open-air-pc-case?from=search#profileId-3072342) to rack mount it. (Mounted my other open case too, but didnt put pc in at this time)
  
- 3D Printed a few [Rack Cover Plates.](https://makerworld.com/en/models/2961946-6-10-19-rack-panel-generator-blank-vented?from=search#profileId-3370217)

<img width="150" height="400" alt="Second Server Rack Version" src="https://github.com/user-attachments/assets/70a019ca-d34f-4c95-b3ce-085d4bf73175" />

| Server Rack Layout  |
| :-------------: |
| 2u Cover plate <br><br> |
| 1u 7 port PDU  |
| 1u Open for Camera NVR system  |
| Unmanaged 24port TP Link switch  |
| Cisco 3750x |
| 24 Port Patch Panel  |
| 7 Plug PDU (Display Screen)  |
|<br> 3u Shelf for audio equpiment <br><br> |
|<br> 4U PC case (GANDALF) <br><br><br> |
| 1u Brush plate |
| 1u shelf with Audio interface |
| 1u Brush plate |
|<br> 3U PC case (EMPTY) <br><br> |
|<br> 3u Cover plate <br><br> |
|<br> 3u Storage Shelf <br><br> |
| 2u Cover plate <br><br> |
| Audio equipment stored below |
