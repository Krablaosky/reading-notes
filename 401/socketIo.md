# Socket.io

### [Web Sockets](https://en.wikipedia.org/wiki/WebSocket)

1. What is a Web Socket?
   * A Web Socket is a communication protocol that provides a persistent, full-duplex connection between a client (usually a web browser) and a server. It enables real-time bidirectional communication, allowing both the client and server to send data to each other at any time without the need for frequent polling.

2. Describe the Web Socket request/response handshake and what happens once the connection is established.
   * The Web Socket request/response handshake begins with the client sending an HTTP request to the server, expressing its desire to upgrade the connection to a WebSocket. If the server supports WebSocket connections, it responds with an HTTP 101 status code, indicating a successful upgrade. Once the connection is established, the communication switches from the HTTP protocol to the WebSocket protocol.
   * Once the connection is established, both the client and server can freely send data to each other without the overhead of HTTP request/response headers. This enables real-time, low-latency communication between the two parties. The client and server can exchange messages, and any updates or events can be sent and received instantly.

3. Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client.
   * Web Sockets provide a standardized way for the server to send content to a client without the client explicitly requesting it. In traditional HTTP, the client initiates requests to the server, and the server responds with the requested content. However, with Web Sockets, the server can proactively send data to the client whenever there is new information or updates available, without waiting for the client to request it. This enables real-time data streaming and push notifications, among other use cases.

### [Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)

1. What does the event handler io.on() do?
   * The event handler io.on() in Socket.io is used to listen for incoming events from clients. It allows the server to handle events emitted by clients using the Socket.io library. The server can define specific event names to listen for and provide corresponding callback functions to handle those events.

2. Describe some possible proof of life or proof that the code works as expected
   * Possible proofs of life or checks to ensure that the code works as expected in a Socket.io application could include:
     * Verifying that the server is successfully running and listening for incoming connections on the specified port.
     * Checking if clients can connect to the server and establish WebSocket connections.
     * Emitting test events from the client and confirming that the server receives and handles those events correctly.
     * Sending messages or data from the server to the client and ensuring that the client receives and processes them as expected.
     * Testing scenarios where multiple clients are connected and verifying that the server can handle and broadcast events to all connected clients.

3. What does socket.emit() do?
   * The function socket.emit() in Socket.io is used to emit or send an event from the client to the server or from the server to a specific client. It allows the client or server to send custom events with data to other connected clients or the server itself. The event name and the associated data can be specified as arguments to the socket.emit() function.a

### [Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/)

1. What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).
   * WebSocket is a protocol that provides a standardized way for creating a full-duplex communication channel between a client and a server. It is a low-level protocol that operates at the transport layer of the networking stack.
   * Socket.IO, on the other hand, is a library that uses WebSocket as the underlying transport protocol but also provides additional features and abstractions. It simplifies the usage of WebSockets and adds features like automatic reconnection, support for fallback mechanisms (such as long polling) in environments where WebSocket connections may not be available, and support for broadcasting messages to multiple clients.

2. When would you use Socket.IO?
   * Socket.IO is commonly used when building real-time applications that require bidirectional communication between the server and clients. It provides additional features and abstractions on top of WebSockets, making it easier to handle real-time events, handle disconnections, and support a wide range of clients, including browsers, mobile devices, and other servers.

3. When would you use WebSockets?
   * WebSockets are a good choice when you need a low-level, full-duplex communication channel between a client and a server. They are suitable for scenarios where you require high-performance, real-time data exchange and don't need the additional features and abstractions provided by libraries like Socket.IO. Using WebSockets directly gives you more control but also requires more manual handling of connection management and event dispatching.  

### [OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0)

1. What are a couple of key takeaways from this video?
   * The OSI (Open Systems Interconnection) model is a conceptual framework that helps in understanding how different network protocols and technologies work together to enable communication between devices.
   * The OSI model consists of seven layers, each responsible for specific functions and tasks related to data transmission and communication.
   * The layers of the OSI model include the Physical layer, Data Link layer, Network layer, Transport layer, Session layer, Presentation layer, and Application layer.
   * Each layer has its own set of protocols and functions, and data passes through these layers from the sender to the receiver during communication.
   * The OSI model provides a standard reference for network architects and engineers to design, troubleshoot, and understand how different networking components interact with each other.

### [TCP Handshakes Explained](https://www.youtube.com/watch?v=xMtP5ZB3wSk)
 

2. Translate the gist of this video to a non-technical friend
   * Imagine you want to have a conversation with your friend, but you're not sure if they're available or if they can hear you. So, before you start talking, you perform a handshake to ensure a proper connection.
   * In computer networks, when two devices want to communicate with each other using a protocol called TCP (Transmission Control Protocol), they also go through a handshake process to establish a reliable connection.
   * The handshake involves a series of steps where the devices exchange messages to confirm that they are ready and capable of receiving and sending data.
   * During the handshake, the devices agree on certain parameters, such as the size of data packets they can handle, and set up a unique identification for the connection.
   * Once the handshake is complete and both devices are satisfied with the agreement, they can start sending and receiving data.
   * The handshake ensures that the communication between devices is reliable and that both sides are ready to exchange information.
   * Just like in a conversation with your friend, the handshake in computer networks helps establish a connection and sets the stage for smooth communication.

### Bookmarks

[Socket.io Documentation](https://socket.io/docs/)

[Socket.io Server API](https://socket.io/docs/server-api)

[Socket.io Client API](https://socket.io/docs/client-api)

[Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)

## [Back](../401readingNotes.md)