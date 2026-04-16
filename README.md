# SFC — Secure Financial Corporation Bank Project

This repository contains all working files, configurations, and documentation used throughout the **SFC Secure Enterprise Network Project**.
Everything here documents the design, implementation, verification, and backups for a secure multi-site banking network built and tested in a lab environment.

---

## What’s in This Repository

### 1) Network Configurations

Full CLI configurations, backups, and device-specific files for all routers, switches, and firewalls across SFC sites:

* Headquarters (HQ)
* Branch Office
* MPLS / ISP connections

These configurations include routing protocols, WAN/VPN setups, firewall policies, security controls, and verification states.

---

### 2) Design & Documentation Files

* **Network Topology** — Visual representation of HQ, Branch, MPLS, and ISP connectivity
* Design documents explaining:

  * Network architecture
  * VLAN segmentation (IT, HR, Finance, Admin, Servers)
  * Security zones (Inside, DMZ, Outside)
  * IP addressing and routing design

  ![Topology](Network%20Topology.png) 

---

### 3) Backup Files

Snapshots of device configurations taken during key stages of implementation, testing, and failover validation.

---

### 4) System & Server Files

Supporting materials from the EVE-NG environment and virtual machines, including:

* Windows Server (Active Directory, DNS, DHCP)
* RADIUS (AAA authentication)
* Syslog server
* Endpoint devices (Windows 10 clients)

---

## Purpose & Scope

The goal of this project is to design and implement a **secure, high-availability enterprise banking network** that connects a Headquarters and a Branch using industry-standard technologies.

This project demonstrates:

* Secure network segmentation using VLANs
* Firewall-based traffic control and DMZ isolation
* Centralized authentication using Active Directory and RADIUS (AAA)
* Secure inter-site communication using:

  * MPLS Layer 3 VPN (Primary)
  * Site-to-Site VPN (Backup)
* Automatic failover between WAN links
* Network monitoring and logging using Syslog

Everything in this repository is practical and can be deployed in a simulator like EVE-NG for verification and testing.

---

## How to Use This Repository

**If you’re studying or reviewing this project:**

1. Open the **Network Topology** diagram to understand the overall design.
2. Load the configurations into your lab environment (EVE-NG recommended).
3. Use the configs and backups to step through:

   * Routing (OSPF/BGP/MPLS)
   * VPN tunnels and failover
   * Firewall policies and access control
   * VLAN segmentation
4. Perform verification using CLI:

   * `ping`, `traceroute`
   * `show` and `debug` commands
5. Compare your results with the provided configurations.

---

## Recommended Tools

* **EVE-NG** (full lab simulation)
* Cisco IOSv / L2-L3 images
* Cisco ASAv (Firewall)
* PuTTY (remote access)
* CLI tools (`show`, `debug`, `ping`, `traceroute`)

---

## Attribution

All work in this repository was completed by **Husain Ali (Student ID: 202202674)** as part of the Secure Financial Corporation (SFC) enterprise network project.
