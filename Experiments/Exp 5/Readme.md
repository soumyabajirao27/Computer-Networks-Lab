# EXPERIMENT 5

Socket Programming for Transport Layer Protocol (UDP Client)


## Terminal Session
```
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ vim udp_client_1290.c
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ gcc udp_client_1290.c -o udp_client
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ ./udp_client 127.0.0.1
Enter message to send: Hello UDP Server
Echo from server: Hello UDP Server
```

## CONCLUSION
The UDP Client socket was successfully implemented at the Transport Layer. Using connectionless datagram sockets (`SOCK_DGRAM`) along with `sendto()` and `recvfrom()`, the client successfully transmitted and received packets from the server without requiring a dedicated connection circuit or prior handshake.
