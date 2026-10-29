# EXPERIMENT 4

Socket Programming for Transport Layer Packet (UDP Server)

## Terminal Session
```
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ vim udp_server_1290.c
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ gcc udp_server_1290.c -o udp_server
lab-03-17@lab-03-17-OptiPlex-3280-AIO:~$ ./udp_server
UDP Echo Server listening on port 10290...
Received from client: Hello UDP Server
Sent back to client: Hello UDP Server
```

## CONCLUSION
The UDP Server socket was successfully implemented at the Transport Layer. By utilizing `SOCK_DGRAM` with `recvfrom()` and `sendto()`, the server successfully bound to its designated port and processed incoming connectionless datagrams without establishing a prior network handshake.
