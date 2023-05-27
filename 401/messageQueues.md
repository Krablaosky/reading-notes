# Message Queues

### [Socket.io Chat Example](https://socket.io/get-started/chat/)

1. Explain to a non-technical recruiter what the Chat Example (above) does.
   * The Chat Example is a simple chat application that allows users to communicate with each other in real-time. It is implemented using Socket.io, a library that enables real-time, bidirectional communication between the server and clients. Users can enter chat messages through an input field, and these messages are instantly displayed on the screens of all connected users. The application creates a web server using Node.js and Express, handles client-server communication using Socket.io, and updates the chat interface dynamically.

2. What proof of life are we getting on the backend from the above app?
   * The proof of life we are getting on the backend from the above app is the console log message "a user connected" when a new user establishes a connection with the server. This log message indicates that the server is receiving connections from clients and is able to handle real-time communication.

3. Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?
   * If we want to send a message to everyone except for a certain emitting socket, we can use the broadcast flag. The socket.broadcast.emit() method is used to emit an event to all connected sockets except the one emitting the event.

### [Rooms](https://socket.io/docs/v4/rooms)

1. What is a room and how might a room be useful?
   * A room is a concept in Socket.io that allows grouping multiple sockets into a virtual channel. It provides a way to organize clients based on a common attribute or purpose.
   * Rooms can be useful in scenarios where you want to broadcast messages or events to a specific group of connected clients rather than broadcasting to all clients. For example, in a chat application, you might have separate rooms for different chat channels or private conversations.

2. How do you join a room?
   * To join a room, a client can use the `socket.join(roomName)` method. By providing the desired room name, the client can become a member of that specific room.

3. how do you leave a room?
   * To leave a room, the client can use the `socket.leave(roomName)` method. This will remove the client from the specified room, and they will no longer receive events specifically targeted to that room.

### [Namespaces](https://socket.io/docs/v4/namespaces/)

1. What is a Namespace and what does it allow you to do?
   * A Namespace in Socket.io is a way to separate different sets of functionality or communication channels within the same application.

2. Each namespace potentially has its own what? (hint: 3 things)
   * Each namespace potentially has its own set of events, rooms, and clients.

3. Discuss a possible use case for separate namespaces
   * Separating functionality into different namespaces can be useful when you want to isolate different parts of your application or when you want to provide different APIs or features to different sets of clients. For example, you could have a namespace for real-time notifications, another namespace for chat functionality, and so on.
   * Using separate namespaces allows you to define different event handlers, rooms, and configurations for each namespace, providing flexibility and organization within your application.

### Bookmarks

[Socket.io Emit Cheatsheet](https://socket.io/docs/v4/emit-cheatsheet/)