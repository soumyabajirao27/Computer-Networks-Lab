# EXPERIMENT 3

Socket Programming for Transport Layer Packets (TCP Client)

## Terminal Session
```
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ vim client_1290.c
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ gcc client_1290.c -o client
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ ./client 127.0.0.1
Connected to server. Enter message: Hello Server
Echo from server: Hello Server
```

## CONCLUSION
The TCP Client socket was successfully constructed at the Transport Layer. Using the active open mechanism (socket, setting server parameters, and connect), the client successfully established a connection with the server via the TCP Three-Way Handshake and enabled reliable stream-based data transmission.
