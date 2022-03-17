---
id: 2c2ma0eGryXI9CFysgqd4
title: Notes
desc: ''
updated: 1645125654161
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

    **Propagation Delay**: The delay for a signal to propagte/travel thorugh a medium, good example of this time takes for WiFi signal to move thorugh air to reach other terminal.

    **Transmission Delay**: The delay for a data packet to be put into the transmission link or the physical layer.

    **Queuing Delay**: This delay is results of the packet arriving to a router network interface and waiting for its turn to be forwared to the next network interface.

    **Throughput**: When refering to Throughput we are refering to the amount of that successfully sent to other network interface. Normally will be measured in bits, megabytes, and gigabytes per seconds.

3. (12pts) Discuss the difference between Internet-of-Things, Wireless Sensor Networks and Cyberphysical Systems.

    **Internet-of-Things:** 
    **Wireless Sensor Networks:**
    **Cyberphysical Systems:**


4. (12pts) In CSMA/CD, after the fifth collision, what is the probability that a node chooses K = 3? The result K = 3 corresponds to a delay of how many seconds on a
10 Mbps Ethernet?

https://gateoverflow.in/132269/Networking-kurose-ross

5. (12pts) Explain the process for how MAC addresses are created by IEEE and assigned to physical devices.




6. (12pts) Compare IPv4 and IPv6 headers in terms of fields and bit size. And then find out what is the percentage of routers on Internet core which still does not support
IPv6.



7. (12pts) What is the difference between ”source routing” and ”distance vector” routing? Explain your answer.



8. (12pts) Consider a broadcast channel with N nodes and a transmission rate of Rbps. Suppose the broadcast channel uses polling (with an additional polling node) for multiple access. Suppose the amount of time from when a node completes transmission until the subsequent node is permitted to transmit (that is, the polling delay) is dpoll. Suppose that within a polling round, a given node is allowed to transmit at most Q bits. What is the maximum throughput of the broadcast channel?




9. (7pts) What is an RFC? Go to IETF web site and find the first and last RFC on TCP. List their names and RFC numbers.



### Week 6

#### Quiz 2 

Full Mesh: every node is connected to every node

#### Layer 1
1. Transmission Fundementals
    * Relaying Information: Electrogmagnetic Signal
    * Signal:
        * Function of time
        * 3 Componets: Amplitude, frequency, Phase
        * Sine wave
        * Analog(no breaks in the signal or continuos) or Digital(discrete signal intensity)
        * Wavelength: distance ocuppied by 1 cycle
    * Effects of Signal:
        * Attenuation: lose power, lower amplitude
        * Distortion: Interference  of defferent frequencies components(Interference: Block the path of, disruption.)
        * Noise: The absence of signal, there is random mix of frquencies on the channel called noise.
        * Error: When combined with noise, can lead to bits been changed causing an error.
    * Spectrum: range of frequencies a signal contains
    * Bandwidth: Width of the scpectrum, increasing the bandwith makes the wave look more like a square
        * Increasing bandwith reduce distortion.
    * Channel Capacity: Maximun rate at which data can be transmited over a given path.(C=2B log(M)) B = Bandwith, M = Voltage levels, C = Channel capacity
    * **important** SNR: (Signal Nooise Ratio) Signal/Noise Power (represented by decibels)
        * SNR = 10log10(signal.pow/noise.pow)
    * Digitial signals can only propagate thorugh wired mediums. So we need to convert Digital-to-analog.   
    * Modem: modulator, demodulator
    * Encoding(Modulation of analog to digital):
        1. ASK Amplitude shift keying
        2. FSK Frequency shift keying
        3. PSK Phase shift keying
    
    > QAM: modulation technique

    * Analog to digital
        * Modulation will help to provide frequency devision multiplexing
        * AM Amplitude Modulation
        * FM Frequency Modulation
        * PM Phase Modulation
    * Digitization: convert analog data into digital signals (slide 12)
        * Pulse Code Modulation (PCM)
        * Delata Modulation (DM)
    * Multiplexing
        * Carrying multiple signals in one medium
        * FDM Frequency Devision Multiplexing
        * TDM Time Devision Multiplexing
    * Transmission Media for Signals
        * Guided media: Solid media such as copper, optical fiber, etc.
        * Unquided: Atmosphere, outer space: Wireless transmission
    * General Frequency Ranges:
        * UHF Ultra high frequency
    * FCC Federal Communication Commission
        * Regulate the interstate and international communications.
        * Prevent interferences between different devices.
        * Spectrum Allocation


2. Radio Basics:(RF)
    * Radio Waves
        * 3KHz to 300 GHz
        * Easy to generate
        * Penetrate buildings
        * Omnidirectional
    * All signals are converted to analog
    * Antenas:
        * Electrical conductor(radiates/transmits) electromagnetic waves into space
        * Radiation Pattern of an Antenna
            * Radiates in all direction(ideal case)
            * ISOTROPIC(Omni-directinl radiation pattern in 3D) - sun is the best example
            * Real antennas are not isotropic
            * Usually in 2D donut
            * Dipoles (half-wave) and Quarter wave dipoles
    * Directional Antenneas
        * Directional are very common, often based on stations
        * Beam width: measure of directivity antenna
        * Antenna gain: Power output, in a particular direction, compared to pefect omnidirectional.(measure in dBi) ![antenas dBi](https://www.ahsystems.com/EMC-formulas-equations/images/Antenna-gain-dBi.png)
        * Types Examples: Isotropic, Omni DIrectional, Yagi Dish.
    * Radio Propagation
        ![Radio Propagation](https://image.slidesharecdn.com/lectureu1u2wirelesstransmission-151115072403-lva1-app6892/85/wireless-transmission-12-320.jpg?cb=1447572373)
        * Transmission Range: Communication possible and low error rate.
        * Detection range: no communication possible, detect the signal
        * Interefence Range: signal may not be detected, adds noise from background
    > Higher frequency travel less
    * Propagation: 
        * Ground wave: Freq: 2MHz, contour  of earth, AM Radio
        ![ground wave pro](https://7am0d.weebly.com/uploads/1/3/6/7/13675140/7432717.png?1)
        * Sky Wave: Travel thousans of kilometers, reflected from ionessphere and earth's surface, Military Comm
        ![Sky wave pro](https://7am0d.weebly.com/uploads/1/3/6/7/13675140/1701360.png?1)
        * Line of Sight: Freq: 30MHz 
        ![Line of Sight(LOS)](https://7am0d.weebly.com/uploads/1/3/6/7/13675140/8792977.png?1)
    * Impairments in LOS Transamission:
        * The signal recieved is different the signal transmitted.
        * Coomon Imparments: noise, thermal noise, free space loss, multipath propagation, fading, Reflection, Scattering, Shadowing, Diffraction
        * Reeiving power of he signasl depends on these  factors.
    > Important
    * Fading: Varaition of recieved signal power caused by changes in the medium or path.
         * Causes: Free sapce loss, multipath propagation(reflection,scattering, ...), mobility, atmospheric absorption, interference.
         * Mobile envrioments creates more complex effects.
    
    * Free Space Loss: Any type of signal disperses with the distance as signal is being spread over larger and larger area.
        * Equation: ![](https://www.radartutorial.eu/01.basics/formel/rb55(3).print.png)
        * K*1/f^2d^2
    * Multipath Propagation:
        * Reflection: signal encounters a surface that is large relative to wavelength of the signal
        * Scattering: Incoming signal hits an object whose size in the order of the wavelength if signal or less.
        * Diffraction: edge of impenetrable body that is large enough  compared to the wavelength
        * Refraction: Bending of radio waves as they propagate thorugh the atmophere.
    * Mobility effects:
        * As user moves, signal paths may chnage.
        * Fast Fading (ends like a noise, move half the wavelenght) and slow fading(move larger that wavelegnth)
        ![Fast and slow fading](https://www.rfwireless-world.com/images/fast-fading-vs-slow-fading.jpg)
    * Spread Spectrum(transmit in wider freq.)
        * Motivation : wider bands the signals can be wiped out.
        * Solution: wider bandwidth, transmit many different frequencies.
        * Initial Motive: Prevent jamming for military applications
        * Used in every wireless networks today. Multiple transmitters can transmit at the same freq range.
    * Frequency Hopping Spread Spectrum(FHSS)
        * Multiple base freq(channels)
        * randomlly hops to one of thoses
        * Recviever should do the same
        * SPreading code = Hoping Sequence
        * Fast Hopping(several freq per bit), and slow Hopping(several bit per freq)
            * dewll time: stick with that feq
            * bit period: time to stay on a bit
    * Spread code: predefine sequences
    * Direct Sequence Spread Spectrum(DSSS) 
        * Each bit in orginal signal  is represented by multiple bits in the transmitted signal
        * Very resilient to interference
        * Transmitted signal is code CHIP
        * Multiple users can share the bandwidth, using differen chipping.

3. Hardware
    * Example: Sensor, actuators, etc
    * Components: Sensor, IO, Controller Radio, Power unit
    * ADC in IO = Analog to digital converter
    * Actuation = taking a physical action
    * Mobilizer = ability to move, flying like drones, it requires additional hardware
    * Location finding system: GPS, or location tech
    * Requirements of the application are design decision(size, energy, cost, sensors/actors)
    * Controller:
        * Factors: # of transistors(size, cost, power), # clock cyles(power), time to develop(acceptance), nonreccurring enginerring cost (NRE)(cost, acceptance)
        * Ideal minimize all factors at the same times.
        * CPU: Central Proccessing Unit of the device
        * Different architectures:
            * Mircocontroller(MCU): resource contranted, sofware controlled, general purpose
            * Digital Proccessor(DSP): Proccess large data streams, parallelizing.
            * Field-Proggrammble Gate Arrays(FPGA): Special harware, expensive, limited configuration
            * Application-Specfific Integrated Circuits(ASIC): Special hardware designed only for one application, possible embedding several MCU or DSP cores. 

> HW1: Source Routing(know the whole path)  vs Distance Vector(only know the neighbor distance)
> Source: Does routing computation before sending, nobody keeps other information.


4. MAC for Wireless Enviroments
    * What is MAC: open, brodcast medium, limited bandwidth, multiple user
    * MAC Protocols: Multiple Access Control, Medium Access, or Media Access
    * Expected from MAC Protocol: limted delay, high throughput, fairness, scalability, stability, low power consumption. QoS, robustness agaisnt channel fading
    * Problems: Half duplex,Packet Loss, location depended, limted battery time, Time Varying Channel,
    * Causes energy waste: Collision, Control packet overhead, overhearing unnecessary traffic, Long Idle time (**Dominat Factor**)
    * _Important_ Random Access PRoblem: Hidden and Exposed terminal
    * Distributed and Centralized MAC Protocol

5. Wireless LAN Standard (802.11 - 1999)
    * Provides a MAC and Physical functionality
    * Frequency allocation: alll user must operate on a common freq. band
    * Inference and reliability: Collision, Security, Power cons., Human safety, Mobility
    * Std today: 802.11ac Max: 1300 Mbps OFDM/QAM
    * 5 GHz
    * MIMO Multiple Input and MUltiple output
    * Two Operational Modes: 
        * Infratructure Mode
            * BBS Basic Service Set
            * Extended Service set (ESS)
        * Ad-hoc: IBSS Independent Basic Service Set
    * CSMA/CA with ACK
    * Wifi solution to exposed and hidden terminal is RTS(Request to send) and CTS(Clear to send)  Virtual Carrier Sensing
    * RTS 20 bytes and CTS 16 bytes
    * Contention Window (CW) wait for to be idle to send from 0 to CW
    * _Important_ You require ACK cz cant detect collision 
    * Channel Assigment and Regiistration:
        * Roaming: moving from access point to others. Re-Association
    * Other issures: Fragmentation, Synchronization, Power Management, QoS for Voice Packets















---
To be Continued

