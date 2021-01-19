CSY2026 Modern Networks
Contents
1. Virtual Demo	1
2. Implementation	4
3. Test	6
References	6


1. Virtual Demo 
• Java TCP Listener <-> Java TCP 

 ![image](https://user-images.githubusercontent.com/58506840/104924738-cfdb5d00-59d8-11eb-9558-68d064a0d93f.png)
 
• Java UDP Listener <-> Java UDP 

 ![image](https://user-images.githubusercontent.com/58506840/104924749-d538a780-59d8-11eb-92a1-d1ed51768143.png)
 
• C# TCP Listener <-> C# TCP 

 ![image](https://user-images.githubusercontent.com/58506840/104924753-d8cc2e80-59d8-11eb-9159-8db2f65d3e93.png)
 
• C# UDP Listener <-> C# UDP 

 ![image](https://user-images.githubusercontent.com/58506840/104924768-dd90e280-59d8-11eb-88e0-9d6d33dd0a44.png)
 
• Java TCP Listener <-> C# TCP 

 ![image](https://user-images.githubusercontent.com/58506840/104924786-e2ee2d00-59d8-11eb-9c0d-a1e443f64896.png)

• Java UDP Listener <-> C# UDP 

 ![image](https://user-images.githubusercontent.com/58506840/104924798-e7b2e100-59d8-11eb-938d-998e91d04914.png)
 
• C# TCP Listener <-> Java TCP 

 ![image](https://user-images.githubusercontent.com/58506840/104924813-eb466800-59d8-11eb-89fe-7eab060c55fe.png)
 
• C# UDP Listener <-> Java UDP

 ![image](https://user-images.githubusercontent.com/58506840/104924829-f13c4900-59d8-11eb-87c4-9dcd831b558b.png)

2. Implementation 
• Java TCP Listener <-> Java TCP 
A client/server application display regularly is seen as a remotely found, powerful figuring gadget that stores a huge amount of information with business rationale to get to them in a system. The UI is taken care of by the customer programming on a moderately modest machine. This thought isn't particular in light of the fact that any machine serving the demand can conceivably be known as a server. Despite the fact that the server trusts that the customer will begin a discussion, sometimes a similar program may go about as both customer and server. In that sense, a solitary machine can go about as a system giving the correspondence between the customer and the server program that experiences layers of a TCP/IP convention stack. An attachment is an API given by the OS to understand the association. The bundle java.net gives the vital fixings to execute the attachment correspondence between two of the highest TCP/IP layers: application and transport. The article expounds the idea driving the customer/server demonstrate with hands-on subtleties in making a TCP customer/server application in Java.
• Java UDP Listener <-> Java UDP 
One of the models where UDP is favored over TCP is the live inclusion of TV channels. In this angle, we need to transmit however many edges to live group of onlookers as would be prudent not stressing over the loss of a couple of edges. TCP being a solid convention include its own overhead while transmission. 

Another model where UDP is favoured is online multiplayer gaming. In recreations like counter-strike or honourable obligation, it isn't important to transfer all the data yet the most essential ones. It ought to likewise be noticed that the majority of the applications, in actuality, utilizes watchful mix of both UDP and TCP; transmitting the basic information over TCP and rest of the information by means of UDP.
• C# TCP Listener <-> C# TCP 
In this application you have 3 sections, the server (a class record), the correspondence portion (a class archive) and the client application. We will look at all 3 of these parts freely, and how they can join to make your basic visit application. The essential fragment, the visit server, is the place the messages are sent forward and in reverse between the client and the server. Before forming any strategies, you need to add the going with references to your class. 
 ![image](https://user-images.githubusercontent.com/58506840/104924843-f600fd00-59d8-11eb-9a60-62e95167732a.png)



• C# UDP Listener <-> C# UDP 
The information structure used to trade between the customer and the server is appeared as follows. Attachments transmit and get information as a variety of bytes, the over-burden constructor and the ToByte part work plays out this conversion. One vital point to note here is that, in UDP, there is no such refinement between the customer and server applications. In contrast to TCP, UDP servers don't tune in for approaching customers; they simply search for information originating from different customers. When we get information, we check whether it's a message for login, logout, and so forth
• Java TCP Listener <-> C# TCP 
The information structure used to trade between the customer and the server is appeared as follows. Attachments transmit and get information as a variety of bytes, the over-burden constructor and the ToByte part work plays out this conversion.One vital point to note here is that, in UDP, there is no such refinement between the customer and server applications. In contrast to TCP, UDP servers don't tune in for approaching customers; they simply search for information originating from different customers. When we get information, we check whether it's a message for login, logout, and so forth.
• Java UDP Listener <-> C# UDP 
I could have composed the code in C or C++, yet I picked Java for a few reasons. To start with, the applications are all the more flawlessly and neatly written in Java; with Java there are less lines of code, and each line can be disclosed to the beginner developer absent much trouble. Second, customer server programming in Java is ending up progressively mainstream, and may even turn into the standard in up and coming years. Java is stage free, it has exemption systems for strong treatment of normal issues that happen amid I/O and systems administration tasks, and its threading offices give an approach to effortlessly actualize ground-breaking servers.
• C# TCP Listener <-> Java TCP 
On the off chance that I was making an association among customer and server utilizing TCP, it has few usefulness like, TCP is suited for applications that require high dependability, and transmission time is generally less basic. It is utilized by different conventions like HTTP, HTTPs, FTP, SMTP, Telnet. TCP adjusts information bundles in the request indicated. There is unshakable certainty that the information exchanged stays unblemished and touches base in a similar request in which it was sent. TCP flows Control and requires three bundles to set up an attachment association, before any client information can be sent. TCP handles dependability and blockage control. It additionally does mistake checking and blunder recuperation. Incorrect parcels are retransmitted from the source to the goal
• C# UDP Listener <-> Java UDP
In UDP, the customer does not shape an association with the server like in TCP and rather just sends a datagram. Also, the server requires not acknowledge an association and just hangs tight for datagrams to arrive. Datagrams upon entry contain the location of sender which the server uses to send information to the right customer.
3. Test 
 
The execution of the test instrument in C# is genuinely straight forward. The .NET structure library gives us simple to utilize organizing classes in System.Net.Sockets. We utilize the Tcp Client and the Udp Client as the premise of our customer association classes. The multi-threading is similarly simple. We use System.Threading.Thread and essentially need to give the capacity that we wish our strings to execute. The principle string hangs tight for the laborer strings to finish utilizing a ManualResetEvent. The strings decrement a counter utilizing the Interlocked class. Utilization of the Interlocked class implies that each string is ensured to decrement the counter as a solitary nuclear activity. Without it, two strings getting to the counter in the meantime could prompt surprising conduct. The string that moves the counter to 0 sets the occasion and the fundamental string close down. Arrangement is a breeze utilizing the classes from System.Xml to stack a XML setup record and walk the hubs of the tree.
I was agreeably astonished at the fact that it was so natural to make an interpretation of our plan into code utilizing C# and .NET and the main grumble we have is the absence of genuine various legacy. It would have been decent to have the capacity to have the interfaces, or a class got from the interfaces, give default executions to a few strategies, for example, the MessageTransmitted() and ConversationComplete() techniques and adequately give the client of the interface the alternative to actualize whether they require conduct other than the default.

References
(n.d.). codeproject.com. 
(n.d.). javaworld.com. 


