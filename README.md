# Multi-Site Enterprise Network Simulation

## Overview
This project is a comprehensive network topology simulation built using **Cisco Packet Tracer**. It demonstrates a multi-site enterprise network architecture connecting two distinct locations (Site A and Site B) across an ISP router. The network incorporates advanced switching and routing concepts, including VLAN segmentation and dedicated server infrastructure.

## Network Topology & Features

The network is divided into two primary logical and physical boundaries:

### 1. Site A (Headquarters)
* **Core & Edge Routing:** Configured with an edge router connecting to the ISP.
* **VLAN Segmentation:** End devices are segmented into multiple VLANs (VLAN 10, VLAN 20, VLAN 30, VLAN 40) for broadcast domain management and security.
* **Local Servers:** Dedicated local DHCP Server and DNS Server for Site A.
* **Server Farm:** A centralized server cluster attached via a dedicated switch, hosting:
  * **Web Server** (IP: 192.168.100.11)
  * **DNS Server** (IP: 192.168.100.22)
  * **FTP Server** (IP: 192.168.100.33)

### 2. Site B (Branch Office)
* **Routing:** Connected back to Site A via the ISP router.
* **VLAN Segmentation:** Mirrors the headquarters with VLANs 10, 20, 30, and 40.
* **Local Services:** Independent DHCP Server configured specifically for Site B's local network requirements.

## Technologies & Protocols Demonstrated
* **Cisco Packet Tracer (.pkt):** Used for full environment simulation.
* **VLAN Configuration (802.1Q):** Subnetting and inter-VLAN routing.
* **DHCP Configuration:** Automated IP address distribution across multiple VLANs.
* **DNS & Web Services:** Resolving domain names to the internal simulated web server.
* **FTP Services:** File transfer protocol setup for the network.
* **WAN/LAN Routing:** End-to-end connectivity across simulated external networks.

## How to Run the Project

1. Ensure you have **Cisco Packet Tracer** installed on your machine.
2. Clone or download this repository to your local machine.
3. Open the `Final Project.pkt` file using Cisco Packet Tracer.
4. Allow the network devices to converge (wait for the link lights to turn green).
5. Use the PC command prompts to test connectivity via `ping`, test the web server via the simulated web browser, or test file transfers via the FTP client.

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/1016a4d4-7c8a-4c45-96eb-a985450c210b" />


## Repository Contents
* `Final Project.pkt` - The main Cisco Packet Tracer simulation file.
* `image_834963.jpg` - A visual screenshot of the logical topology map.
