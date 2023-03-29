## 9 - Recap: TCPIP and DNS
**Informational**
> *LETS break TCP/IP*

Welcome to Day 09 :smile:!!!

![](../assets/Day09-%2070DaysofServicemesh.png)

 ### What is TCP/IP?
 

 TCP stand for **(Transmission Control Protocol)**. This is responsible for ensuring that data is transmitted reliably and in the correct order, while IP **(Internet Protocol)** and it is responsible for routing the data to its destination.

 >**Note:** The TCP/IP model consists of four layers. The following layers are

### 1 Network Access Layer
The network access layer, also known as the data link layer, handles the physical infrastructure that lets computers communicate with one another over the internet. This covers ethernet cables, wireless networks, network interface cards, device drivers in your computer, and so on.

The network access layer also includes the technical infrastructure — such as the code that converts digital data into transmittable signals — that makes network connection possible.

### 2 Internet Layer
The internet layer, also known as the network layer, controls the flow and routing of traffic to ensure data is sent speedily and accurately. This layer is also responsible for reassembling the data packet at its destination. If there’s lots of internet traffic, the internet layer may take a little longer to send a file, but there will be a smaller chance of an error corrupting that file.

### 3 Transport Layer
The transport layer provides a reliable data connection between two communicating devices. It’s like sending an insured package: The transport layer divides the data in packets, acknowledges the packets it has received from the sender, and ensures that the recipient acknowledges the packets it receives.

### 4 Application Layer
The application layer is the group of applications that let the user access the network. For most of us that means email, messaging apps, and cloud storage programs. This is what the end-user sees and interacts with when sending and receiving data.

>Which IP addresses do TCP/IP work with?

Whether you have an IPv4 or IPv6 address that's mean you’re already using the TCP/IP model. This is the standard model for most existing internet infrastructure. 

### How TCP/IP relate to DNS?

TCP/IP and DNS work together to enable users to access websites by translating domain names into IP addresses and then transmitting data over the internet using the TCP/IP protocol.

TCP/IP and DNS are two fundamental protocols that work together to make the internet work. TCP/IP provides the underlying transport mechanism for transmitting data over the internet, while DNS provides the system for translating domain names into IP addresses that can be used by TCP/IP to route data.

When a user wants to access a website, they type the domain name into their web browser. The browser sends a DNS query to a DNS server to obtain the IP address associated with that domain name. Once the IP address is obtained, the web browser uses TCP/IP to establish a connection with the web server associated with that IP address. The TCP protocol is responsible for ensuring that data is transmitted reliably and in the correct order, while the IP protocol is responsible for routing the data to its destination.