# TCP chat server

A TCP chat server written in Python.

This simple TCP server receives messages and echoes them back to the client. The client program sets up its socket differently from the way a server does. Instead of binding to a port and listening, it uses connect() to attach the socket directly to the remote address.
