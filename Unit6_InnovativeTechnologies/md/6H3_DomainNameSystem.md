<iframe src="../assets/header.html" width=100% height=28></iframe>

<!-- ######################################### -->

#Domain Name System


##The Internet's Directory Assistance

Every website is essentially a collection of content stored on a web server. Every web server is just a program running on an internet-connected computer. Every internet-connected computer is a networked node. And every networked node is assigned an IP address that identifies where it can be found on the network. So, it is reasonable to conclude that every website can be identified by its 32-bit IP address.

But how often have you ever entered an IP address into your browser? How often do you see any IP address in the address bar as you browser the Web? For most people, the answer to these questions is "rarely, if ever." Instead of IP addresses, most users rely on the use of _domain names_ to reference an online site or service. And the Domain Name System is the hidden service quietly working in the background that makes it all possible.


##Domain Names

The fact is that a 32-bit number, while perfectly ideal for the digital and electronic components of the routers and other computational devices that support the Internet, is not very human-friendly. Which of the following is more intuitive for humans?

+ `01000010110111001001111001000100`

+ `	66.220.158.68`

+ `facebook.com`

The first is an actual 32-bit address. The second is that same address expressed in a more human-friendly format of four octets. The last version, however, is the most recognizable of the three because it is descriptive and tells us everything that we, as humans, would want to know &mdash; namely that it refers to the Google search engine.

Numbers are great ways of cataloging and indexing things. People have Social Security Numbers, the products we buy have Universal Product Code (UPC barcodes), books have International Standard Book Numbers (ISBN), credit cards and bank accounts are numbered, drivers licenses have numbers, etc. But these numbers are meant for automated systems to store and process computationally. We prefer to call each other by our first and last names, products by their brands, and books by their titles. So it comes as no surprise that we would prefer to reference our favorite websites by descriptive names rather than an obscure and seemingly arbitrary sequence of numbers.


##DNS Lookup

When you type a URL into an address bar, it is usually in a form that includes a domain name. For example:

	https://www.facebook.com/

But how does this translate into an IP address that your computer and all of the intermediate routers and gateways can use to locate the actual Google server that hosts the page you are trying to load? The answer is a massive _lookup table_ that acts like a large directory, dictionary, or phonebook that allows you to use a value that you do know to look up a value you do not know.

When you try to load a webpage, your web browser (e.g., the client) isolates the domain name specified in the URL you typed (e.g., "facebook.com") and sends that name to a special server known as a Domain Name Server (DNS). That is, the browser sends a request to a pre-configured IP address that corresponds to the location of a nearby nameserver (usually belonging to your ISP, although Google actually operates a couple handy nameservers at `8.8.8.8` and `8.8.4.4`).

The nameserver, which is a computer that stores an updated list of every registered domain name and the IP address of the server that hosts that domain, looks up the address of requested domain name and sends that information back to your web browser.

Your web browser then sends the URL of your original page request to the IP address that it received from the nameserver.

Without a centralized name server at a known IP address, your browser would have no way of knowing which IP address it should contact to fulfill your page request.





<!-- ######################################### -->

<iframe src="../assets/footer.html" width=100% height=60></iframe>
