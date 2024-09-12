![SettingUpASmallOfficeNetworkGIF](https://github.com/user-attachments/assets/25cc86e3-3d84-4d44-ba50-0d626acd4fc4)


# Network Address Translation

**NAT** (Network Address Translation) is a technique used to conserve IP addresses and to hide the internal network from the outside world. When a router uses NAT to forward packets to a specific IP address inside a private network, it follows these steps:

1. **Packet Arrival**: A packet arrives at the router from the internet, containing a source IP address (from the internet) and a destination IP address (the public IP address of the router).
2. **NAT Lookup**: The router consults its NAT table to find the corresponding private IP address associated with the public IP address.
3. **Packet Modification**: The router modifies the destination IP address in the packet to the private IP address found in the NAT table.
4. **Packet Forwarding**: The router forwards the modified packet to the internal network, where it is routed to the specific device with the private IP address.
5. **Return Path**: When a response packet is sent from the internal device back to the router, the router again consults its NAT table to find the corresponding public IP address. It modifies the source IP address in the response packet to the public IP address and forwards the packet back to the internet.

This process allows the router to effectively translate between public and private IP addresses, ensuring that packets reach their intended destinations within the private network while protecting the internal network from direct access from the internet.
