# CCNA
Study Material in preparation for the CCNA Certification.
# 1.0 Network Fundamentals
## 1.1 Explain the role and function of network components 
### 1.1a Routers
Routers facilitate communication between different networks. Routers connect networks, route data packets between them, enforce security policies, optimize traffic flow, and provide various other critical functions to ensure efficient and reliable communication across interconnected networks.
### 1.1.b Layer 2 and Layer 3 Switches
Layer 2 switches primarily operate at the Data Link layer (Layer 2) of the OSI model, focusing on MAC addresses and Ethernet frames. They are essential for LAN connectivity, MAC address learning, and VLAN support.

Layer 3 switches operate at both the Data Link layer (Layer 2) and the Network layer (Layer 3). They provide additional functionality such as IP routing, inter-VLAN routing, and support for routing protocols. Layer 3 switches are more versatile and suitable for larger networks requiring routing capabilities.
### 1.1.c Next-generation firewalls and IPS
Next-generation firewalls and Intrusion Prevention Systems (IPS) are critical for modern network security.

Next-Generation Firewalls (NGFW) combine traditional firewall capabilities with more sophisticated detection and prevention technologies to address a broader range of security threats. 
    - Application Awareness & Control: identify and control applications regardless of port, protocol, or encryption method
    - Integrated Intrusion Prevention System (IPS): built-in IPS functionality to detect and prevent network threats
    - Advanced Threat Protection: offers advanced protection features like sandboxing, which allows suspicious files to be executed in a controlled environment to observe their behavior and detect advanced malware and zero-day exploits.
    - SSL/TLS Inspection: inspect encrypted traffic by decrypting SSL/TLS connections.
    - User Identity Awareness: enforce policies based on user identity rather than just IP addresses.
    - Content Filtering and Data Loss Prevention (DLP): filer web content and prevent access to malicious or inappropriate websites.
    - Threat Intelligence Integration: integrate with threat intelligence services to receive real-time updates on emerging threats, ensuring that the firewall can recognize and block the latest attack methods.
Intrusion Preventing System (IPS) is focused on detecting and preventing network threats in real-time. It is designed to monitor network traffic and take immediate action to block or mitigate malicious activity. 
    - Traffic Monitoring and Analysis: continuously monitors network traffic for signs of malicious activity.
    - Threat Detection and Prevention: take various actions such as dropping malicious packets, blocking traffic from specific IP addresses, resetting connections, or alerting network administrators.
    - Signature-Based Detection: relies on a database of known attack signatures to detect threats.
    - Anomaly-Based Detection: can detect unusual patterns in network traffic that may indicate a new or unknown attack.
    - Protocol Analysis: can analyze network protocols to ensure they conform to expected behavior.
    - Integration with Security Ecosystem: can integrate with other security devices and systems, such as firewalls, SIEM (Security Information and Event Management) systems, and endpoint protection solutions, to provide a coordinated response to threats.
NGFWs and IPS work together to provide layered security. NGFWs may handle application control, SSL inspection, and basic IPS functions, while dedicated IPS devices can provide deeper inspection and more granular control over network traffic.
### 1.1.d Access points
Access points (APs) enable devices to connect to a network wirelessly, providing mobility and flexibility for users usually in wireless local area networks (WLANs).
    - Wireless Connectivity to devices
    - Network Extension: connect to wired network and provide signal to areas where cabling is impractical
    - Client Mobility: Users can move around within the coverage area of multiple access points
    - Radio Signal Transmission: transmit and receive radio frequency (RF) signals
    - Network Bridging: bridge between wireless and wired networks
    - SSID Broadcasting: SSID names identify the wireless network for clients to find and connect
    - Authentication & Security: enforce network security to protect against unauthorized access (Wi-Fi Protected Access 2 & WPA3)
    - Traffic Management: manage the flow of data between wireless clients and the network
    - Quality of Service (QoS) - prioritize types of traffic to ensure critical applications receive sufficient bandwidth and reduce latency
    - Mesh Networking: multiple APs form a network of interconnected nodes for dynamic route optimization and redundancy, which enhances coverage and reliability
### 1.1.e Controllers (Cisco DNA Center and WLC)
Controllers like Cisco DNA Center and Wireless LAN Controllers (WLC) provide centralized control, automation, monitoring, and optimization of network resources.

Cisco DNA Center is a network management and command center for Cisco's Digital Network Architecture (DNA). It provides a comprehensive solution for managing and automating network operations, enhancing visibility, and ensuring network security.
    - Network Automation: supports Zero-Touch Provisioning (ZTP) and configuration of new devices
    - Policy-based Management: centralized approach for network policies
    - Assurance & Analytics: real-time monitoring and analytics for network performance and reliability
    - Network Segmentation: supports Software-Defined Access (SD-Access) to enhance security by isolating segments of the network
    - Security Integration: integrates with security tools for threat detection and migitation 
    - Application Visibility & Control: detailed visibility into application performance and user experience
    - Simplified Management: unified interface for wired and wireless networks

Wireless LAN Controllers (WLC) are responsible for centralizing the management and control of wireless access points (APs) in a network. They provide a single point of control for all APs, ensuring consistent configuration, security, and performance across the wireless network.
    - Centralized Management: manage multiple APs from a single interface
    - Dynamic RF Management: automatically adjusting channel assignments and power levels of APs to minimize interference and maximize coverage
    - Seamless Routing: client roaming between APs within the same network
    - Enhanced Security: enforce security policies across all managed APs
    - Quality of Service (QoS): prioritize traffic to ensure critical applications receive the necessary bandwidth and low latency
    - Guest Access Management: guest access solutions allowing visitors to connect to the netwrok securely witout accessing sensitive internal resources
    - Monitoring & Troubleshooting: real-time monitoring and troubleshooting of wireless network
    - Scalability: manage a large numbers of APs making them suitable for enterprise environments

Cisco DNA Center provides a holistic management solution for both wired and wireless networks, focusing on automation, policy-based management, and advanced analytics.
WLCs specifically manage wireless networks, providing centralized control over APs and ensuring seamless wireless connectivity and security.
Cisco DNA Center can integrate with WLCs to provide a unified management platform for both wired and wireless networks. This integration allows for comprehensive network visibility, policy enforcement, and automation across all network segments.
### 1.1.f Endpoints
Endpoints refer to devices that connect to and interact with the network. These devices are critical as they are the primary points of access for users and applications to interact with network services and resources. 
    - User Interaction: how users interact with the network
    - Data Generation & Consumption: produce data that is transmitted across the network and receive data from other network devices
    - Network Edge Participation: help to determine the network's edge performance and security
    - Communication & Collaboration: between devices
    - Application Access: provide access to various apps and services
    - Data Input & Output
    - Security Enforcement: run security software like antivirus programs, firewalls, and endpoint protection platforms (EPP)
    - Device Management & Monitoring: software updates, configuration management, and performance monitoring 
    - Resource Utilization: utilize resources like bandwidth, storage, and processing power
    - Peripheral Connectivity

### 1.1.g Servers
Servers provide various services and resources to client devices. They are powerful computers designed to manage, store, process, and deliver data to other computers (clients) over a network. 
    - Centralized Resource Management
    - Data Storage & Management
    - Application Hosting: allows multiple users to access and use applications simultaneuosly
    - Network Control Management: user authentication, network configuration, & resource allocation
Features
    - File & Print Services
    - Web Hosting
    - Database Management
    - Email Services
    - Application Services
    - Authentication & Authorization
    - Virtualization
    - Backup & Recovery
    - Remote Access
    - Monitoring & Management
Types of Servers
    - Dedicated Servers: dedicated to a single task or service
    - Virtual Servers: virtualized instances of servers running on a physical host
    - Cloud Servers: accessible over internet 
    - Blade Servers: modular servers that fit into a chassis
### 1.1.h PoE
Power over Ethernet (PoE) allows ethernet cables to carry electrical power in addition to data. This innovation simplifies network design and reduces the need for additional power supplies and outlets.
    - Simplified Cabling 
    - Cost Reduction
    - Flexibility & Scalability
    - Enhanced Network Reliability: can be backed up by uninterruptible power supplies (UPS) ensuring that devices remain operational during outages
Functions
    - Power Delivery: over Cat5e and above
    - Data Transmission
    - Device Compatibility: APs, IP Cameras, VoIP phones, network switches, IoT devices
    - Power Management

### OSI Model
Physical Layer (Layer 1) - deals with the physical aspects of transmitting data over a physical medium, such as cables, fibers, or wireless signals. It defines characteristics like voltage levels, data rates, physical connectors, and transmission distances. Ex. Network Interface Cards (NICs), hubs, repeaters
Data Link Layer (Layer 2) - handles the reliable transmission of data frames between nodes on a network segment. It provides error detection and manages access to the physical medium and controls data flow. Ex. Switches, bridges
Network Layer (Layer 3) - responsible for routing packets across different networks to their destination based on logical address (IP addresses). It determines the optimal path for data transmission and handles addressing, routing, and traffic control. Ex. Routers, Layer 3 switches
Transport Layer (Layer 4) - ensures reliable and efficient data transfer between end systems. It breaks down large messages into smaller segments, manages acknowledgment and retransmission of lost data, and ensures data integrity. Ex. TCP (Transmission Control Protocol), UDP (User Diagram Protocol)
Session Layer (Layer 5) - establishes, manages, and terminates sessions between applications on different devices. It handles syncronization, checkpointing, and recovery of data exchange sessions. Ex. Session establishment, maintenance, and termination. Ex. Session establishment, maintenance, and termination
Presentation Layer (Layer 6) - ensures that data is presented in a format that the application layer can understand. It handles data compression, encryption, and decryption to provide data security and privacy. Ex. Data encryption, compression, and format conversion
Application Layer (Layer 7) - provides network services directly to end-user applications. It supports communication services for applications like email, web browsing, file transfer, and remote access. Ex. HTTP, FTP, SMTP, SSH