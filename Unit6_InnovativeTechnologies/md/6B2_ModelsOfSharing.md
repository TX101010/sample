<iframe src="../assets/header.html" width=100% height=28></iframe>

<!-- ######################################### -->

#Models of Sharing


##It's All About Who You Know

Whether you are a developer of a social network or merely one of the countless users of such a network, it is important to recognize that not all social structures are the same. There are many different types of relationships that individuals might have with one another and there are many different ways that they might want to either limit or encourage interaction between each other.

For example, there are many different ways of "knowing" somebody. You might _know about_ George Washington or Thomas Jefferson from history class, but do you _know_ them personally? Likely not, as they both died over 200 years ago. Similarly, you might _know_ your school counselor, nurse, or principle, but do you _know_ any of them outside of school? Better still, do any of them _know_ you? And if so, to what degree? The school nurse might know about your peanut allergy, but does she know what you did on you last family vacation or the name of your favorite author or musical artist? What about your best friends? How well do they _know_ you? How well do you _know_ them? Do you share everything? Or do you only share some things? Likely, you choose to share a limited set of details with certain individuals or groups while sharing a different subset of your life with other individuals or groups.

Today's most popular online social networks and self-publishing platforms exhibit this diversity of "knowing" in their very design. Each service is designed to model a very specific form of relationship that you or anybody else might have in your everyday, offline lives.



##Public vs. Private Communication

There is an idiom that refers to the difficulty of "putting the genie back in the bottle." The idea is that once a particular event is done, it cannot be undone. Information works in the same way. Once a bit of information is distributed and known by others, it is virtually impossible to retract that information and force it to once again become "unknown." This makes the issue of _privacy_ a critical factor in our globally connected, digital world. The technology makes it easy to share information with a wide array of individuals. Usually that is seen as one of the strengths of the internet, but it also serves as one of its drawbacks as information may be shared (or even _re-shared_) in ways that were never intended.

When it comes to designing or using a social network, it is critical to understand how the service might handle the issue of privacy. On one end of the spectrum, a service might choose to make all information publicly available to _anybody_ at _any time_. At the other end of the privacy spectrum, all information is securely locked down and made available only to the owner or creator of the information. The very nature of a "social" medium that involves the interaction and exchange of ideas between multiple people would suggest that the latter extreme is inappropriate for such a service. However, the former extreme in which everything is publicly accessible might be too public. Most cases call for a solution that falls somewhere in between the two extremes. That is, users usually want to be able to restrict what they share to their intended audience on more of a case-by-case basis.

**Public**<br>
In its original conception, the World Wide Web was seen as a tool for facilitating a one-to-many publishing platform. Website authors would publish their content where it would be _publicly_ hosted on a web server that anybody with a web browser could access and retrieve a copy of the published materials. By default, the content hosted at a web site was to be considered completely public (i.e., available to anybody at any time).

**Private(ish)**<br>
On the other hand, the email (or "electronic mail") protocol was designed to facilitate _private_ communication. That is, email is shared communication that is intended only for the very specific recipient(s) to which it is sent. Ironically, while access to an email message is usually limited to the recipient, the [Simple Mail Transfer Protocol (SMTP)](https://tools.ietf.org/html/rfc821) that defines how all email transmission is handled, actually does not ensure total privacy. In fact, as an email message is transmitted from node to node throughout the public network of routers and gateways across the internet, the contents of the messages are exposed in plaintext. In real-world terms, email is _private_ in the way that a postcard sent through the US Postal Service is _private_ &mdash; in the end, only the addressee receives the card, but any mail handler who looks at the back of the card can see and read its contents.

**Private**<br>
A better example of truly _private_ communication (to the extent that that is not an oxymoron) might be Skype or Google Hangouts. Like email, these forms of communication allow one individual to specify their intended contact(s) and limit the conversation to just those parties. Unlike email, however, these video chat services employ encryption so that the digital information that makes up the audio and video signal is encoded before it is transmitted across the internet and then decoded only after it reaches its destination. This means that the two people on either end of the conversation can see and hear everything being said, but for any eavesdropping router along the way between them, the signal will be unintelligible. In this case, the use of _encryption_ is the key factor that enables true privacy with video chat systems. However, this does not prevent either party on either end of the conversation from recording the chat session and later sharing it with others &mdash; a privacy vulnerability that even something like Snapchat cannot solve. 


##Symmetric vs. Asymmetric Relationships

Consider the differences between your relationship with your best friend versus the relationship you have with your favorite Hollywood celebrity. In your friend's case, the friendship is likely mutual. That is, each of you considers the other to be their friend. If so, what you have is a _symmetric_ relationship – you like your friend and your friend likes you. However, in the case of the Hollywood celebrity, while you might be a huge fan of theirs, they likely do not even know you exist (sometimes the truth hurts). When a person becomes famous, by definition, it means that millions of people suddenly know who they are. But the reverse cannot be said. Becoming famous does not ensure that the celebrity knows each and every one of their millions of adoring fans. Almost all of those millions of relationships are one-sided. These are examples of _asymmetric_ relationships.

In enabling users to interact with one another, online social networks encourage and regulate the types of activities their users can engage in based on the nature of the type of relationship the network is designed to serve. A symmetric system is built upon the idea that interactions will involve two-way exchanges, often of a more personal nature and in which both parties are more or less peers. In contrast, an asymmetric system assumes a largely one-way flow of information that often involves an impersonal delivery of information.

Which model an online service chooses, whether _symmetric_ or _asymmetric_, will dictate the primary characteristics of the network, the engagements it offers, and the users it aims to serve. And of course, many services that start out as one type might, over time, adopt features of the other type, resulting in a hybrid system that is sometimes symmetric and other times asymmetric.


**Symmetric**<br>
Facebook was built to be a _symmetric_ network. The very idea of "friending" involves mutual actions by both parties in the friendship. One person must first choose to "Add Friend" and then the second person must accept the friend request. Both parties must take action to create the relationship in the Facebook system and both parties then have equal access to the features that such a relationship enables within the Facebook ecosystem. In every way, the relationship is mutual, two-way, and symmetric. Of course, over time, Facebook has added features that introduce more asymmetric behaviors, such as the ability to selectively restrict which friends can see/interact with a post. Nevertheless, the service is still primarily true to its symmetrically designed origins.


**Asymmetric**<br>
Twitter, on the other hand, was built to be an _asymmetric_ network. Unlike Facebook's friend-based approach where all users are on par with one another, Twitter uses a publisher-subscriber model. One user "tweets" (publishes) a message that is then automatically sent to each of their "followers" (subscribers). For public accounts, these relationships are one-way, requiring action by only one party to create the relationship. Namely, the subscriber chooses to "Follow" the posts from another user. Unlike Facebook, the publishing user does not need to "accept" or explicitly permit the relationship to be established. And like Facebook, Twitter has also evolved into a hybrid system that incorporates some symmetric aspects through the use of direct messages, protected accounts, and per-user blocking.


##Open vs. Closed Platforms

The internet as we know it today got its start in the early 1960s as a US Department of Defense project known as ARPANET (Advanced Research Projects Agency Network). For the next 20 years, ARPANET was privately operated by the US military and its use was limited exclusively to government and military applications. Only in the 1980s did the network open up to civilian uses and transition to the free and open internet that we know today.

Together, the ARPANET and internet provide excellent examples of the differences between _closed_ and _open_ systems. Closed platforms are often referred to as being "proprietary" because they are owned, managed, and operated by a single owner or proprietor. While that owner might choose to allow others to access and use their platform, they still maintain final control over the system, how it is used, and how it evolves. Open platforms, however, do not have a single owner calling the shots. Instead, they might have a centralized committee of interested partners to coordinate and manage the development and growth of the platform.

There are advantages and disadvantages to both approaches, but the ultimate choice of whether a platform should be open or closed comes down to the goals that drive the development of the system. In the case of ARPANET, the US military had ample government funding to build and operate the network as well as the need for a secure and reliable means of maintaining communication in the event of a nuclear attack. As such, it was _their_ system that _they_ built with their _own_ funds and for their _own_ needs, so they kept it to _themselves_ (i.e., a _closed_ network). By the 1980s, the technological and economic advantages of making a global, electronic network available to the commercial market merited opening up the network to more civilian uses by business and individuals. 


**Open**<br>
Email and web publishing are both examples of open platforms that have been created around open standards. Any developer can create an email application that conforms to the various standards for handling email ([SMTP](https://tools.ietf.org/html/rfc5321), [POP](https://tools.ietf.org/html/rfc1939), [IMAP](https://tools.ietf.org/html/rfc3501)). The program can then send email to and receive email from any other email user anywhere on the internet no matter which email client (program) they might be using. Without these open standards, there would be no guarantee that any message that you write and send would be compatible with the software being used by your intended recipient. But with these standards, all emails created by any standards-compliant email client are guaranteed to be fully compatible with all other such clients, thus enabling the global communications system that we have come to rely on.

**Closed**<br>
While services like Facebook and Twitter might be publicly available and free to use, they are still closed, proprietary systems. Each company controls the data that they store and strictly regulates how that data can be accessed and modified by its users. For example, users cannot easily transport their tweets, status messages, comments, chat histories, or friends lists to other competing services. Similarly, the ability to integrate these services into other, third-party apps or sites is strictly limited to what Facebook or Twitter choose to allow. Having this level of control over their platform gives each company the ability to more reliably build, develop, and monetize their platform, but it comes at the expense of user choice and compatibility.



##Assignment

As a class, make a list of all of the different services and methods that people can use to communicate and/or interact with one another online. Then, working in pairs, decide whether you would classify each of the services as either public or private, open or closed, and symmetric or asymmetric. Be prepared to explain and defend your choices.

| Service | Public/Private | Symmetric/Asymmetric | Open/Closed |
|:-------:|:--------------:|:--------------------:|:-----------:|
| email   |     private    |      asymmetric      |    open     |
| Facebook|     private    |      symmetric       |   closed    |
| Twitter |     public     |      asymmetric      |   closed    |


<!-- ######################################### -->

<iframe src="../assets/footer.html" width=100% height=60></iframe>
