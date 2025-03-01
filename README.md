Networking
------------

* Protocol - A defined set of standards that computers must follow in order to communicate properly;
* Computer Networking - Full scope of how computers communicate with each other;

-> TCP/IP Five-Layer Model
---------------------------
#       Layer Name        Protocol           Protocol Data Unit      Addressing
5       Application       HTTP, SMTP, etc       Messages                n/a
4       Transport         TCP/UDP               Segment               Port #'s
3       Network             IP                  Datagram              IP Address
2       Data Link        Ethernet, Wi-Fi        Frames                MAC Address
1       Physical         10 Base T, 802.11      Bits                    n/a

1. Physical Layer
------------------
* Represents the physical devices that interconnect computers, specification, joiner, specifications of the signals sent through, cabling, connectors and sending signals;

2. Data Link Layer / Network Interface / Network Access Layer
-------------------------------------------------------------------
* Responsible for defining a common way of interpreting these signals so network devices can communicate;
* Many protocols for the Data link layer - most common - Ethernet, although wireless technologies are becoming popular;

- The Ethernet standard - specifyes the physical layer attributes and defines protocols responsible for getting data to nodes on the same network or link;

- The data link layer is responsible to get data across a single link;

3. Network Layer / Internet Layer
----------------------------------
* Enables different networks to communicate with each other through a devices known as routers;
- A collection of networks connected together through routers is called the Internetwork - Internet;
- The network layer is responsible for getting data delivered across a collection of networks;
- The most common protocol used here is the IP - Internet Protocol; 
- IP is the heart of the Internet and most smaller networks around the world;

- The network layer delievers data between two individual nodes;

4. Transport Layer
------------------
* Sorts out which client and server programs are supposed to get the data;
- Most common protocol - TCP - Transmission Control Protocol - provides reliability;
- Another protocol - UDP - User Datagram Protocol - does not provide data reliability;

- The Transport Layer (TCP/UDP) - ensures the data on the node gets to the respective application;

5. Application Layer
---------------------
- Many protocols - application specific;
- Protocols allowto browse the web or send receive emails, etc;

------------------------------------------------------------------------------------------------------------------------------------
* OSI Model - Open Systems Interconnectin Model

------------------------------------------------------------------------------------------------------------------------------------
          Layer	             Protocol data unit (PDU)	                                Function[3]
------------------------------------------------------------------------------------------------------------------------------------
  7. Application	                     	                      High-level APIs, including resource sharing, remote file access
  ----------------------------              ---------------------------------------------------------------------------
  6. Presentation	                 Data                       Translation of data between a networking service and an application;                                                                     including character encoding, data compression and encryption/decryption
  ----------------------------                 -------------------------------------------------------------------------------
  5. Session	                                                  Managing communication sessions, i.e. continuous exchange of information                                                                 in the form of multiple back-and-forth transmissions between two nodes
  ------------------------------------------------------------------------------------------------------------------------------
  4. Transport	             Segment (TCP) / Datagram (UDP)     Reliable transmission of data segments between points on a network,                                                                     including segmentation, acknowledgement and multiplexing
   ------------------------------------------------------------------------------------------------------------------------------
	3. Network	                     Packet	                      Structuring and managing a multi-node network, including addressing,                                                                     routing and traffic control
   ------------------------------------------------------------------------------------------------------------------------------
  2. Data link	                     Frame	                    Reliable transmission of data frames between two nodes connected by a                                                                   physical layer
   ------------------------------------------------------------------------------------------------------------------------------
   1. Physical	                      Bit                       Transmission and reception of raw bit streams over a physical medium
    ------------------------------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------------------------------------
* Basics of Networking Devices
------------------------------

1. Cables - Connect different devices to each other allowing data to be transmitted over them; 
 - 2 types - Copper or fiber, binary data value is sent through these copper cables by changing the voltage and the system at the receiving end is able to interpret these voltage canges and the binary data;
a. The most common forms of copper twisted-pair cables used in networking are Cat5, Cat5e, and Cat6 cables; - Cat -> category -             different physical categories like the number of twists, lengths and transfer rates, inteferences, crosstalk;
  - Crosstalk - When an electrical pulse on one wire is accidently detected on another wire;
b. Fiber optic cables - Contain individual optical fiber, which are tiny tubes made out of glass about the width of a human hair;
  - Pulses of light are used to represent ones and zeros of the data;
  - It is used in places where there is a lot of electromagnetic interfernces;
  - Higher speed, longer distances, no data loss, expensive;
  
  
2. Hubs and Switches
----------------------
* Hub - A physical layer device that allows for connections from many computers at once, it could cause a collision domain;
- Collison domain - a network segment where only one device can communicate at a time, otherwise electrical signal from other systems will interfere, slows;

* Switch - A Data-link layer device - It inspects the contents of the Ethernet protocol data being sent around the network, determine which system the data is intended for and send it to it; Eliminates collision domain;

3. Routers
------------
* Hubs and Switches are the primary devices used to connect computers on a single network , usually referred to as LAN (Local Area Network);
- Router - A device that knows how to forward data between independent networks;
- It operates at the 3rd layer - Network Layer;
- A router detemines the IP address to determine where to send the data;
- Routers store internal tables containing information about howto route traffic between lots of different networks in the world;
- Home network , local office netowrks have less sophisticated routers, whereas the one connected to the ISP are called core routers which handle a lot of traffic and functionality;

- Border Gateway Protocol (BGP) - Routers share data with each other via this protocol, which lets trhem to learn about the most optimal paths to forward traffic;

