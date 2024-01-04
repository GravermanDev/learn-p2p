# Part 0 - theoretical bullsh*t
This is the beginning of my series on peer-to-peer networks in Rust.

## Video script
After this video, you'll understand the basic theory behind peer-to-peer networks. Today, I'll go over some of the protols very briefly explaining what they do, however in future videos I'll go deeper into the interesting concepts and actually code them.

It's important to note that this is also something new to me and I will make mistakes. Hopefully we can all learn, and maybe make a community project if the channel continues to grow. Let's get into it.

### **What are peer-to-peer networks?**
A peer to peer network is a network distributed decentrally over different machines. Instead of a centralized server, that every client connects to, users form a network of nodes that can communicate. This has multiple advantages, the main technical one being there is no need for a big centralized server that can often be a bottleneck in internet speeds, but also the failure of one computer won’t disrupt the entire of the system. These networks also scale better in terms of cost, because it's the users maintaining it collectivly.

The more social reason for peer to peer networks, is that no one group controls the system, these networks can allow for a more democratic control over the internet. This can be very important in many cases, for example in fight agaist oppression. There are multiple anti-authoritarian groups using these tools to rebel agaist repressive governments. I'm actually very interested in social implications of different technologies, so if you want my take on tech such as AI or peer-to-peer networks, I'll be glad to give some of my radical ideas here.

### **The Internet Protocol (IP)**
Before diving into the protocols of peer-to-peer networks, let's start with the basics of the internet, as they will be needed for future episodes. This applies to all types of networks, not just peer-to-peer. For those familiar with IP/TCP, feel free to skip ahead.

The Internet Protocol, or IP for short, is a set of rules that govern how machines communicate over a network. It's a crucial component of the TCP/IP protocol suite, which forms the foundation of the Internet. IP enabled computers to connect and communicate on a massive scale. Imagine a region with an established internet infrastructure. Here, IP facilitates the exchange of data by assigning IP addresses to each device on the network. Routers, using these addresses, determine the best path to forward packets to their destination. There are two versions of IP in use: IPv4 and the newer IPv6, which was developed to address the issue of IPv4 address exhaustion, most of the internet still uses IPv4.

### **TCP Protocol**
While IP allows us to send packets, which are small bits of data, typically a few hundred bytes in size, what happens when we need to send larger files, like videos? TCP works on top of IP and is designed for the reliable and ordered delivery of a stream of packets on the internet. It ensures that large files are split into manageable packets, transmitted, and then correctly reassembled at the destination. If a packet is lost during transmission, TCP detects this and resends the lost packet. Furthermore, TCP is responsible for flow and congestion control, ensuring that data transmission is efficient and adapts to varying network conditions.

I haven't watched the entire series yet, but I can comfortably recommend [this](https://youtu.be/bzja9fQWzdA) series about implementing TCP for the ones that know low-level linux.

### **p2p protols**
Let's now go over some of the interesting protols used in p2p networks, again, this will be a brief introduction, as we will dive deeper later.

### 
