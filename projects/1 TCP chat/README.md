# TCP chat server

This simple TCP server receives messages and echoes them back to the client. The client program sets up its socket differently from the way a server does. Instead of binding to a port and listening, it uses connect() to attach the socket directly to the remote address.

## Client-Server Architecture

For our application, we will use the client-server architecture. This means that we will have multiple clients (the users) and one central server that hosts everything and provides the data for these clients.

<img src="https://i.imgur.com/mPCiBLf.png" alt= “” width="350">

Therefore, we will need to write two Python scripts. One will be for starting the server and one will be for the client. We will have to run the server first, so that there is a chat, which the clients can connect to. The clients themselves, are not going to directly communicate to each other but via the central server.

## Running the client

We always need to start the server first because otherwise the clients can’t connect to a non-existing host. Here you can see an example of a chat with two clients (you can also connect with 20 if you want):
