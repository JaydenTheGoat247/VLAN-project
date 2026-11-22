VLAN (Virtual Local Area Network)

A VLAN is a logical grouping of devices on a network that behaves as if they were on their own separate physical LAN, even when they share the same switches and cabling. Instead of dividing a network by physical location, VLANs let you divide it by function, department, or security needs.

How it works

Switches assign each port (or device) to a VLAN, identified by a number from 1 to 4094. Devices in the same VLAN can talk to each other directly at Layer 2, while traffic between different VLANs must pass through a router or a Layer 3 switch (called inter-VLAN routing). When traffic for multiple VLANs travels over a single link between switches, the frames are labeled with a VLAN ID using the IEEE 802.1Q tagging standard. Such a link is called a trunk.

Key benefits

Security: Sensitive systems (finance, servers, guest Wi-Fi) are isolated from the rest of the network.
Smaller broadcast domains: Broadcast traffic stays within its VLAN, which reduces congestion and improves performance.
Flexibility: Users can be grouped logically regardless of where they sit in the building, and moving a device only requires a configuration change.
Easier management: Policies, QoS, and access controls can be applied per VLAN.
Cost savings: One physical switch can serve multiple separate networks, so less hardware is needed.

Common VLAN types

Data VLAN: Carries normal user traffic.
Voice VLAN: Prioritizes IP phone traffic.
Management VLAN: Used to access and configure network devices.
Native VLAN: Carries untagged traffic on a trunk.
Default VLAN: VLAN 1 on most switches, where all ports start out.

Simple example

A company might place Sales on VLAN 10, HR on VLAN 20, and Guests on VLAN 30. All three groups plug into the same switches, but Sales cannot see HR traffic unless a router explicitly allows it.
