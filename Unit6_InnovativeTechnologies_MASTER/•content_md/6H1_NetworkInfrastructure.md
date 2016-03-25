<iframe src="../assets/header.html" width=100% height=28></iframe>

<!-- ######################################### -->

#Network Infrastructure


##Network Architecture


In its simplest form, the internet is just a large collection of interconnected devices. Some of the devices are connected directly to one another while others are only connected indirectly through a series of intermediate devices. Altogether, these devices make up the network. They consist of all varieties of electronic, computational hardware, including desktop computers, laptops, tablets, phones, printers, cameras, routers, Wi-Fi access points, etc.

Through this arrangement of interconnectedness, any two devices are able to "communicate" with one another by transmitting a digital signal along the appropriate medium (e.g., copper wire, fiber optic cable, radio wave transmission, etc.) that makes up that connection.

One of the strengths of the internet's design is the inherent redundancy that such a complex and multiply connected network offers. In most cases, there is more than one pathway through which a transmission can be sent in order to reach its destination. This allows the network to not only be fast and efficient by finding the most optimal route, but also robust enough to continue functioning even if part of the network fails and a pathway is cut off.



##Client-Server Model

The basic operation of any networked communication system centers on the transmission of information between two parties. Traditionally, these parties are referred to as the "client" and the "server."

Typically, the _client_ initiates the communication by sending a request to the _server_ &mdash; usually a fully automated program running on a remotely located computer &mdash; which then processes the request and sends the appropriate response back to the _client_. Examples of client software that users might be familiar with include web browsers, e-mail applications, and chat programs. 

When a user clicks on a link in a browser, a URL (i.e., the address of a web page) request is sent out into the larger network, where it is then routed to the location of the particular computer that is running a web server for the requested URL. The server then generates the content for the page (formatted in HTML) and transmits it back through the network to the user's computer. The web browser (i.e., the client) then interprets the HTML information that it receives and uses that to render the text and images onto the users screen.

In some use-cases, the _server_ might initiate the communication in what is referred to as a "server-side _push_" (in contrast to the "client-side _pull_" described above). In a "push" situation, a centralized server _pushes_ information out to one or more clients without the end-user explicitly requesting the information.

A chat program is example of an application that makes use of both "client-side pull" and "server-side push" transmissions. In a situation where two users are messaging with one another, they are each operating an application that is functioning as a _client_ and are remotely communicating with a central _server_ located somewhere on the larger network. The server effectively sits in between these two users, relaying their messages from one to the other. When one user sends a message, the contents of the message as well as delivery instructions are sent to the server, which is listening for such an incoming transmission. The server then interprets the delivery instructions to identify which user the message is intended for. The _server_ then initiates a transmission in which the message is "pushed" to other user's _client_, which renders the message on their device as an incoming message from the first user.


##Nodes, Gateways, and Routers

The overall structure of a communications network, through which all digital traffic flows, consists of a number of _nodes_. Each node is a machine or device that acts as either a communication endpoint (e.g., a _client_ computer or a remote _server_), a connection point that links together two other nodes (e.g., a _gateway_, _bridge_, or _modem_), or a redistribution point that links together multiple nodes and other networks (e.g., a _router_, _hub_, or _switch_).




<!-- ######################################### -->

<iframe src="../assets/footer.html" width=100% height=60></iframe>
