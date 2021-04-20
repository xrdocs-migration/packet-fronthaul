---
published: false
date: '2021-03-26 10:09 +0530'
title: Industry’s first Converged Packet Fronthaul Solution – The NCS540-FH
author: Sounak Mukherjee
tags:
  - Packet Fronthaul
  - Converged Fronthaul
  - NCS540-FH
  - CPRI
  - eCPRI
  - RoE
  - oRAN
---


With the huge amount of technology innovation in the Radio Access Network driven by need for higher bandwidth, larger radio channels, increased network density, lower latency, power efficiency and enhanced inter-cell coordination (to name a few), every mobile operator is examining possible architectural modifications in their network. Exploring the large benefits of Centralized and/or Cloud/Virtualized RAN, Cisco has made successful inroads into the RAN space with a Packet Fronthaul product of their own.  


<a href="https://github.com/xrdocs/packet-fronthaul/tree/gh-pages/images/FH_1.png"><img src="https://github.com/xrdocs/packet-fronthaul/tree/gh-pages/images/FH_1.png" width="450" height="450" class="align-center" /></a>
  
  
Even though there are existing (sub-optimal) Fronthaul solutions in the industry, there were a bunch of reasons that drove Cisco’s decision to develop a Packet fronthaul solution, some of them being:  
1. Reduced Total Cost of Ownership as qualified by [ACG Research](https://www.cisco.com/c/dam/en/us/solutions/collateral/service-provider/mobile-internet/acg-fronthaul-architectures-for-5g-networks.pdf)  
2. High Speed and ultra-low latency forwarding with Stat-Muxing benefits
3. Flexible and Programmable architecture (ASIC + FPGA Based)
4. Precise Timing and Synchronization Capabilities (Class C compliant)
5. End to End IP based network for more visibility and easier integration with transport network
6. Open and Automated Management (Easier Programmability with IP Based Fronthaul)
7. Topology Independence (Ring, Mesh, Point to Point – Everything can be supported with SR-MPLS based Transport)  

Along with these advantages, the product is consistent with Cisco’s End to End IP network strategy built to run on a [Converged SDN Transport](https://www.cisco.com/c/en/us/solutions/service-provider/converged-sdn-transport.html) architecture. This essentially extends Cisco’s transport architecture to the Radio Access Network, seamlessly. If we are to focus only on the RAN, the Packet Fronthaul portfolio can support legacy LTE (CPRI Based), New Radio (5G eCPRI), oRAN (7.2x) and Enterprise (Ethernet) all in one platform.
  

![FH_2.png]({{site.baseurl}}/images/FH_2.png)
  
  
Now, that we have understood the product placement and development reasoning, let me introduce the actual products to you. The Cisco NCS540-FH or NCS540 Fronthaul portfolio is based on two products, a Cell Site Router or the N540-FH-CSR-SYS and the Aggregation router or the N540-FH-AGG-SYS. The Cell Site router, as the name suggests, sits at a Cell Site (inside a Cabinet) and can carry 300 Gbps of ingress/egress traffic. It is capable of packetizing legacy (LTE based) CPRI traffic using IEEE 1914.3 Radio over Ethernet technology and carrying it on a point-to-point pseudo wire over an IP/Ethernet network.  
This is the first ever Cisco platform capable of processing and packetizing CPRI constant rate bit streams. The Aggregation router sits at a Far Edge Data Center (or a Centralized Hub Site) and can process 900 Gbps of ingress/egress traffic. It has the same capabilities as the Cell Site Router but can also be used for aggregating multiple cell site routers and connecting your Fronthaul to the Midhaul/Backhaul network.
  
  
![FH_3.png]({{site.baseurl}}/images/FH_3.png)
  
  
While you can take a look at the Data Sheet of these models [here](https://www.cisco.com/c/en/us/products/collateral/routers/network-convergence-system-500-series-routers/datasheet-c78-744599.html), let me summarize the key highlights of Cisco’s Converged Packet Fronthaul portfolio :  
- The CSR and the AGG router can support upto 12 and 24 CPRI Ports respectively
- Some of these CPRI Ports can act as Universal Ports wherein we can operate them for either CPRI or Ethernet traffic
- Both routers can support 1G/10G/25G/100G Interfaces, while you can configure 2x100G on the CSR, you will be able to have 4x100G uplinks on the AGG router
- CPRI Rate Options 3, 4, 5, 6, 7 and 8 are supported while eCPRI and oRAN based 7.2x traffic can also pass through these products
- The Packet Fronthaul portfolio can operate seamlessly with the legacy CPRI based RAN vendors like Ericsson, Huawei, Nokia and Samsung 
- There is support for IEEE 1914.3 Radio over Ethernet for the purpose of packetization of radio traffic
- RoE Structure Agnostic Type-0 (Tunnel Mode) and Structure Agnostic Type-1 (Line Code Aware Mode) are supported on both platforms
- Time Sensitive Networking (TSN) in the form of IEEE 802.1 Qbu or [Frame Preemption](https://www.ieee802.org/1/pages/802.1bu.html) is supported on both platforms, wherein you can preempt lower priority traffic to reduce the latency of higher priority traffic (like CPRI/eCPRI) in your network
- Both platforms are built for ultra-low latency applications and are capable of <10 µs of forwarding latency.
- SyncE, PTP and Class-C Boundary clocks are supported on both platforms
- Both routers support the existing routing and switching feature-set of the [NCS540 portfolio](https://www.cisco.com/c/en/us/products/collateral/routers/network-convergence-system-500-series-routers/datasheet-c78-740296.html)
- The Converged Packet Fronthaul portfolio is telemetry ready, supporting a wide range of Cisco’s native YANG Data Models. There is limited support for IETF and OpenConfig Models too
- These devices can be seamlessly integrated into Cisco’s [Crosswork Network Automation](https://www.cisco.com/c/en/us/products/cloud-systems-management/crosswork-network-automation/index.html) portfolio for enhanced management and programmability.  

If you are interested in the Cell Site Router, you can already connect with us to place an order. The device is running Cisco’s IOS-XR code base which is our common operating system across the physical and virtual platforms, and it is optimized for enhanced performance and emerging market needs.  

We will follow this up with multiple blogs on this platform, going in-depth into the configuration and capabilities of the platform, so watch out for this space.  

---------------------------------------------------------------


**Author : Sounak Mukherjee**  
**Role : Technical Marketing Engineer | 5G | Mobile Fronthaul**


---------------------------------------------------------------
