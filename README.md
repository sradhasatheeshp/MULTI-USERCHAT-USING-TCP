# MULTI-USERCHAT-USING-TCP

Aim: To implement a client server chats using TCP.

Algorithm

SERVER

• Include appropriate header files.

• Create a TCP Socket.

• Fill in the socket address structure (with server information)

• Specify the port where the service will be defined to be used by client.

• Bind the address and port using bind() system call.

• Server executes listen() system call to indicate its willingness to receive connections.

• Accept the next completed connection from the client process by using an accept()
system call.

• Create a new process (child process) using fork(), to handle the client request.

• parent process will be waiting for new incoming connections.

• Receive a message from the Client using recv() system call.

• Write the message thus obtained from each client on the standard output.

CLIENT

• Include appropriate header files

• Create a TCP Socket.

• Fill in the socket address structure (with server information)

• Specify the port of the Server, where it is providing service

• Establish connection to the Server using connect() system call.

• Each client connected with server can send a message to the server using send() system Call.
