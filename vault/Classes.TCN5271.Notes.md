---
id: 2c2ma0eGryXI9CFysgqd4
title: Notes
desc: ''
updated: 1645035812653
created: 1642696041361
---



### Week 1: Introductions



### Week 2: Recap Networking

####  Trends

**Important**

* Realiazation of Iot advancement came from  microcontrollers, flash storage radio, communication, and sensors.
* Bell's law: every 10 years new type of computers
* Cyber-physical: Interaction with the physical world(control)(car)
* Ubiquitous Computing (Sensor and networks everywhere)

> Next Class(1/27): Come up with other interesting IoT application and IoT devices. (Wierd one) (UWB :) )

**Possible aplications:** medicine, entretainment, enterprises, home, traffic, emergency situation.

* Dedicated short range Comminication(DSRC): vehicle sommunication.(research)
* Remote control Beetle: US Army studies
* Soccer: Goal Detection
* GDPR

#### Characteristics of wireless networks

**Types**: Satellite, WAN, Mobile ad-hoc networks, 1G-5G, UWB ,etc

Challenges OF Wireless Computing:

    1. Wireless Communication
    2. Mobility
    3. Poor REsources dure to Portability


### Week 3

70% traffic is wireless in the internet

#### Wireless Challenges

1. limited transmission: 10m - 500m
2. Mosly Limited Bandwith: 
3. Disconnections: Network partition and stall all application.
4. Security: Easy to intrude in the network
5. Heterogeneous devices and network connections.
    * wired links
    * Outdoor: Radio
    * Indoor: Infrared
    * Rural Areas: Satellites

> HW: Measure the data RATE and which standard, cable provider

RG-6 100 MBps

Wireless enviroment is not deterministic  or stocastich(performance degragation)

Context-Aware systems: Depends on the context the behavior will change.

#### From QUiz:

Active Network: Aggressive networking

* **Important:** steps of evolution

* Iot is subset of CPS(Cyber-physical systems): False

### Week 4

#### What is Network

* Componets
* Inter - connecting multiple networks
* Intra - Within something
* Core - Medium used for networks to connect(Beltway)
* ISP - connect regions
* Miami ISP
* Protocol - Semantics, timing, syntax

* Current model of the internet of Client-Server

* Peer-to-Peer: Bittorrent
* Wep3.0

#### Protocol

OSI - Official
TCP/IP - Defacto(Everyone uses it but is not official)
SMPT - Simple mail transfer protocol

### Week 5

> Important: Slide 29 (Layer Description) - OverviewNetworking-1
> Ethernet: today is star topology
Ethernet std. (20-30) revisions

1. **Data link:** responsability of transferring datagram from one node to adjacent node over a link.
    * Services: Framing, reliable delivery, flow control(pacing), **error detection, error correction**, Half duplex, full duplex.
    * MAC medium access control -> channel partition, random access, taking turn
    * CSMA - Carrier Snese Multiple Access
        * Propagation delay: Time it takes signal to spread over a share medium.
        * Transmission delay: Time it takes to put data into the share medium.
    * CSMA/CA(Collition avoidance) - WiFi, wireless technology
    * CSMA/CD (Collition Detection) - Ethernet
    * CRC: Cyclic Redundancy Check
    * ARP: Helps finding link layer address

2. **Network(Routing) layer**: Helps routing from network to network, not end-to-end
    * Forwarding: passing interface to interface  in router itself.
    * Routing: detrmine route taken , from source to destination
    * Routing algorithms: finds least cost path
        * Global or decentralized  / Static or dynamic
        * Dijkstra's algorithm(centralized)
        * Distance Vector (Decentralized)
        * Routing Portocols: RIP, OSPF, BGP, EIGRP and IS-IS.

3. **Transaport layer:** end-end(E2E), port numbers
    * System ports or Well-know: 0-1023


### HW 1

1. (9pts) Provide names and brief descriptions for one protocol at MAC, network and application layers which are specifically designed for Internet-of-Things.

    **MAC Layer:** LoRaWAN is a Access Contorl (MAC) protocol used for wide area network, which it is used in conjuction with LoRa to transamit signals for very large distances in the magnitude of miles. The difference betweem LoRa and LoRaWAN is that like we specified before LoRa is a methods of  transmisttin signals which makes it a layer 1 on the OSI model, while LoRaWAN is the protocol used for point to point communication which is a layer 2 protocol.

    **Network Layer**: CARP (Channel-Aware Routing Protocol) 

    **Application Layer:** Message Queuing Telemetry Transport (MQTT) works on top of TCP/IP layer, it was design to be used on low power consumption devices and helps with unreliable communcation in networks. It uses a subscriber, pusblisher and broker model


2. (12pts) Describe the following: Propagation Delay, Transmission Delay, Queuing Delay, and Throughput. 



3. (12pts) Discuss the difference between Internet-of-Things, Wireless Sensor Networks and Cyberphysical Systems.

4. (12pts) In CSMA/CD, after the fifth collision, what is the probability that a node chooses K = 3? The result K = 3 corresponds to a delay of how many seconds on a
10 Mbps Ethernet?

5. (12pts) Explain the process for how MAC addresses are created by IEEE and assigned to physical devices.

6. (12pts) Compare IPv4 and IPv6 headers in terms of fields and bit size. And then find out what is the percentage of routers on Internet core which still does not support
IPv6.

7. (12pts) What is the difference between ”source routing” and ”distance vector” routing? Explain your answer.

8. (12pts) Consider a broadcast channel with N nodes and a transmission rate of Rbps. Suppose the broadcast channel uses polling (with an additional polling node) for multiple access. Suppose the amount of time from when a node completes transmission until the subsequent node is permitted to transmit (that is, the polling delay) is dpoll. Suppose that within a polling round, a given node is allowed to transmit at most Q bits. What is the maximum throughput of the broadcast channel?


9. (7pts) What is an RFC? Go to IETF web site and find the first and last RFC on TCP. List their names and RFC numbers.