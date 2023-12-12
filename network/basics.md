#### Network Hardware components
- Hub
  - Receives message from one computer and relays to all others
- Switch
  - Receives message from one and transfers message directly to the target
- Router
  - Connects dissimilar networks
  - Uses routing table
- Gateway
  - Connect internal networks to internet 

#### Network Protocols: OSI Model
- Open Systems Interconnection (OSI) Model
- 7 Layers
  - 7- Application
    - Ex: HTTPS, HTTP
    - Referred as Data or messages
  - 6- Presentation
    - Encryption
    - Unicode translation
  - 5- Session
    - Decides if it will simplex, duplex etc
  - 4- Transport
    - Blocks of data is called segments
  - 3- Network
    - Handling comm between networks
    - handles packetization and addressing
  - 2- Data link
    - Refered as Frames
    - Packet framing within a network
    - Addressing within a network
    - Media access control
    - Ex: Ethernet - Used for LAN
  - 1- Physical
    - Bits
    - Data is placed on comm medium

#### TCP/IP Model
- Doesnt map well in OSI Model
- Covers all layers and has multiple protocols
- TCP/IP Model layers
  - Application layer
    - Covers Application, Presentation and Session layers of OSI Model
    - Protocols: HTTP, FTTP, Telnet, NTP, DHCP and PING
    - Dynamic Host Configuration Protocol ( DHCP )
      - Assigs network addresses as needed
  - Transport
    - Covers Transport and partially session layers
    - Protocols: TCP, UDP
    - UDP - Used for short quick messages
    - TCP
      - Splits large messages
      - Error checking
  - Network
    - Covers Network layer in OSI model
    - Protocols: IP, ARP, ICMP, IGMP
    - Handles addressing, routing packages across networks
  - Network Interface
    - Covers Data link and Physical layers in OSI Model

#### IP Management
- IP V4
- Mitigation for limitation of IP V4 sizing
  - Private addressing
  - IP V6
- Address Translation
    - Network Address Translation (NAT)
      - Required to translate internal IPs to and from external IPs
    - Port Address Translation

#### Ethernet
- Used in LAN
- Communication Technique -  Carrier Sense Multiple Access (CSMA) / Collission Detection (CD)
 
  - 
