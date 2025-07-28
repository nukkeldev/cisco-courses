# Exploring Networking with Cisco Packet Tracer - Notes

## Module 1

### Section 2

Rack-mounted patch panels give jack points for cabling coming from the end devices
via wall mounts. The wall mount has port N connected to the end device and then punch
down N to the patch panel punch down N, which corresponds to jack N on the panel.

#### Activity 1.1.4

I completed 1.1.4 per the instructions but it said the Default Gateway for Office-Admin was incorrect. The web server that specifies the gateway as 0.0.0.0 for its static IP of 192.168.20.1, which was the Default Gateway assigned by DHCP on Office-Admin, yet it still refused
that answer. Even when checking 1.1.6 which had the solution to 1.1.4 as it starting point it
was still 192.168.20.1 :(.

#### Activity 1.1.6

This activity was straightforward. We had to connect Laptop to the office's WLAN, as well as
change it to use DHCP to remedy the same issue we had in the previous activity. Then we connected
a tablet and speaker together via Bluetooth and tether another Laptop to a smartphone's cellular
connection also over Bluetooth.

#### Using the CLI

- All commands in PT's "Config" tabs show the IOS commands below.
- To access the CLI from an end device, as we did in getting started, use an RS232 or USB cable
  then open a terminal emulator with the proper settings.
- Devices load IOS first, then load saved settings.
- The default mode is "User Exec" mode for monitoring purposes.
- Calling `enable` moves the shell into "Privileged" mode.
- `?` shows a help output.
- When in privileged mode, you can start configuring the device with `configure terminal`
  - Any modifications are initially only applied to the running configuration in memory.
  - To persist the configuration run `copy running-config startup-config`.

For devices that need to be pre-configured and don't have an active network connection,
console configuration is a convenient way to access the device.

#### Activity 1.1.8

Fortunately this one was my cup of tea. We had to change a few configurations on a new
switch for the office and did so through the IOS CLI. Basically we just did as was stated
in the informational section above.

## Module 2

### Section 1

Simulation mode allows the user to step through time and inspect each PDU (Protocol Data Unit)
as it goes through the network.

The PDU and Complex PDU tools at the end of the toolbar allow for users to manually send, or
schedule, PDUs to be sent from devices.

#### Activity 2.0.3

- Basic inspection of ICMP and ARP PDUs as well as manual creation of them using tooling.

#### Topology Annotation

Logical mode can be annotated with various shapes, media, and notes.

#### Activity 2.0.7

- I connected a new switch to the previous one through a straight-through through gigabit ports.
- Connected port 1 of the new switch to a patch panel port then connected it to a new PC in the office through a wall mount.
- I then added a second home network with a PC, Home Gateway, and Cable Modem.

### Section 2

