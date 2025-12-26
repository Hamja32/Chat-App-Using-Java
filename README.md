# Chat-App-Using-Java
Java Socket Chat Application A multi-client real-time chat application built using Java Sockets and multithreading.
📄 Chat Application – Workflow Explanation (LinkedIn / README)

# Java Socket Based Chat Application – Workflow
This project is a console-based multi-client chat application built using Java Sockets and Multithreading.

# The application follows a client-server architecture:
Server Side
The server starts on a specific port using ServerSocket.
It continuously listens for incoming client connections.
For every new client, a separate ClientHandler thread is created.
This allows multiple clients to chat simultaneously without blocking each other.

Client Handling
Each client sends their username when they connect.
The server stores all active clients in a shared list.
Whenever a client sends a message, it is broadcasted to all other connected clients.

Multithreading
Every client runs on its own thread.
This ensures real-time message delivery and smooth communication.
Message Broadcasting
Messages are sent using buffered streams (BufferedReader & BufferedWriter).
The server relays messages to all clients except the sender.

Client Disconnect Handling
When a client leaves, the server removes them from the active list.
A notification message is broadcasted to remaining users.

Technologies Used
Java
Socket Programming
Multithreading
I/O Streams

This project helped me understand network programming, concurrency, and real-time communication concepts in Java.
Result : link
