# Part 1 - basics
This is the beginning of my series on peer-to-peer networks in Rust. The source code in this folder runs a simple `chat` example in libp2p.

## Video script
In this video I will show you the bacics of peer-to-peer networks, building a teminal chat app. I'll give you actual examples in Rust code, with a library libp2p, however this knowledge will apply to other languages. I aim to make this a series, after which we can all develop decentralized systems.

It's important to note that this is also something new to me and I will make mistakes. Hopefully we can all learn, and maybe make a community project if the channel continues to grow. Let's get into it.

### **What are peer-to-peer networks?**
A peer to peer network is a network distributed decentrally over different machines. Instead of a centralized server, that every client connects to, users form a network of nodes that can communicate. This has multiple advantages, the main technical one being there is no need for a big centralized server, that can often be a bottleneck in internet speeds. Also the failure of one computer won’t disrupt the rest of the system. This just clearly scales batter and reduces the costs sigificantly

The more social reason for peer to peer networks, is that they are decentralized, meaning no one group controls the system. This can be very important in many cases in fight agaist oppression. And I personally know anti-authoritarian groups using these tools to rebel agaist repressive governments. I'm actually very interested in social implications of different technologies, so if you want my take on tech such as AI or peer-to-peer networks (and why they should be connected), I'll be glad to give some of my radical ideas here.

### **Back to the technical shenanigans**
Since peer to peer has no centralized sever, it uses protocols to coordinate work. There are different protocols that can be used. Ranging from social media to filesharing and also blockchain. We will utilize a library called libp2p in Rust to make these protocols. Before we get into the coding, let's look at the key features of libp2p, at least the ones we will be using.

### Addressing
Addresses in libp2p are stored in multiaddress format, let's go over it real quick.

Mutliaddr supports multiple protocols, every protocols can be written like this:
 - ip4/198.51.100
 - tcp/1234
 - https/

The main advantage of multiaddr is that these adresses can be composed. We will look at a simple example of TCP/IP. When we want to send some data to a different computer, we can use the Internet Protocol (IP). IP allows us to send packets, which are these small bits of data, usually couple hundred bytes, but what if we want to send a video? A TCP protocol splits big files into packets and sends them in a way that doesn't corrupt the entire file, it also takes into considuration packet loss and allows for multiple connections, because each connection has it's unique port. What multiaddr does is allow us to store protocols as instructions. For instance ``ip4/198.51.100/tcp/1234`` tells us to send the data to this IP address under this TCP port. We can have multiple connections between to computers, like this: ``ip4/198.51.100/tcp/1234``, ``ip4/198.51.100/tcp/2137``.

## mDNS


### Swarm
Swarm contains the behaviour that the local node should have, as well as it's local state, meaning all the information that local node has. The behaviour is stored in two traits:
 - NetworkBehaviour, which defines what data to send and to whom this data should be sent.
 - Transport which defines how to send the data

## gossipsub


### **Now let's look at the code!**


### Conclusion
In next videos we will continue working on peer to peer networks. I'm thinking of a chat application made with libp2p. Let me know what you think, see ya.
