# TCP/IP Five-Layer Network Model:

## 1. Physical Layer
The physical layer is a lot like what it sounds. It represents the physical devices that interconnect computers. This includes the specifications for the networking cables and the connectors that join devices together, along with specifications describing how signals are sent over these connections. Physical layer is all about cabling, connectors and sending signals.

## 2. Data Link Layer/Network Interface/Network Access Layer
Responsible for defining a common way of interpreting these signals so network devices can communicate. Lots of protocols exist at the data link layer, but the most common is known as Ethernet, although wireless technologies are becoming more and more popular.

Ethernet standards also define a protocol responsible for getting data to nodes on the same network or link.

Data link layer is responsible for getting data across a single link.

## 3. Network Layer/Internet Layer
That allows different networks to communicate with each other through devices known as routers.
- **Internetwork**: A collection of networks connected together through routers is an internetwork, the most famous of these being the Internet.

Network layer is responsible for getting data delivered across a collection of networks.

E.g: Think of when a device on your home network connects with a server on the Internet. It's the network layer that helps get the data between these two locations.

Most common protocol used at this layer is called IP or Internet protocol.

E.g:
Network software is usually divided into client and server categories, with the client application initiating a request for data and the server software answering the request across the network. A single node may be running multiple client or server applications. So you might run an email program and a web browser, both client applications on your PC at the same time. And your email and web server might both run on the same server. Even so, emails end up in your email application, and web pages end up in your web browser.

The network layer delivers data between two individual nodes.

## 4. Transport Layer
Sorts out which client and server programs are supposed to get that data.
Protocol used in the transport layer is TCP or Transmission Control Protocol.

Other transport protocols also use IP to get around, including a protocol known as UDP or user datagram protocol. 

The big difference between the two is that TCP provides mechanisms to ensure that data is reliably delivered, while UDP does not.

## 5. Application Layer
There are lots of different protocols at this layer, and as you might have guessed from the name, they're application specific. Protocols used to allow you to browse the web or send and receive email are some common ones.

## RWE (Real World Example)
Think of layers like different aspects of a package being delivered. The physical layer is the delivery truck and the roads. The data link layer is how the delivery trucks get from one intersection to the next over and over. The network layer identifies which roads need to be taken to to get from address A to address B. The transport layer ensures that delivery driver knows how to knock on your door to tell you your package has arrived, and the application layer is the contents of the package itself.

---

TCP/IP Model only has four layers, as it doesn't differentiate between the physical layer and the data link layer, but is otherwise very similar to the one we'll be working with.