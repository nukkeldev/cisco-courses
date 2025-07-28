# Getting Started with Cisco Packet Tracer - Notes

## Module 1

### Section 1

This module outlines the basic usage of Cisco Packet Tracer (CPT). CPT is primarily interacted with through one of two modes: logical mode or physical mode.

Logical mode gives an architecture overview of the relationships between devices on a
network, less so to the verbosity of physical mode; which defines the physical linkages
and placement of devices in their respective locations.

Module 1 introduced the software and it's basic usage (i.e. keyboard shorts, where things are, etc.)

It then concluded with a Packet Tracer Tutored Activity (PTTA) titled "Logical and Physical Mode Exploration"
that had me install a back-up router in a network closet and configure it's hostname.

As this software is produced by Cisco, I believe all devices with CLI-capabilities are running an emulated
version of Cisco's Internetworking Operating System (IOS), which has a rather unfortunate acronym.

I've been suprised by the fidelity of specifically physical mode. Being able to interact with all parts of
the devices, from power to the individual ports which I can further connect together with a variety of cabling,
is really impressive in my opinion.

## Module 2

### Section 1

CPT can interact with four types of files:
- `.pka` - A **P**acket **T**racer **A**ctivity that has an instructions window that
  guides the user to solve an initial network into a hidden answer network.
- `.pkt` - The regular CPT file type, can embed media assets.
- `.pksz` - A PTTA file.
- `.pkz` - Deprecated; used to embed media assets before `.pkt` files had the ability to.

### Section 2

In this section, I did the "Create a Simple Network" activity. 
It had us attach a cable modem to an ISP via coaxial, the modem to a wireless router via a 
straight-through copper ethernet cable, then the wireless router to end devices: 
a PC via ethernet and a laptop wirelessly. All of the addressing was resolved via DHCP.

I ran into an odd issue after closing then reopening the file where the PC kept failing DHCP
requests and fell back to APIPA (Automatic Private IP Addressing). I fixed it somehow by either
disconnecting the laptop from the network temporarily or changing the port the PC was connected
to on the wireless router.

Some terms of note:
- `DHCP` - Dynamic host configuration protocol; basically allows the device to negotiate an IP
  address configuration from the router. This must be enabled on the router for it to work.
- `NIC` - Network interface card.
- `Subnet Mask` - Differentiates the network ID and host portions of the IP address. 
- `Default Gateway` - Funnels traffic out of the network.

## Conclusion

I enjoyed this brief course. It was well put together and was fun to do.