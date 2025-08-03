# Module 7: The Access Layer

## Section 1: Encapsulation and the Ethernet Frame

The contents of the Ethernet Frame are as follows (keep in mind this is only within a
network):

- Preamble - 7 bytes - Indicates to the destination NIC that an Ethernet Frame is coming.
- Start Frame Delimiter (SFD) - 1 byte - Starts the Ethernet Frame.
- Destination MAC Address - 6 bytes
- Source MAC Address - 6 bytes
- Length / Type - 2 bytes - How long the data field is or what type of data it is (i.e. IPv4)
- Data - 46-1500 bytes - The encapsulated data.
- Frame Check Sequence (FCS) - 4 bytes - Used for destination error checking.

_Encapsulation_ is the process of placing one protocol's message format in another.
For instance, an IPv4 packet can be encapsulated in an Ethernet Frame to allow for addressing
an end device by an IP address.

The Ethernet protocol resides in layer 2 of the OSI model.

## Section 2: The Access Layer

Ethernet Switches operate at layer 2 based on the addressing information of Ethernet frames.
Switches contain MAC Address Tables that correlate each port of the of the switch to a MAC
address (perhaps multiple?).

### MAC Address Tables

A scenario of a switch's MAC Address Table being populated from an empty state is described
below:

1. An Ethernet frame from Host 1 with MAC Address AA-AA to Host 4 with MAC Address DD-DD is
   sent to the Ethernet switch.
2. The switch, seeing as it knows nothing, sees that Host 1's packet came from port 1, so it
   associates port 1 with Host 1's MAC address.
3. The destination MAC address is unknown to the host, an _unknown unicast_, so the switch
   sends the frame to all of its unknown ports (as old ethernet hubs did). 
   Unmatched hosts ignore the packet seeing as its not addressed to them.
   - Apparently, the switch does not get confirmation if the packet was received. So if the
     destination doesn't respond then does the switch continually send packets to all of its
     unknown hosts?

> The switch might send it out all the ports, not just unknown. How do the tables get
> renewed when hosts change?

> Quiz Results: 11/11