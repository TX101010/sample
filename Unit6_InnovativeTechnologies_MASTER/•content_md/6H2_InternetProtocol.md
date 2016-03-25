<iframe src="../assets/header.html" width=100% height=28></iframe>

<!-- ######################################### -->

#Internet Protocol


##A Protocol for Packet Network Intercommunication

When Vint Cerf and Bob Kahn first proposed the _Transmission Control Program_ in 1974, it established the use of a technique, known as _packet switching_, as the underlying method of transferring data between nodes across the Internet.

With packet switching (or packet _routing_), all data is subdivided into small, suitably sized blocks that are then transmitted independently from one another, potentially taking different routes to reach the data's intended destination. Rather then sending an entire message of some arbitrary and varying length all at once and hoping that it reaches its destination intact, larger messages are broken up into smaller, fixed-size _packets_.

Each of these packets contains two components: a _header_ and a _payload_. The header contains the IP addresses of the source node (e.g., the sending client) and the destination (e.g., the receiving server) and any other information needed to deliver the packet. The payload is the actual data that is being sent.

In a real-world example, the process of sending digital information across a network is a lot like mailing a document across the country via postal mail. The sender seals the document (the _payload_) in an envelope or box (the _header_) upon which is written the return address (_source_ IP address) and the recipient's address (_destination_ IP address). Delivery of the package involves handing it off through a series of many postal carriers and routing systems (_nodes_) as they transport the package to where it needs to go.

By sending data as individualized packets of information, the internet is able to operate more efficiently and is better able to handle unforeseen errors in transmission.

Imagine sending a very large document consisting of thousands of pages. If sent all at once as a single document, any single error, delay, or misdelivery along the way will require the entire document to be resent in full. However, if each page of the document was individually sent, any misdelivery will require only that particular page to be resent. In addition, as the amount of data traffic varies over time, different routes might become faster than others. By sending the larger document as many smaller pieces, each piece can be routed along the most optimal path at that moment. Together these advantages of packet switching serve to improve the speed, efficiency, and reliability of the communication network.


##IP Addresses

The relative location of each node on the network is specified by the node's IP address, a unique numerical identifier, that allows other nodes to know which nodes they are directly connected to and to determine a route for sending data to its intended destination. In the case of the internet, the people who designed the network devised a system for assigning unique 32-bit numbers to each device on the network.

For example, as of 2016, the address for the [google.com](https://google.com) search engine is [`74.125.224.72`](https://google.com). What this means is that when you _"Google something,"_ your browser (i.e., your _client_) sends a search request through the internet's network of nodes, addressed to a _server_ located in some far-off location whose IP address just happens to be `74.125.224.72`.

As devices are added to the network, each is assigned an IP address that translates roughly to its geographic location on the network. More precisely, the Internet Assigned Numbers Authority (IANA) oversees the distribution of these addresses through a number of regional registries. Each registry then assigns blocks of addresses to different entities, like your local internet service provider (ISP), which then assigns an available address from that block to each computer or device that connects through its service.

As a result, while each IP address can provide a general sense of the geographic location of the organization that a node is associated with (e.g., your local ISP), the actual address does not specifically locate the actual node itself. For example, two computers with very similar IP addresses from the same block of numbers might actually be physically located across town from one another and have nothing in common other than they both use the same ISP for internet connectivity.


##IPv4 ("Internet Protocol, version 4")

An IP address is usually expressed in human-readable form as a series of four numbers, each within the range of `0` through `255`, separated by periods (e.g., `123.45.67.89`). That is, the lowest possible numerical value for any address would be `0.0.0.0` and the highest possible value would be `255.255.255.255`.

Each of these four numbers is referred to as an _octet_ because they each represent _eight_ bits (or _binary digits_) of information. In **Unit 2: Data Representation**, we looked  at binary numbers and how they correspond to the decimal (base-10) numbers that you are more familiar with and we will see why eight bits of data can only represent values between `0` and `255`. Suffice to say, four octets of eight bits each adds up to 32 bits of total information that can be used to identify each node on a network.

Just like there is a limit to the range of possible values that can be represented by 8 bits of data (e.g., `0` &ndash; `255`),  there is a similar limit to what can be represented by 32 bits of information (e.g., `0` &ndash; `4,294,967,296`). That means that the internet, as originally designed, can only generate 4.3 billion unique, 32-bit addresses, which limits the internet to a maximum capacity of no more than 4.3 _billion_ nodes. While that is a _lot_ of devices, that number is still finite and can easily run out. In fact, it already has in some areas. APNIC (the Asia Pacific Network Information Centre), the registry organization for the Asia Pacific region, exhausted its pool of regional addresses in 2011. Then, in the fall of 2015, the American Registry for Internet Numbers (ARIN), the registry organization that assigns address for the United States, Canada, the Caribbean, and North Atlantic islands issued the last of its unassigned addresses.


##IPv6 ("Internet Protocol, version 6")

While most internet traffic today uses IPv4 as its addressing standard (and will likely continue for some time to come), it is gradually being replace by IPv6 ("version 6") due to this issue of limited address capacity. IPv6 solves this problem by using 128-bit addresses &mdash; four times the length of the IPv4 addresses. With 128 bits of data packed into each address, this new standard is capable of sustaining more than 3.4x10<sup>38</sup> individual nodes. That is _340 billion billion billion billion!_ 

But is that _enough_? Well, to put that number in perspective, if every grain of sand on all of Earth's beaches were assigned its own, unique IP address, the IPv6 standard would still allow for 60 quadrillion more similar Earthlike planets each with their own IP-enabled beach sand to have their own, unique addresses. In other words, while that number, too, is finite, it is reasonable to say that yes, it most likely is _enough_.



<!-- ######################################### -->

<iframe src="../assets/footer.html" width=100% height=60></iframe>
