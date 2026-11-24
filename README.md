# Cisco Small Office LAN – Packet Tracer Project

## 📌 Project Overview

This project demonstrates the design and configuration of a small office Local Area Network (LAN) using Cisco Packet Tracer.

The network consists of 3 PCs connected to a Cisco 2960 switch, which is connected to a Cisco 2911 router. The project focuses on basic network configuration, IPv4 addressing, default gateway configuration, and connectivity testing.

## 🖥️ Network Topology

**Devices Used:**
- 1 × Cisco 2911 Router (R1)
- 1 × Cisco 2960 Switch (SW1)
- 3 × PCs (PC0, PC1, PC2)
- Copper Straight-Through Cables

## 🌐 IP Addressing Scheme

| Device | IP Address | Subnet Mask | Default Gateway |
|---|---|---|---|
| Router R1 | 192.168.1.1 | 255.255.255.0 | N/A |
| PC0 | 192.168.1.10 | 255.255.255.0 | 192.168.1.1 |
| PC1 | 192.168.1.11 | 255.255.255.0 | 192.168.1.1 |
| PC2 | 192.168.1.12 | 255.255.255.0 | 192.168.1.1 |

**Network Address:** 192.168.1.0/24

## ⚙️ Configuration Performed

### Router Configuration

The following commands were used to configure the router interface:

```bash
enable
configure terminal
interface gigabitEthernet 0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit
```

### PC Configuration

Static IPv4 addresses were manually assigned to all three PCs along with the appropriate subnet mask and default gateway.

## 🧪 Connectivity Testing

The following tests were performed to verify network connectivity:

**1. PC-to-Router Connectivity**

```bash
ping 192.168.1.1
```

**2. PC-to-PC Connectivity**

```bash
ping 192.168.1.11
ping 192.168.1.12
```

**3. Router Interface Verification**

```bash
show ip interface brief
```

The router interface was verified to ensure that its status and protocol were both UP.

## 📸 Screenshots

Screenshots demonstrating the network configuration and testing are available in the `screenshots` folder.

1. `01-topology.png` – Complete network topology.
2. `02-ip-configuration.png` – PC IP configuration.
3. `03-router-ping.png` – PC-to-router ping test.
4. `04-pc-connectivity.png` – PC-to-PC connectivity test.
5. `05-interface-status.png` – Router interface status verification.

## 🛠️ Tools & Technologies

- Cisco Packet Tracer 9.0.1
- Cisco IOS CLI
- IPv4 Addressing
- LAN Networking
- ICMP (Ping)
- Basic Router and Switch Configuration

## 🎯 Learning Outcomes

Through this project, I practiced:

- Building a small office LAN topology.
- Connecting PCs, switches, and routers.
- Configuring IPv4 addresses and subnet masks.
- Understanding default gateways.
- Configuring router interfaces.
- Testing network connectivity using ping.
- Verifying router interface status using Cisco IOS commands.

## 📂 Project Files

- `Small_Office_LAN.pkt` – Cisco Packet Tracer project file.
- `README.md` – Project documentation.
- `screenshots/` – Network topology and configuration screenshots.

## 👨‍💻 Author

Networking Practice Project – CCNA Learning Journey

**Project 02: Small Office LAN Configuration**
