Enterprise Network Security Lab



Project Overview



This project is a complete simulation of a small enterprise network environment designed to demonstrate practical networking, system administration, and security monitoring skills. The lab integrates Cisco Packet Tracer for network design and Oracle VM VirtualBox running Ubuntu Server for real-world system deployment and hardening. The primary goal of this project was to simulate how an organization builds, secures, and monitors its internal infrastructure while maintaining segmentation and visibility across the network.



The lab reflects the practical responsibilities of a SOC Analyst or Network Security Analyst, including network configuration, server hardening, intrusion detection deployment, firewall configuration, and log analysis.



Enterprise Network Design



The network architecture was first designed in Cisco Packet Tracer to simulate a small enterprise environment. The topology consists of a router acting as the default gateway, a Layer 2 switch for internal connectivity, multiple end-user PCs representing different departments, and a centralized server.



An IP addressing scheme based on the 192.168.1.0/24 network was implemented. The router was configured with the gateway address 192.168.1.1, and end devices were assigned static IP addresses within the subnet. Connectivity between all devices was validated using ICMP ping tests to ensure proper routing and switching functionality.



This phase demonstrates understanding of IP addressing, routing configuration, interface management, and end-to-end connectivity validation.



VLAN Segmentation and Network Isolation



To simulate a realistic enterprise environment, VLAN segmentation was implemented on the switch remembering that organizations separate departments to improve security and reduce broadcast domains.



Two VLANs were created:



VLAN 10 for the HR department



VLAN 20 for the IT department



Switch ports were manually assigned to their respective VLANs using access mode configuration. Inter-VLAN routing was enabled on the router to allow controlled communication between departments when necessary.



This configuration demonstrates knowledge of network segmentation principles, VLAN configuration, access port management, and routing between logical networks. It also reflects real-world enterprise practices used to limit lateral movement in case of compromise.



Ubuntu Server Deployment and Configuration



An Ubuntu Server instance was deployed using Oracle VM VirtualBox to simulate a production server inside the enterprise network. The server was configured with a static IP address aligned with the Packet Tracer network design to maintain architectural consistency.



SSH services were enabled to allow secure remote management. Root login over SSH was disabled to reduce attack surface. The system firewall (UFW) was configured to allow only required services while blocking unnecessary ports.



System updates were applied to ensure the server was running the latest security patches. Service status checks and log verification were performed using systemctl and journalctl commands to confirm stable operation.



This phase demonstrates Linux administration, service management, network configuration, and system hardening practices.



Apache Web Server Deployment



To simulate an internal enterprise application server, Apache was installed and configured on the Ubuntu machine. A custom HTML page was created and deployed within the Apache document root directory.



The web server was tested locally to verify availability and functionality. This simulates hosting an internal company application or web portal.



Deploying Apache in this lab demonstrates knowledge of service installation, web hosting basics, configuration management, and validation of service accessibility.



Intrusion Detection System (Snort) Implementation



To introduce a security monitoring component, Snort IDS was installed and configured on the Ubuntu server. Snort was set to monitor network traffic and generate alerts based on detected activity.



Traffic was generated within the network to validate that alerts were being triggered and logged correctly. Log files were reviewed to analyze detection output.



This component simulates the monitoring responsibilities of a SOC environment, where analysts review alerts, validate suspicious activity, and monitor network behavior.



Security Hardening and Monitoring



Security hardening measures implemented in this lab include:



Disabling root SSH login



Configuring firewall rules using UFW



Segmenting network traffic using VLANs



Monitoring network activity using Snort



Verifying service integrity through system logs



These steps reflect layered security principles and demonstrate understanding of defense-in-depth strategies commonly applied in enterprise environments.



Skills Demonstrated



Through this project, the following technical competencies were demonstrated:



Enterprise network design and IP addressing



VLAN configuration and inter-VLAN routing



Linux server deployment and hardening



SSH configuration and firewall management



Intrusion detection system setup and monitoring



Log analysis and service validation



Technical documentation using GitHub



Learning Outcome



This lab bridges networking and security concepts into a single integrated environment. It reflects how infrastructure and security controls work together in real-world enterprise systems.



By completing this project, practical experience was gained in designing segmented networks, deploying hardened Linux servers, configuring monitoring tools, and documenting technical implementations clearly.



This project aligns closely with the responsibilities of SOC Analyst and Network Security roles and demonstrates hands-on understanding rather than theoretical knowledge.

