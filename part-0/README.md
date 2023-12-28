# Part 0 - theoretical bullsh*t
This is the beginning of my series on peer-to-peer networks in Rust.

## Video script
After this video, you'll understand the basic theory behind peer-to-peer networks. Today, I'll show you how all of this works on paper, however in future videos I'll explain actual code examples in the Rust programming language. 

It's important to note that this is also something new to me and I will make mistakes. Hopefully we can all learn, and maybe make a community project if the channel continues to grow. Let's get into it.

### **What are peer-to-peer networks?**
A peer to peer network is a network distributed decentrally over different machines. Instead of a centralized server, that every client connects to, users form a network of nodes that can communicate. This has multiple advantages, the main technical one being there is no need for a big centralized server that can often be a bottleneck in internet speeds, but also the failure of one computer won’t disrupt the entire of the system. These networks also scale better in terms of cost, because it's the users maintaining it.

The more social reason for peer to peer networks, is that no one group controls the system, these networks can allow for a more democratic control over the internet. This can be very important in many cases, for example in fight agaist oppression. There are multiple anti-authoritarian groups using these tools to rebel agaist repressive governments. I'm actually very interested in social implications of different technologies, so if you want my take on tech such as AI or peer-to-peer networks, I'll be glad to give some of my radical ideas here.

### **The Internet Protocol**
Back to the theory. Let's first examine the basics of internet, so we can understand how networking works in general, this applies to all kinds of networks, not just p2p. 

The Internet Protocol, in short IP, is a protocol, meaning it is a set of rules that allow machines to communicate with each other. The Internet Protocal was revolutionary because it allowed computers to communicate on a massive scale. Imagine this is a region with an internet infrastructure set up like this. IP enables networks to send packets, to each other. The way it works is by giving individual devices an IP address. Next routers a table of how to get to some address. The packets navigate the network based on the protocol, and they get to the destination.

### **TCP protocol**
IP allows us to send packets, which are these small bits of data, usually couple hundred bytes, but what if we want to send a video? The TCP protocol splits big files into packets and sends them in a way that doesn't corrupt the entire file, after that it instructs the computer on how to reconstruct the files. While doing all of that, it deals with packet loss and also allows computers to have multiple connections with each other.
