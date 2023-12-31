# SDN-Summary

Software-Defined Access (SDA):

1. Edge Node to Edge Node: Communication between Edge Nodes in SDA uses the VXLAN protocol for encapsulation. This allows for network segmentation and the creation of scalable overlay networks.

2. Edge Node to Control Plane Node: Edge Nodes communicate with Control Plane Nodes using protocols like PnP (Plug and Play) for device discovery and onboarding, and protocols like LISP (Locator/ID Separation Protocol) and IS-IS (Intermediate System to Intermediate System) for routing information exchange.

3. Edge Node to Border Node: Edge Nodes communicate with Border Nodes using VXLAN for encapsulation and LISP for traffic engineering and policy application.

4. Border Node to Outside Network: Border Nodes communicate with external networks using traditional routing protocols such as BGP (Border Gateway Protocol) or OSPF (Open Shortest Path First). VXLAN encapsulation ends here, and the packet is sent to the external network in its original form.

Software-Defined Wide Area Network (SD-WAN):

1. WAN Edge to WAN Edge: Communication between WAN Edges in SD-WAN uses IPSec VPN tunnels for secure connectivity. This can be over any type of internet connection.

2. WAN Edge to vSmart: The communication between WAN Edge and vSmart devices happens over secure DTLS (Datagram Transport Layer Security) or TLS (Transport Layer Security) connections. They use OMP (Overlay Management Protocol) for route advertisement.

3. vSmart to vSmart: vSmart controllers can communicate with each other over secure connections using protocols like TLS or DTLS for synchronization and load balancing.

4. vSmart to vManage: vSmart controllers communicate with vManage using REST APIs over secure connections. These APIs are used to control and manage the SD-WAN environment.

5. vManage to vManage: vManage instances communicate with each other over secure connections for synchronization and load balancing.

6. vManage to vBond: vManage communicates with vBond using REST APIs over secure connections for orchestration.

7. vManage to vAnalytics: vManage communicates with vAnalytics using REST APIs over secure connections for network monitoring and analysis.

Each of these communications uses secure, encrypted connections to ensure the privacy and integrity of network data.
