# Part 1 - basics
This is the beginning of my series on peer-to-peer networks in Rust. The source code in this folder runs a simple `ping` example in libp2p.

## Video script
In this video I will show you the bacics of peer-to-peer networks. I'll give you actual examples in Rust code, with a library libp2p, however this knowledge will apply to other languages. I aim to make this a series, after which we can all develop decentralized systems.

It's important to note that this is also something new to me and I will make mistakes. Hopefully we can all learn, and maybe make a community project if the channel continues to grow. Let's get into it.

**What are peer-to-peer networks?**

A peer to peer network is a network distributed decentrally over different machines. Instead of a centralized server, that every client connects to, users form a network of nodes that can communicate. This has multiple advantages, the main technical one being there is no need for a big centralized server, that can often be a bottleneck in internet speeds. Also the failure of one computer won’t disrupt the rest of the system. This just clearly scales batter and reduces the costs sigificantly

The more social reason for peer-to-peer networks, is that they are decentralized, meaning no one group controls the system. This can be very important in many cases in fight agaist oppression. And I personally know anti-authoritarian groups using these tools to rebel agaist repressive governments. I'm actually very interested in social implications of different technologies, so if you want my take on tech such as AI or peer-to-peer networks (and why they should be connected), I'll be glad to give some of my radical ideas here.

Back to the technical shenanigans.