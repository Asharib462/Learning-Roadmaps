# Basic Networking Devices

## Cables

Cables are what connect different devices to each other, allowing data to be transmitted over them.

Most network cables used today can be split into two categories:

### 1. Copper Cables

- Most common form of networking cable
- Made up of multiple pairs of copper wires inside plastic insulator
- Binary data is transmitted by changing voltage between two ranges
- Receiving system interprets voltage changes as binary ones and zeros

#### Common Types of Copper Cables

| Cable Type | Description |
|------------|-------------|
| Cat 5 | Older standard, mostly replaced by Cat 5e |
| Cat 5e | Improved version of Cat 5, reduces crosstalk |
| Cat 6 | Higher performance, shorter maximum distance at higher speeds |

**Crosstalk**: When an electrical pulse on one wire is accidentally detected on another wire, causing network errors.

### 2. Fiber Cables

- Contain individual optical fibers (tiny glass tubes)
- Use pulses of light to represent binary data
- Advantages:
  - Immune to electromagnetic interference
  - Faster data transport
  - Longer distance without data loss
- Disadvantages:
  - More expensive
  - More fragile
- Common in data centers rather than home/office environments

## Network Devices

### Hub

- Physical layer device (Layer 1)
- Allows multiple computer connections
- All connected devices communicate simultaneously
- Creates a collision domain

**Collision Domain**: A network segment where only one device can communicate at a time. Multiple simultaneous transmissions cause interference, requiring retransmission.

### Switch (Switching Hub)

- Data link layer device (Layer 2)
- Similar to hub but more intelligent
- Can inspect Ethernet protocol data
- Determines intended recipient and sends data only to that system
- Reduces/eliminates collision domains
- Results in:
  - Fewer retransmissions
  - Higher overall throughput

### Router

- Network layer device (Layer 3)
- Forwards data between independent networks
- Stores internal routing tables
- Types:
  1. **Home/Small Office Routers**
     - Basic routing tables
     - Forwards traffic to ISP
  2. **Core ISP Routers**
     - Forms Internet backbone
     - Handles complex routing decisions
     - Multiple connections to other routers

**BGP (Border Gateway Protocol)**: Protocol that allows routers to share data and learn optimal traffic paths.

## Network Concepts

### Node
- Any device connected to a network

### Server vs Client

| Role | Description |
|------|-------------|
| Server | Provides data to requesting devices |
| Client | Receives data from servers |

**Important Notes:**
- Programs on the same node can be servers and clients to each other
- Most devices function as both server and client at different times
- Devices are typically primarily one or the other
- Primary purpose determines classification (e.g., email server)

### LAN (Local Area Network)
- Network of devices in a limited geographical area

## Network Engineering

Network engineers design the infrastructure of the Internet, similar to how civil engineers design roads.