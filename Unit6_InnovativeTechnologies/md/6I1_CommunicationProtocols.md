<iframe src="../assets/header.html" width=100% height=28></iframe>

<!-- ######################################### -->

#Communication Protocols


##The Importance of Protocols

<div class="cBox">
<b>protocol</b><br>
<blockquote>
A set of formal standards that specify the proper formatting of data, communication procedures, and handling of information between any two networked components.
</blockquote>
</div>

The processes involved in browsing a webpage, sending an email or text message, or uploading a photo to an online service all seem relatively straightforward and simple. You click on a link and the webpage loads in your browser. You type your message and click `Send`. Or you tap the `Share` icon and select your favorite social media site and after a few seconds, your photo just magically appears online. It is all so very simple. Except that, behind the scenes, it is not simple at all.

Every time you perform one of these actions as a user, you set off a chain reaction of complex data processing and information exchange within dozens, if not hundreds, of separate computational devices across the breadth of the internet. In these examples, the software running on your computer, phone, tablet, or other computing device responds to your clicks and taps by initiating a multi-stage network transmission in which your data hops from node to node as it is handed off from one router or hub to the next until it finally reaches an appropriate server on the other end. In each of these hops, where your data is transmitted between two nodes, the exchange of information is made possible through the use of standard, agreed-upon communication protocols that each node follows precisely.

These protocols, or sets of rules for the proper handling and formatting of information, are designed to establish a common interface through which different hardware/software components can interact, regardless of their own internal design or manufacturer.

In the case of communication protocols, abstraction allows for a clear set of standards for how information should be exchanged to be explicitly described while avoiding the complexity and minutiae of how a manufacturer might actually implement that standard in their hardware or software. By describing the standards broadly, abstraction also enables future innovation by not limiting or restricting the kinds of hardware that can implement the standards. As long as it conforms to the expected protocols, any type of compatible component can be developed to participate in the exchange of digital information on the internet.


##Standard Protocols

Throughout the history of the internet, as technologies have evolved, a number of standards have been developed to ensure the efficiency and robustness of these new capabilities. Traditionally, the task of developing these communication protocols falls on the shoulders of independent researchers who develop the protocols and ad hoc standards committees, often made up of experts and organizations who have a vested interest in the proper functioning of the internet as a whole. Together these committees agree upon and oversee application and further refinement of existing protocol standards.

Designing and developing a protocol is no easy task. Any agreed-upon standard needs to 1) enable reliable and efficient transmission of data at large and small scales, 2) provide an unambiguous set of protocols, and 3) be flexible enough to adapt to and accommodate future technological innovations.

Several of the most commonly used protocols include those for internet data transmission (IP, TCP, UDP), e-mail (SMTP), webpages (HTTP, HTTPS), and files (FTP). Using the notion of abstraction, the internet protocol suite, more commonly known as TCP/IP, organizes each of these into a stack of distinct layers based on the hierarchical relationships of their use. These include the _link_, _transport_, _internet_, and _application_ layers.

But communication protocols are not just limited to the Internet as a whole. A number of independent, privately owned platforms also offer protocols for publicly integrating third-parties into their networks through the use of API's (_application program interface_).

For example, when Twitter first launched in 2006 as a private messaging service, it was built around the SMS text messaging standards (whose protocol limits messages to 160 characters). Twitter's protocol limited its own messages to 140 characters, using the remaining 20 characters to convey meta information about the message (e.g., user id of the sender, etc.). However, Twitter's initial growth benefited from their offering of a public API that allowed countless third-party developers to create their own innovative applications. By following the protocols laid out in the API, these applications could tap into the Twitter backbone to send and retrieve tweets.


##The Link Layer

These standards specify the protocols for establishing the physical (and wireless) connections between end-point devices.


**Ethernet ([IEEE 802.3](http://standards.ieee.org/about/get/802/802.3.html))**

This protocol specifies the use of physical, short-range connections commonly used in local area networks (LAN), such as homes or offices, which uses coaxial cable, twisted pair, or fiber optic connections. You will often see these types of connections between a cable modem and a wireless access point or router or between  a desktop computer and a wall outlet (which ultimately connects elsewhere to a modem).


**Wireless LAN ([IEEE 802.11](http://standards.ieee.org/about/get/802/802.11.html))**

802.11 is the standard wireless protocol for Wi-Fi communications seen in most laptops, phones, tablets, and other networked devices that are not physically connected to a network.


**Bluetooth ([IEEE 802.15.1](http://standards.ieee.org/about/get/802/802.15.html))**

Bluetooth is another wireless connectivity protocol intended specifically as a _peer-to-peer_ connection between two close-range devices. The protocol specifies procedures for two devices to be "paired" with one another so that they can securely exchange data over the air, without the need for a physical connection.


##The Transport Layer

These standards specify the protocols for how data is transmitted through the network.


**Transmission Control Protocol ([TCP](https://tools.ietf.org/html/rfc793))**

The TCP protocol ensures that all packets of a data stream are transmitted and received exactly as originally sent. It specifies methods of performing error-checking analysis of the received packets to ensure that no error or loss of information was introduced along the way. If a packet is lost or found to be damaged, the TCP protocol will identify the error and request that the packet be resent. TCP is most suited for applications that prioritize accuracy and completeness of transmission over speed, such as e-mail (SMTP), webpages (HTTP, HTTPS), and file transfer (FTP).


**User Datagram Protocol ([UDP](https://tools.ietf.org/html/rfc768))**

The UDP protocol is better suited for applications in which speed is more important that accuracy or completeness of information, such as online gaming or video or audio streaming.


##The Internet Layer

These standards specify the protocols for how individual datagrams (i.e., packets) are packaged and labeled for delivery over the network.


**Internet Protocol ([IP](https://tools.ietf.org/html/rfc791))**

Originally developed as part of the _Transmission Control Program_ in 1974 and then later separated out as its own standard, the Internet Protocol (IP) specifies  how individual packets of information are packaged and labeled for delivery, much like the way that the postal service specifies how envelopes and packages should be sized, addressed, and stamped.


##The Application Layer

These standards specify the protocols for handling data that is designed for specific use-cases, such as e-mail (SMTP), the World Wide Web (HTTP, HTTPS), or raw file handling (FTP).


**Simple Mail Transfer Protocol ([SMTP](https://tools.ietf.org/html/rfc821))**

This protocol specifies how electronic mail should be formatted in order to be sent and routed to the intended recipient. Most notably, the standard specifies how header information may be prepended to the beginning of a message by each node that handles the message along the way. Users who receive an e-mail can view the headers of the full message once they receive it to see various information about where the message came from and through which server it originated from and those that it passed through on its way to their inbox.


**Hypertext Transfer Protocol ([HTTP](https://tools.ietf.org/html/rfc2616), [HTTPS](https://tools.ietf.org/html/rfc2818))**

These are the primary tranport protocols used by the World Wide Web for delivering web content. The protocol was designed to transmit hypertext documents that have been formatted according to another protocol, HTML (Hypertext Markup Language). The "S" at the end of "HTTPS" indicates "Secure" and provides additional protocols and procedures for encrypting information prior to transmission and decrypting it upon receipt.

Other common protocols in the application layer include the **File Transfer Protocol ([FTP](https://tools.ietf.org/html/rfc959))** for sending files, **Domain Name System ([DNS](https://tools.ietf.org/html/rfc1034))** for looking up IP addresses of domains, **Dynamic Host Configuration Protocol ([DHCP](https://tools.ietf.org/html/rfc2131))** for initializing an Internet connection with an ISP, and **Post Office Protocol ([POP](https://tools.ietf.org/html/rfc1939))** and **Internet Message Access Protocol ([IMAP](https://tools.ietf.org/html/rfc3501))** for storing/retrieving e-mail messages.






<!-- ######################################### -->

<iframe src="../assets/footer.html" width=100% height=60></iframe>
