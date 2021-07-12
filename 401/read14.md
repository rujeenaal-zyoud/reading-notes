# Message Queues


1. **What does it mean that web sockets are bidirectional? Why is this useful?**

it works both ways, meaning that both parties can send and receive at the same time. (either the client or server can send a message to the other party whenever a message is available)

2. **Does socket.io use HTTP? Why?**

Yes, socket use HTTP at the beginning to initialize the connection between the server and the client then after establish connection it start using TCP. Also if the TCP fall down socket io will start using HTTP.

3. **What happens when a client emits an event?**
If the server is listening to that event, the server will execute the handler function for that event.

4. **What happens when a server emits an event?**
All listening clients will execute the handler for that event.


5. **What happens if a client “misses” an event?**

this means there are no listening to that event or the emitter accrue before the listener, i

6. **How can we mitigate this?**
confirms that the client received the first emit in the first place




# Terms
1. **Socket :**
a socket is an endpoint of a communication between two programs running on a network. Sockets are used to create a connection between a client program and a server program.


2. **Web Socket**
WebSocket is its own layer 7 protocol, similar to HTTP. WebSockets create a full-duplex connection for sending messages from client to server, or server to client at any instant. This pattern is far superior to HTTP request-response when an application requires systems to get the latest data ASAP.

3. **Socket.io**
Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server.


4. **Client**
A client is a connection on the frontend.

5. **Server**
A system that provides services to other systems in its network.

6. **OSI Model**
is a conceptual framework used to describe the functions of a networking system

7. **TCP Model**
TCP/IP model (Transmission Control Protocol/Internet Protocol) is a model with four layers which is for both modelling current Internet architecture, as well as providing a set a rules that govern all forms of transmission over a network.

8. **TCP**
TCP (Transmission Control Protocol) is a protocol for sending information between computers. TCP guarantees* that all the information will be sent and that it will be received in order.

9. **UDP**

User Datagram Protocol: is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet. It speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party.

10. **Packets**

is a small segment of a larger message. Data sent over computer networks, such as the Internet, is divided into packets. These packets are then recombined by the computer or device that receives them.



## Preparation Materials
 ### Socket.io Chat Example
Sockets have traditionally been the solution around which most real-time chat systems are architected, providing a bi-directional communication channel between a client and a server.

for chat Server You will need to have node.js installed. We will be using express to simplify setup.


### Rooms and Namespaces
A room is an arbitrary channel that sockets can join and leave.

It can be used to broadcast events to a subset of clients
rooms are a server-only concept (i.e. the client does not have access to the list of rooms it has joined).

**Default room**
Each Socket in Socket.IO is identified by a random, unguessable, unique identifier Socket#id. For your convenience, each socket automatically joins a room identified by its own id.

**Sample use cases**
broadcast data to each device / tab of a given user send notifications about a given entity

Usage with asynchronous code
Please make sure to use io.to(...).emit(...) (or socket.to(...).emit(...)) in a synchronous 

**Disconnection**
Upon disconnection, sockets leave all the channels they were part of automatically, and no special teardown is needed on your part.

You can fetch the rooms the Socket was in by listening to the disconnecting event:



