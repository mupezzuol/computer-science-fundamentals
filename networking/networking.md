# Networking

This README is focused in the topics related with networking in general, OSI Model, TCP/IP, HTTP, DNS, etc.

<details>
<summary><strong>OSI Model</strong></summary>

The Open Systems Interconnection (OSI) model is a conceptual framework that standardizes the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology. It divides network communication into seven abstraction layers.

#### Layer 1: Physical Layer
- **Purpose**: Transmits raw bit streams over physical medium
- **Functions**: 
  - Electrical and physical specifications of devices
  - Data encoding and signaling
  - Physical topology
- **Examples**: Cables, hubs, repeaters, network adapters
- **Data Unit**: Bits

#### Layer 2: Data Link Layer
- **Purpose**: Provides node-to-node data transfer and error detection/correction
- **Functions**:
  - Frame synchronization
  - Error detection and correction
  - Flow control
  - MAC addressing
- **Examples**: Ethernet, Wi-Fi, PPP, switches
- **Data Unit**: Frames

#### Layer 3: Network Layer
- **Purpose**: Routes data between different networks
- **Functions**:
  - Logical addressing (IP addresses)
  - Path determination
  - Routing
  - Packet forwarding
- **Examples**: IP, ICMP, routers, Layer 3 switches
- **Data Unit**: Packets

#### Layer 4: Transport Layer
- **Purpose**: Provides reliable data transfer between end systems
- **Functions**:
  - Segmentation and reassembly
  - Connection establishment and termination
  - Flow control
  - Error recovery
- **Examples**: TCP, UDP
- **Data Unit**: Segments (TCP) / Datagrams (UDP)

#### Layer 5: Session Layer
- **Purpose**: Manages sessions between applications
- **Functions**:
  - Session establishment, maintenance, and termination
  - Session checkpointing and recovery
  - Dialog control (half-duplex or full-duplex)
- **Examples**: NetBIOS, RPC, SQL sessions
- **Data Unit**: Data

#### Layer 6: Presentation Layer
- **Purpose**: Data translation, encryption, and compression
- **Functions**:
  - Data format translation
  - Encryption and decryption
  - Data compression
  - Character encoding
- **Examples**: SSL/TLS, JPEG, MPEG, ASCII, EBCDIC
- **Data Unit**: Data

#### Layer 7: Application Layer
- **Purpose**: Provides network services directly to applications
- **Functions**:
  - Network process to application
  - User interface
  - Application services
- **Examples**: HTTP, HTTPS, FTP, SMTP, DNS, SSH
- **Data Unit**: Data

### OSI Model Data Flow
```
Application Layer    │ Data
Presentation Layer   │ Data
Session Layer        │ Data
Transport Layer      │ Segments/Datagrams
Network Layer        │ Packets
Data Link Layer      │ Frames
Physical Layer       │ Bits
```

### Key Points
- Each layer adds its own header (encapsulation) when sending data down
- Each layer removes its header (decapsulation) when receiving data up
- Lower layers provide services to higher layers
- The model helps in troubleshooting network issues by isolating problems to specific layers

</details>